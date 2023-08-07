---
title: Stap 2 - De mobiele SDK integreren
description: In dit deel integreren we de Android-toepassing met de Mobile SDK. Mobiele SDK integreren met de Android-app
feature: Push
user: Admin
level: Experienced
jira: KT-4826
doc-type: tutorial
activity: use
team: TM
recommendations: noDisplay
exl-id: 0fa53536-8330-4e96-be2f-afc078609bcd
source-git-commit: 913d2c08dc63e2073b3abd1de6b6b16711d817da
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# STAP 2 - Integreer [!UICONTROL Mobile SDK] met Android-app

In dit deel zullen wij de [!DNL Android] app met [!UICONTROL Mobile SDK]. Om te integreren [!UICONTROL mobile SDK] met de [!DNL Android] te gebruiken, voert u de volgende stappen uit:

* Open de *ACSPushTutorial* project in [!DNL Android Studio]
* Een nieuwe Java-klasse maken met de naam *MainApp* die zich uitbreidt [!DNL android.app.Application]
* Uw projectstructuur op dit punt zou hieronder moeten kijken

![main-app](assets/android-main-app.PNG)

* Breid uit [!DNL Gradle Scripts] map. Dubbelklik op de knop [!DNL build.gradle] van de module. Plak de volgende afhankelijkheden in de sectie voor afhankelijkheden van de [!DNL build.gradle] bestand. Uw [!DNL build.gradle] bestand moet er nu als volgt uitzien

<!--
Removed `{.line-numbers}` below
-->

```java
implementation 'com.adobe.marketing.mobile:campaign:1.+'
implementation 'com.adobe.marketing.mobile:userprofile:1.+'
implementation 'com.adobe.marketing.mobile:sdk-core:1.+'
```

![modulewrijving](assets/module-build-gradle.PNG)

* Synchroniseer uw [!DNL Android] project door op de knop Nu synchroniseren te klikken om uw project te synchroniseren

## Wijzigen [!DNL AndroidManifest.xml]{#modify-android-manifest}

Openen *AndroidManifest.xml* en plak de volgende twee regels na het manifestelement en vóór het toepassingselement. Hierdoor kan uw app communiceren met externe gebruikers

<!--
Removed `{.line-numbers}` below
-->

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```

Kopieer de volgende regel in het toepassingselement
[!DNL android:name=".MainApp"]
Sla uw [!DNL AndroidManifest.xml]
Uw [!DNL AndroidManifest.xml] moet er zo uitzien

<!--
Removed `{.line-numbers}` below
-->

```xml
<?xml version="1.0" encoding="utf-8"?>
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="com.example.acspushtutorial">
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

<activity android:name=".MainActivity">
<intent-filter>
    <action android:name="android.intent.action.MAIN" />
    <category android:name="android.intent.category.LAUNCHER" />
</intent-filter>
</activity>
</application>

</manifest>
```
