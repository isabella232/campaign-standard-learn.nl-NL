---
title: Stap 1 - Een Android-toepassing maken en configureren voor gebruik van Firebase Cloud Messaging
description: In dit deel zullen we [!DNL Android] App to receive [!UICONTROL Push notifications] uit Adobe Campaign Standard ontstaan. Om de pushberichten te ontvangen, moet de app zijn geregistreerd bij Google [!DNL Firebase Cloud Service].
feature: Push
topics: Mobile
kt: 4825
doc-type: tutorial
activity: use
team: TM
translation-type: tm+mt
source-git-commit: afe1ae6c8d73b7b776e0eec327fa16db76c23ce1
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 2%

---


# Stap 1 - Het creëren van [!DNL Android] App en het vormen aan gebruik [!DNL Firebase Cloud Messaging]

In dit gedeelte maakt u een [!DNL Android] app die u van Adobe Campaign Standard kunt [!UICONTROL Push notifications] ontvangen. Om de pushberichten te ontvangen, moet de app worden geregistreerd bij Google [!DNL Firebase Cloud Service].

1. Meld u aan bij uw [!DNL Firebase] account.

   [!DNL Firebase] is het mobiele platform van Google waarmee u snel hoogwaardige apps kunt ontwikkelen. Als u geen [!DNL Firebase] account hebt, kunt u [hier](https://firebase.google.com)een account maken.

2. Starten [!DNL Android Studio]
3. Klik op **[!UICONTROL File]** > **[!UICONTROL New]** > **[!UICONTROL New Project].**
4. Selecteer **[!UICONTROL Empty Activity]** en klik op **[!UICONTROL Next].**

   ![android-project](assets/android-project.PNG)

5. Geef het project een betekenisvolle naam.

   In het kader van deze demo hebben wij ons project aangeduid als *[!DNL ACSPushTutorial]*

   ![android-project-configuration](assets/android-project-configuration.PNG)

6. Accepteer de standaardpakketnamen en klik **[!DNL Finish]** om uw project te maken.
7. De projectstructuur moet er ongeveer zo uitzien als hieronder opgenomen scherm

   ![android-projectstructuur](assets/android-project-structure.PNG)

8. Klik op **[!UICONTROL Tools]** > **[!UICONTROL Firebase].**(hiermee wordt het project toegevoegd aan[!DNL Firebase])
9. Klik op **[!UICONTROL Set up Firebase Cloud Messaging].**

   ![installatiefirewall](assets/android-project-firebase-messaging.PNG)

10. Klik op **[!UICONTROL Connect to Firebase].**
11. Klik op de knop nadat de app is verbonden met Firebase **[!UICONTROL Add FCM to your app].**
12. Klik op **[!UICONTROL Accept Changes].**

   Wanneer u FCM aan uw app toevoegt, heeft de wizard uw toestemming nodig om enkele wijzigingen in uw project aan te brengen.

   ![[!DNL add-fcm-to-your-app]](assets/firebase-add-fcm-to-app.PNG)

Als uw app met Firebase is geïntegreerd, ontvangt u een bericht zoals hieronder:

![[!DNL fcm-successfull]](assets/android-firebase-success.PNG)

[Zorg ervoor uw project vermeld [!DNL Firebase ]binnen console is](https://console.firebase.google.com/)

## Instellingen [!UICONTROL Push Channel] configureren

1. Aanmelden bij [!DNL Firebase] console
2. Open het **[!UICONTROL ACSPushTutorial]** project.
3. Klik op het **tandwielpictogram** en open de projectinstellingen

   ![projectinstellingen](assets/firebase-project-settings.PNG)

4. Tab to the **[!UICONTROL Cloud Messaging]** tab.
5. De serversleutel kopiëren

   ![serversleutel](assets/firebase-server-key.PNG)

6. Aanmelden bij uw Adobe Campaign Standard-exemplaar
7. Klik op **[!UICONTROL Adobe Campaign]** > **[!UICONTROL Administration]** > **[!UICONTROL Channels]** > **[!UICONTROL Mobile App].**
8. Selecteer de gewenste optie **[!UICONTROL Mobile Application Property].**
9. Klik op het **[!DNL Android]pictogram **in de **[!UICONTROL Push Channel settings]**sectie.
10. Plak de serversleutel in het veld met de serversleutel.

Als alles goed gaat, zou u een SUCCESS bericht moeten zien.

![push-channel-instellingen](assets/push-channel-settings.PNG)

Samenvattend, hebben wij een [!DNL Android App] en verbonden met [!DNL Android App] met [!DNL Firebase]. Vervolgens hebben we de Mobile App in Adobe Campaign verbonden met de [!DNL Android App] app door de serversleutel van de [!DNL Android] App in de Mobile App in Adobe Campaign Standard te plakken.
