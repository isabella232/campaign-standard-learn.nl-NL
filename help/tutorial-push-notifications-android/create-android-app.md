---
title: Stap 1 - Een Android-toepassing maken en configureren voor gebruik van Firebase Cloud Messaging
description: In dit onderdeel maken we  [!DNL Android] App to receive [!UICONTROL Push notifications] verzonden vanuit Adobe Campaign Standard. Om de pushberichten te ontvangen, moet de app worden geregistreerd bij Google's [!DNL Firebase Cloud Service].
feature: Push
topics: Mobile
kt: 4825
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: cdd78e97f2769503d3d4f26933ccc7f35e9b20b9
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 2%

---


# Stap 1 - het Creëren van [!DNL Android] Toepassing en het vormen om [!DNL Firebase Cloud Messaging] te gebruiken

In dit onderdeel maakt u [!DNL Android]-app om [!UICONTROL Push notifications] te ontvangen die u van Adobe Campaign Standard hebt verzonden. Om de pushberichten te ontvangen, moet de app worden geregistreerd bij [!DNL Firebase Cloud Service] van Google.

1. Meld u aan bij uw [!DNL Firebase]-account.

   [!DNL Firebase] is het mobiele platform van Google waarmee u snel hoogwaardige apps kunt ontwikkelen. Als u geen [!DNL Firebase]-account hebt, maakt u een [van hier](https://firebase.google.com).

2. [!DNL Android Studio] starten
3. Klik op **[!UICONTROL File]** > **[!UICONTROL New]** > **[!UICONTROL New Project].**
4. Selecteer **[!UICONTROL Empty Activity]** en klik op **[!UICONTROL Next].**

   ![android-project](assets/android-project.PNG)

5. Geef het project een betekenisvolle naam.

   Voor deze demo hebben we ons project *[!DNL ACSPushTutorial]* genoemd

   ![android-project-configuration](assets/android-project-configuration.PNG)

6. Accepteer de standaardpakketnamen en klik op **[!DNL Finish]** om uw project te maken.
7. De projectstructuur moet er ongeveer zo uitzien als hieronder opgenomen scherm

   ![android-projectstructuur](assets/android-project-structure.PNG)

8. Klik op **[!UICONTROL Tools]** > **[!UICONTROL Firebase].** (hiermee wordt het project toegevoegd aan  [!DNL Firebase])
9. Klik op **[!UICONTROL Set up Firebase Cloud Messaging].**

   ![installatiefirewall](assets/android-project-firebase-messaging.PNG)

10. Klik op **[!UICONTROL Connect to Firebase].**
11. Nadat uw app is verbonden met Firebase, klikt u op **[!UICONTROL Add FCM to your app].**
12. Klik op **[!UICONTROL Accept Changes].**

   Wanneer u FCM aan uw app toevoegt, heeft de wizard uw toestemming nodig om enkele wijzigingen in uw project aan te brengen.

   ![[!DNL add-fcm-to-your-app]](assets/firebase-add-fcm-to-app.PNG)

Als uw app met Firebase is geïntegreerd, ontvangt u een bericht zoals hieronder:

![[!DNL fcm-successfull]](assets/android-firebase-success.PNG)

[Zorg ervoor uw project vermeld  [!DNL Firebase ]binnen console is](https://console.firebase.google.com/)

## [!UICONTROL Push Channel]-instellingen configureren

1. Aanmelden bij [!DNL Firebase]-console
2. Open het **[!UICONTROL ACSPushTutorial]** project.
3. Klik op het tandwielpictogram **en open de projectinstellingen**

   ![projectinstellingen](assets/firebase-project-settings.PNG)

4. Tab naar het tabblad **[!UICONTROL Cloud Messaging]**.
5. De serversleutel kopiëren

   ![serversleutel](assets/firebase-server-key.PNG)

6. Aanmelden bij uw Adobe Campaign Standard-exemplaar
7. Klik op **[!UICONTROL Adobe Campaign]** > **[!UICONTROL Administration]** > **[!UICONTROL Channels]** > **[!UICONTROL Mobile App].**
8. Selecteer de juiste **[!UICONTROL Mobile Application Property].**
9. Klik op het pictogram **[!DNL Android]** in de sectie **[!UICONTROL Push Channel settings]**.
10. Plak de serversleutel in het veld met de serversleutel.

Als alles goed gaat, zou u een SUCCESS bericht moeten zien.

![push-channel-instellingen](assets/push-channel-settings.PNG)

Om samen te vatten, hebben wij [!DNL Android App] gecreeerd en [!DNL Android App] met [!DNL Firebase] verbonden. Vervolgens hebben we de Mobile App in Adobe Campaign verbonden met de [!DNL Android App] door de serversleutel van de [!DNL Android] App in te plakken op de Mobile App in Adobe Campaign Standard.
