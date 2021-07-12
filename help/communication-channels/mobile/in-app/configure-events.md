---
title: Gebeurtenissen configureren
description: '"Begrijp hoe gebeurtenissen bepalen welke actie van de gebruiker een bericht in-app teweegbrengt om te worden getoond. ’'
feature: In app
kt: 2548
thumbnail: 26245.jpg
doc-type: feature video
activity: use
team: TM
exl-id: 2c7937f4-b0da-46e5-934e-c660012c2c6f
role: User, Developer
level: Beginner, Intermediate
source-git-commit: 2be2719ddd84490b796d9abc6300376fa896ff0c
workflow-type: tm+mt
source-wordcount: '215'
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

## [!UICONTROL Life Cycle events] {#life-cycle-events}

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
