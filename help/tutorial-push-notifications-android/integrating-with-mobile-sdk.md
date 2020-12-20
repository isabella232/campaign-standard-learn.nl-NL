---
title: Stap 2 - De mobiele SDK integreren
description: In dit deel integreren we de Android-toepassing met de Mobile SDK. Mobiele SDK integreren met de Android-app
feature: Push
topics: Mobile
kt: 4826
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 13b4f1d395dfe53f9fc5263e7b06be700e30b986
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# STAP 2 - [!UICONTROL Mobile SDK] integreren met Android-toepassing

In dit deel integreren we de [!DNL Android]-toepassing met [!UICONTROL Mobile SDK]. Ga als volgt te werk om [!UICONTROL mobile SDK] te integreren met de [!DNL Android]-app:

* Open het *ACSPushTutorial*-project in [!DNL Android Studio]
* Maak een nieuwe Java-klasse met de naam *MainApp* die [!DNL android.app.Application] uitbreidt
* Uw projectstructuur op dit punt zou hieronder moeten kijken

![main-app](assets/android-main-app.PNG)

* Vouw de map [!DNL Gradle Scripts] uit. Dubbelklik op [!DNL build.gradle] van de module. Plak de volgende afhankelijkheden in de sectie voor afhankelijkheden van het [!DNL build.gradle]-bestand. Uw [!DNL build.gradle]-bestand moet er nu als hieronder uitzien

<!--
Removed `{.line-numbers}` below
-->

```java
implementation 'com.adobe.marketing.mobile:campaign:1.+'
implementation 'com.adobe.marketing.mobile:userprofile:1.+'
implementation 'com.adobe.marketing.mobile:sdk-core:1.+'
```

![modulewrijving](assets/module-build-gradle.PNG)

* Synchroniseer uw [!DNL Android] project door op de knop Synchroniseren nu te klikken om uw project te synchroniseren

## [!DNL AndroidManifest.xml]{#modify-android-manifest} wijzigen

Open *AndroidManifest.xml* en plak de volgende twee regels na het manifest-element en vóór het toepassingselement. Hierdoor kan uw app communiceren met externe gebruikers

<!--
Removed `{.line-numbers}` below
-->

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```

Kopieer de volgende regel in het toepassingselement
[!DNL android:name=".MainApp"]
Uw [!DNL AndroidManifest.xml] opslaan
Uw [!DNL AndroidManifest.xml] moet er als volgt uitzien

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
