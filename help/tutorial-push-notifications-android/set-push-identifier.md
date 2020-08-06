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
source-git-commit: c3ff1a137fb8ee9506a11f82e1a27d010bbd97e6
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Stap 4 - Instellen [!DNL pushidentifier]

De tekenreeks **[!DNL pushidentifier]** bevat de apparaattoken voor [!DNL Push] meldingen. Dit is het zelfde teken dat door wordt verzonden [!DNL Firebase] en tot SDK gebruikend de [!DNL MobileCore.setPushIdentifier] methode overgegaan.

Open je project in [!DNL Android ]studio. Verwijder de gehele code in [!DNL MainActivity] behalve de eerste regel die de pakketinstructie **** is.

Plak de volgende code in [!DNL MainActivity]:

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
* De [!DNL Android] emulator moet starten en uw app moet met [!DNL "Hello World" ]tekst worden uitgevoerd.
* Open het [!DNL logcat] venster. Zoek naar &quot;[!DNL Got]&quot;. U zou het teken moeten zien dat van [!DNL Firebase] geschreven aan het logboek zoals hieronder getoond werd ontvangen. De lange tekenreeks na &quot;[!DNL Got token]&quot; is de tekenreeks [!DNL pushidentifier ]die naar Adobe Campaign wordt verzonden.

![logcat-token](assets/logcat-got-token.PNG)

### Abonnees voor mobiele toepassingen controleren

Meld u aan bij uw Adobe Campaign Standard-exemplaar.
Navigeren **[!UICONTROL Administration->Channels->Mobile App(AEP SDK)]**. Open de juiste mobiele toepassing. Tab to the [!UICONTROL Mobile Application Subscribers] tab. Je moet een [!UICONTROL registration token ]lijst zien.

![mobiele applicatie-abonnees](assets/mobile-application-subscribers.PNG)

>[OPMERKING]
>Als u geen registratietoken ziet in de [!UICONTROL Mobile Application Subscribers] tab STOP hier voordat u verdergaat.
