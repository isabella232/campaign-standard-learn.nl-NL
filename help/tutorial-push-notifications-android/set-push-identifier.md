---
title: STAP 4 - Push-id instellen
description: De **pushIdentifier** is een tekenreeks die het apparaattoken voor pushberichten bevat. Dit is hetzelfde token dat door Firebase wordt verzonden en via de methode MobileCore.setPushIdentifier aan de SDK wordt doorgegeven.
feature: Push
topics: MOBILE
kt: 4828
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: aa01c2f8fe1560468d0d8f3fae6291bb82f9a21f
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Stap 4 - Set [!DNL pushidentifier]

De **[!DNL pushidentifier]** is een tekenreeks die de apparaattoken voor [!DNL Push]-berichten bevat. Dit is het zelfde teken dat door [!DNL Firebase] wordt verzonden en tot SDK gebruikend de [!DNL MobileCore.setPushIdentifier] methode wordt overgegaan.

Open uw project in [!DNL Android ]studio. Verwijder de gehele code in [!DNL MainActivity] **behalve de eerste regel die uw pakketinstructie** is.

Plak de volgende code in [!DNL MainActivity]:

<!--
Removed `{.line-numbers}` below
-->

```java
import androidx.annotation.NonNull;
import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.util.Log;
import android.widget.Toast;

import com.adobe.marketing.mobile.MobileCore;
import com.google.android.gms.tasks.OnCompleteListener;
import com.google.android.gms.tasks.Task;
import com.google.firebase.iid.FirebaseInstanceId;
import com.google.firebase.iid.InstanceIdResult;

public class MainActivity extends AppCompatActivity {

@Override
protected void onCreate(Bundle savedInstanceState) {
super.onCreate(savedInstanceState);
setContentView(R.layout.activity_main);

registerToken();
}

void registerToken() {
FirebaseInstanceId.getInstance().getInstanceId()
    .addOnCompleteListener(new OnCompleteListener<InstanceIdResult>() {
        @Override
        public void onComplete(@NonNull Task<InstanceIdResult> task) {
            if (!task.isSuccessful()) {
                Log.w("Message App", "getInstanceId failed", task.getException());
                return;
            }

// Get new Instance ID token
String token = task.getResult().getToken();

Log.d("Got token", token);

MobileCore.setPushIdentifier(token);
}
});
}

@Override
public void onResume() {
super.onResume();
MobileCore.setApplication(getApplication());
MobileCore.lifecycleStart(null);
}

@Override
public void onPause() {
super.onPause();
MobileCore.lifecyclePause();
}
}
```

## Uw app testen

Het is nu een goed moment om uw app te testen voordat u verder gaat.

* Voer uw app uit door op de groene pijl te klikken of selecteer **[!DNL Run->Run'app']**.
* De emulator [!DNL Android] moet worden gestart en uw app moet worden uitgevoerd met [!DNL "Hello World" ]tekst.
* Open het venster [!DNL logcat]. Zoeken naar &quot;[!DNL Got]&quot;. U zou het teken moeten zien dat van [!DNL Firebase] werd ontvangen die aan het logboek zoals hieronder wordt geschreven. De lange tekenreeks na &quot;[!DNL Got token]&quot; is de [!DNL pushidentifier ]die naar Adobe Campaign wordt verzonden.

![logcat-token](assets/logcat-got-token.PNG)

### Abonnees voor mobiele toepassingen controleren

Meld u aan bij uw Adobe Campaign Standard-exemplaar.
Navigeer **[!UICONTROL Administration->Channels->Mobile App(AEP SDK)]**. Open de juiste mobiele toepassing. Tab naar het tabblad [!UICONTROL Mobile Application Subscribers]. Er wordt een [!UICONTROL registration token ]vermeld.

![mobiele applicatie-abonnees](assets/mobile-application-subscribers.PNG)

>[!NOTE]
>
>Als u geen registratietoken ziet in de [!UICONTROL Mobile Application Subscribers] lusje STOP hier alvorens verder te gaan.
