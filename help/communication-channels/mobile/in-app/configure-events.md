---
title: Gebeurtenissen configureren
description: 'Wanneer het vormen van een bericht in-app in de gebeurtenissen van Adobe Campaign Standard (ACS) bepaalt welke gebruiker in werking gestelde actie het bericht zal teweegbrengen om worden getoond. '
feature: In-App
topics: Mobile
kt: 2548
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 82fb2d39dc61a55c0aa20ca1fa215f35a7dd9088
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Configureren [!UICONTROL Events] {#configuring-events}

Wanneer het vormen van een [!UICONTROL In-App] bericht, moet u bepalen welke gebruiker-in werking gestelde actie het te tonen bericht teweegbrengt. Deze acties worden genoemd [!UICONTROL events]. Er [!UICONTROL events] zijn drie categorieën beschikbaar: [!UICONTROL Mobile Application events], [!UICONTROL Life Cycle events]en [!UICONTROL Analytics events].

## [!UICONTROL Mobile Application Events] {#mobile-application-events}

[!UICONTROL Mobile Application events] zijn [!UICONTROL custom events] die zijn geïmplementeerd in uw mobiele toepassing.

Voorbeelden zijn:

* Een klant heeft een onderdeel bekeken
* Een klant voegt een item aan het winkelwagentje toe
* Lozing van winkelwagentjes
* Een klant heeft iets gekocht

U moet deze configureren [!UICONTROL events] in Adobe Campaign. In de volgende video wordt beschreven hoe u dit doet.

>[!VIDEO](https://video.tv.adobe.com/v/26245?quality=12)

## [!UICONTROL Life Cycle events]  {#life-cycle-events}

[!UICONTROL Lifecycle events] buiten de doos [!UICONTROL events]. Het volgende [!UICONTROL events] is beschikbaar:

* [!UICONTROL launched]
* [!UICONTROL upgraded]
* [!UICONTROL crashed]

Een voorbeeld van een gebruiksgeval zou een bericht kunnen zijn introducerend nieuwe eigenschappen na een verbetering, of een gebeurtenisbevordering.

>[!NOTE]
>
>Het [!UICONTROL Lifecycle module] moet worden geconfigureerd in de mobiele toepassing. Zie hier voor meer informatie over [hoe u de levenscyclus van uw app kunt toevoegen](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/mobile-core/lifecycle)

## [!UICONTROL Analytics Events] {#analytics-events}

De volgende drie categorieën worden ondersteund, afhankelijk van wat er van instrumenten wordt voorzien in uw mobiele app:

* Adobe Analytics
* [!UICONTROL Context data]
* [!UICONTROL View state]

>[!NOTE]
>
>[!UICONTROL Analytics events] een Adobe Analytics-licentie vereisen. Zodra u de gevormde [[!DNL Analytics] ](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#configure-analytics-extension-in-launch) uitbreiding hebt en [Analytics aan uw App](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-analytics#add-analytics-to-your-app)hebt toegevoegd, worden deze gebeurtenissen beschikbaar in de [!UICONTROL In-App] configuratie in ACS.

## Aanvullende bronnen

* [Levenscyclusstatistieken inschakelen (documentatie)](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
