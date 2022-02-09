---
title: Gebeurtenissen configureren
description: '"Begrijp hoe gebeurtenissen bepalen welke actie van de gebruiker een bericht in-app teweegbrengt om te worden getoond. ’'
feature: In App
kt: 2548
thumbnail: 26245.jpg
doc-type: feature video
activity: use
team: TM
exl-id: 2c7937f4-b0da-46e5-934e-c660012c2c6f
role: User, Developer
level: Beginner, Intermediate
source-git-commit: 57dbf456625d22cd2e4526d92e5a8c20a048d339
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 2%

---

# Configureren [!UICONTROL Events] {#configuring-events}

Wanneer u een [!UICONTROL In-App] bericht, moet u bepalen welke gebruiker-in werking gestelde actie het te tonen bericht teweegbrengt. Deze handelingen worden [!UICONTROL events]. Drie categorieën [!UICONTROL events] zijn beschikbaar: [!UICONTROL Mobile Application events], [!UICONTROL Life Cycle events], en [!UICONTROL Analytics events].

## [!UICONTROL Mobile Application Events] {#mobile-application-events}

[!UICONTROL Mobile Application events] zijn [!UICONTROL custom events] die zijn geïmplementeerd in uw mobiele toepassing.

Voorbeelden zijn:

* Een klant heeft een onderdeel bekeken
* Een klant voegt een item aan het winkelwagentje toe
* Lozing van winkelwagentjes
* Een klant heeft iets gekocht

U moet deze configureren [!UICONTROL events] in Adobe Campaign. In de volgende video wordt beschreven hoe u dit doet.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Life Cycle events] {#life-cycle-events}

[!UICONTROL Lifecycle events] buiten de box [!UICONTROL events]. Het volgende [!UICONTROL events] zijn beschikbaar:

* [!UICONTROL launched]
* [!UICONTROL upgraded]
* [!UICONTROL crashed]

Een voorbeeld van een gebruiksgeval zou een bericht kunnen zijn introducerend nieuwe eigenschappen na een verbetering, of een gebeurtenisbevordering.

>[!NOTE]
>
>De [!UICONTROL Lifecycle module] moet worden geconfigureerd in de mobiele toepassing. Zie hier voor meer informatie over [Lifecycle toevoegen aan uw app](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics Events] {#analytics-events}

De volgende drie categorieën worden ondersteund, afhankelijk van wat er van instrumenten wordt voorzien in uw mobiele app:

* Adobe Analytics
* [!UICONTROL Context data]
* [!UICONTROL View state]

>[!NOTE]
>
>[!UICONTROL Analytics events] een Adobe Analytics-licentie vereisen. Zodra u [[!DNL Analytics] extensie geconfigureerd](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) en toegevoegd [Analyses voor uw app](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app)Deze gebeurtenissen zijn beschikbaar in het dialoogvenster [!UICONTROL In-App] configuratie in ACS.
