---
title: Gebeurtenissen configureren
description: 'Wanneer het vormen van een bericht in-app in de gebeurtenissen van Adobe Campaign Standard (ACS) bepaalt welke gebruiker in werking gestelde actie het bericht zal teweegbrengen om worden getoond. '
feature: In-App
topics: Mobile
kt: 2548
thumbnail: 26245.jpg
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 11263e247184ddc6a8e3df6a8ed0899907fbb366
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 3%

---


# Configureren [!UICONTROL Events] {#configuring-events}

Wanneer het vormen van een [!UICONTROL In-App] bericht, moet u bepalen welke gebruiker-in werking gestelde actie het te tonen bericht teweegbrengt. Deze acties worden [!UICONTROL events] genoemd. Er zijn drie categorieën van [!UICONTROL events] beschikbaar: [!UICONTROL Mobile Application events], [!UICONTROL Life Cycle events] en [!UICONTROL Analytics events].

## [!UICONTROL Mobile Application Events] {#mobile-application-events}

[!UICONTROL Mobile Application events] zijn  [!UICONTROL custom events] die zijn geïmplementeerd in uw mobiele toepassing.

Voorbeelden zijn:

* Een klant heeft een onderdeel bekeken
* Een klant voegt een item aan het winkelwagentje toe
* Lozing van winkelwagentjes
* Een klant heeft iets gekocht

U moet deze [!UICONTROL events] in Adobe Campaign vormen. In de volgende video wordt beschreven hoe u dit doet.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Life Cycle events]  {#life-cycle-events}

[!UICONTROL Lifecycle events] buiten de doos  [!UICONTROL events]. De volgende [!UICONTROL events] zijn beschikbaar:

* [!UICONTROL launched]
* [!UICONTROL upgraded]
* [!UICONTROL crashed]

Een voorbeeld van een gebruiksgeval zou een bericht kunnen zijn introducerend nieuwe eigenschappen na een verbetering, of een gebeurtenisbevordering.

>[!NOTE]
>
>[!UICONTROL Lifecycle module] moet in de mobiele toepassing worden gevormd. Zie hier voor meer informatie over [Lifecycle toevoegen aan uw app](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics Events] {#analytics-events}

De volgende drie categorieën worden ondersteund, afhankelijk van wat er van instrumenten wordt voorzien in uw mobiele app:

* Adobe Analytics
* [!UICONTROL Context data]
* [!UICONTROL View state]

>[!NOTE]
>
>[!UICONTROL Analytics events] een Adobe Analytics-licentie vereisen. Zodra u [[!DNL Analytics] uitbreiding hebt gevormd ](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) en [Analytics aan uw App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app) toegevoegd, worden deze gebeurtenissen beschikbaar in de [!UICONTROL In-App] configuratie in ACS.

## Aanvullende bronnen

* [Levenscyclusstatistieken inschakelen (documentatie)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
