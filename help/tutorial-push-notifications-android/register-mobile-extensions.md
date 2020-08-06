---
title: Stap 3 - Extensies registreren voor uw mobiele app
description: In dit deel voegen we de code toe voor het registreren van de extensies Gebruikersprofiel, Identiteit, Levenscyclus en Signaal.
feature: Push
topics: Mobile
kt: 4827
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: c3ff1a137fb8ee9506a11f82e1a27d010bbd97e6
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Stap 3 - Extensies registreren voor uw mobiele app

In dit deel voegen we de code toe voor het registreren van de extensies Gebruikersprofiel, Identiteit, Levenscyclus en Signaal. Deze uitbreidingen maken deel uit van [[!UICONTROL Mobile Core Extensions]](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core). We moeten ook de Adobe Campaign Standard-extensie registreren, zoals in de onderstaande code wordt getoond.

Open je project in [!DNL Android] studio. Verwijder de gehele code in MainApp **behalve de eerste regel die de pakketinstructie** is.

Plak de volgende code in MainApp

```java
import [!DNL android].app.Application;
import android.util.Log;

import com.adobe.marketing.mobile.AdobeCallback;
import com.adobe.marketing.mobile.Campaign;
import com.adobe.marketing.mobile.Identity;
import com.adobe.marketing.mobile.InvalidInitException;
import com.adobe.marketing.mobile.Lifecycle;
import com.adobe.marketing.mobile.LoggingMode;
import com.adobe.marketing.mobile.MobileCore;
import com.adobe.marketing.mobile.Signal;
import com.adobe.marketing.mobile.UserProfile;

public class MainApp extends Application {

@Override
public void onCreate() {
super.onCreate();

MobileCore.setApplication(this);
MobileCore.setLogLevel(LoggingMode.DEBUG);

try{
    Campaign.registerExtension();
    UserProfile.registerExtension();
    Identity.registerExtension();
    Lifecycle.registerExtension();
    Signal.registerExtension();
    MobileCore.start(new AdobeCallback () {
        @Override
        public void call(Object o) {
            MobileCore.configureWithAppID("copy your launch property id here");
        }
    });
} catch (InvalidInitException e) {
    Log.d("ACS Exception", "exception");
}
}
}
```

Lijn 32 u moet milieu identiteitskaart van uw[!UICONTROL  Launch] Bezit verstrekken. Dit kan vanaf de [!UICONTROL environment tab] van uw [!UICONTROL Launch] bezit worden betreden.

![launch-id](assets/launch-id-property.PNG)
