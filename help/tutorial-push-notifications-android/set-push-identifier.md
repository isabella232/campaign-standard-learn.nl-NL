---
title: STAP 4 - Push-id instellen
description: De **pushIdentifier** is een tekenreeks die het apparaattoken voor pushberichten bevat. Het is hetzelfde token dat door Firebase wordt verzonden en via de methode MobileCore.setPushIdentifier aan de SDK wordt doorgegeven.
feature: Push
jira: KT-4828
doc-type: tutorial
activity: use
team: TM
exl-id: 08387b84-edaa-45ee-ae66-53bcbd5c7c39
source-git-commit: c84867ef59a10448a377a959d0b67ae71343a4aa
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Stap 4 - Instellen [!DNL pushidentifier]

De **[!DNL pushidentifier]** is een tekenreeks die de apparaattoken bevat voor [!DNL Push] meldingen. Het is dezelfde token die wordt verzonden door [!DNL Firebase] en wordt doorgegeven aan de SDK met behulp van de [!DNL MobileCore.setPushIdentifier] methode.

Open uw project in [!DNL Android™]studio. Gehele code verwijderen in [!DNL MainActivity] **behalve de eerste regel die de pakketinstructie is**.

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
* De [!DNL Android™] de emulator moet starten en uw app moet worden uitgevoerd met [!DNL "Hello World"]tekst.
* Open de [!DNL logcat] venster. Zoeken naar &quot;[!DNL Got]&quot;. U moet de token zien die is ontvangen van [!DNL Firebase] geschreven naar het logbestand, zoals hieronder wordt weergegeven. De lange tekenreeks na &quot;[!DNL Got token]&quot; is de [!DNL pushidentifier]die naar Adobe Campaign wordt verzonden.

![logcat-token](assets/logcat-got-token.PNG)

### Abonnees voor mobiele toepassingen controleren

Meld u aan bij uw Adobe Campaign Standard-exemplaar.
Navigeren **[!UICONTROL Administration->Channels->Mobile App(Experience Platform SDK)]**. Open de juiste mobiele toepassing. Tab naar het tabblad [!UICONTROL Mobile Application Subscribers] tab. U dient een [!UICONTROL registration token]vermeld.

![mobiele applicatie-abonnees](assets/mobile-application-subscribers.PNG)

>[!NOTE]
>
>Als u geen registratietoken ziet in het dialoogvenster [!UICONTROL Mobile Application Subscribers] hier STOPPEN voordat u verder gaat.
