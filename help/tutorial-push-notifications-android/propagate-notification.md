---
title: Stap 5 - Meldingen doorgeven
description: In dit deel geven we het bericht door dat we van Adobe Campaign hebben ontvangen via Android Notification Manager.Firebase
feature: Push
jira: KT-4829
doc-type: tutorial
activity: use
team: TM
exl-id: b0e01224-4ddc-4999-b8c6-794e49245428
source-git-commit: c84867ef59a10448a377a959d0b67ae71343a4aa
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---

# Service toevoegen om melding te verzenden

In dit deel geven we het bericht dat we van Adobe Campaign hebben ontvangen door [!DNL Android Notification Manager]. [!DNL Notification manager] wordt gebruikt om de gebruiker op de hoogte te stellen van gebeurtenissen die plaatsvinden.
Zo vertelt u de gebruiker dat er iets op de achtergrond is gebeurd:

* Starten [!DNL Android Studio]
* Openen *[!DNL ACSPushTutorial]* project
* De projectstructuur uitbreiden
* Klik met de rechtermuisknop op de pakketmap ([!DNL com.example.acspushtutorial]) en [!DNL New ->Java Class]
* Deze klasse een naam geven *[!DNL MyService]* en ervoor zorgen dat het zich uitbreidt [!DNL FirebaseMessagingService]
* Maken *[!DNL sendNotification]* in deze klasse. In deze methode moet u de inhoud en het kanaal van het bericht instellen met een [!DNL NotificationCompat.Builder] object. Om het bericht te maken verschijnen, roep [!DNL NotificationManagerCompat.notify()], door het een unieke id voor de melding en het resultaat van [!DNL NotificationCompat.Builder.build()].

<!--
Removed `{.line-numbers}` below
-->

```java
package com.example.pushmessaging;
import android.app.NotificationChannel;
import android.app.NotificationManager;
import android.app.PendingIntent;
import android.content.Context;
import android.content.Intent;
import android.media.RingtoneManager;
import android.net.Uri;
import android.os.Build;
import android.util.Log;

import androidx.core.app.NotificationCompat;

import com.google.firebase.messaging.FirebaseMessagingService;
import com.google.firebase.messaging.RemoteMessage;

import java.util.Map;

public class MyService extends FirebaseMessagingService {
@Override
public void onMessageReceived(RemoteMessage remoteMessage)
{
Map<String,String> data  = remoteMessage.getData();
Log.d("data payload: ", data.toString());
sendNotification(remoteMessage);
}


private void sendNotification(RemoteMessage message) {
Intent intent = new Intent(this, MainActivity.class);
intent.addFlags(Intent.FLAG_ACTIVITY_CLEAR_TOP);
PendingIntent pendingIntent = PendingIntent.getActivity(this, 0 /* Request code */, intent, PendingIntent.FLAG_ONE_SHOT);

String channelId = "0";
Uri defaultSoundUri = RingtoneManager.getDefaultUri(RingtoneManager.TYPE_NOTIFICATION);
NotificationCompat.Builder notificationBuilder =
        new NotificationCompat.Builder(this, channelId)
                .setSmallIcon(R.drawable.ic_launcher_background)
                .setContentTitle("Message from AEM")
                .setContentText(message.getData().get("body"))
                .setAutoCancel(true)
                .setSound(defaultSoundUri)
                .setContentIntent(pendingIntent);

NotificationManager notificationManager =
        (NotificationManager) getSystemService(Context.NOTIFICATION_SERVICE);

// Since android Oreo notification channel is needed.
if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.O) {
    NotificationChannel channel = new NotificationChannel(channelId,
            "Channel human readable title",
            NotificationManager.IMPORTANCE_DEFAULT);
    notificationManager.createNotificationChannel(channel);
}

notificationManager.notify(0 /* ID of notification */, notificationBuilder.build());
}
}
```

## Wijzigen [!DNL AndroidManifest.xml]

Voeg de dienst toe die aan uw werd gecreeerd [!DNL AndroidManifest.xml]. De definitieve [!DNL AndroidManifest.xml] zou als hieronder moeten kijken:

<!--
Removed `{.line-numbers}` below
-->

```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.pushmessaging">

    <uses-permission android:name="android.permission.INTERNET" />
    <uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />

    <application
        android:name=".MainApp"
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/AppTheme">
        <service
            android:name=".MyService"
            android:exported="false">
            <intent-filter>
                <action android:name="com.google.firebase.MESSAGING_EVENT" />
            </intent-filter>
        </service>

        <activity android:name=".MainActivity">
            <intent-filter>
                <action android:name="android.intent.action.MAIN" />

                <category android:name="android.intent.category.LAUNCHER" />
            </intent-filter>
        </activity>
    </application>

</manifest>
```

## De app uitvoeren

Voer de app uit door op de knop **groene pijl** op de werkbalk of van de [!DNL Run] -menu.
