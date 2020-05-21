---
title: Inleiding tot In-App-berichten
description: Met het communicatiekanaal van Adobe Campagne Standard (ACS) In-App Messaging kunt u de gebruiker contextafhankelijk berichten in de app presenteren als reactie op het real-time gedrag van de klant in de mobiele toepassing.
feature: In-App
topics: Mobile
kt: 1911
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 82fb2d39dc61a55c0aa20ca1fa215f35a7dd9088
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---


# Inleiding tot [!UICONTROL In-App] berichten {#introduction}

Met het [!UICONTROL In-App Messaging] kanaal kunt u een bericht weergeven wanneer de gebruiker actief is in de mobiele toepassing. Voor dit kanaal moeten mobiele toepassingen worden geïntegreerd met [!UICONTROL Adobe Experience Platform SDK].

In deze zelfstudie worden de stappen beschreven die nodig zijn om de mobiele eigenschappen, de [!UICONTROL Launch] extensie voor het [!UICONTROL In-App Messaging] kanaal in te stellen, en wordt uitgelegd hoe u [!UICONTROL In-App] berichten kunt voorbereiden, aanpassen en verzenden in Adobe Campaign Standard. De koppelingen leiden u naar de videozelfstudies over elk van de gemarkeerde onderwerpen.

## Vereisten {#prerequisites}

1. Controleer of u toegang hebt tot het **[!UICONTROL In-App]** kanaal. Neem contact op met uw accountteam als u deze kanalen niet kunt openen.
1. Controleer of uw **gebruiker** beschikt over de benodigde **machtigingen** in Adobe Campagne Standard en [!UICONTROL Launch].

   1. Controleer in Adobe Campaign Standard of de IMS-gebruiker deel uitmaakt van de [!UICONTROL Standard User] groep en de [!UICONTROL Administrator] groep.\
      Met deze stap kan de gebruiker zich aanmelden bij Adobe Campagne Standard, naar de pagina voor mobiele apps voor het Experience Platform SDK navigeren en de eigenschappen van de mobiele app bekijken die u hebt gemaakt in [!UICONTROL Launch].
   1. Controleer [!UICONTROL Launch]in dat geval of uw IMS-gebruiker deel uitmaakt van een [!UICONTROL Launch] productprofiel.\
      Met deze stap kan de gebruiker zich aanmelden om de eigenschappen te maken [!UICONTROL Launch] en weer te geven. Zie [!UICONTROL Launch]Uw productprofiel [maken voor meer informatie over productprofielen in](https://docs.adobelaunch.com/launch-reference/administration/user-permissions#3-create-your-product-profile). In het productprofiel, zou er geen toestemmingen moeten zijn die op het bedrijf of de eigenschappen worden geplaatst, maar de gebruiker zou nog login moeten kunnen.

1. In Adobe Experience Platform Launch:

   1. Maak de mobiele toepassing door een mobiele eigenschap te maken en instrumenteer uw mobiele app met Experience Platform SDK.
   1. Installeer de extensie **Adobe Campagne Standard** voor uw mobiele toepassing.

Raadpleeg voor meer informatie over extensies de extensie Campagne Standard [configureren in Adobe Launch](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-campaign-standard) in de [!UICONTROL Adobe Launch ]documentatie.

## Stappen voor het instellen van [!UICONTROL In-App] berichten {#steps-to-set-up}

1. [Configureer een mobiele toepassing met de Adobe Experience Platform SDK](/help/communication-channels/mobile/configure-mobile-apps-using-aep-sdk.md).

1. [Configureer gebeurtenissen](/help/communication-channels/mobile/in-app/configure-events.md).

## Leveringen maken, beheren en publiceren [!UICONTROL In-App] {#create-manage-publish}

U kunt ofwel één keer In-App-leveringen maken door op de **[!UICONTROL Create an In-App Message]** kaart van de startpagina, van de pagina te klikken [!UICONTROL Marketing Activities], of u kunt een In-App-levering [maken binnen een workflow](/help/communication-channels/mobile/in-app/in-app-activity.md).

Bij het instellen van de levering hebt u drie mogelijkheden om uw gebruikers als doel in te stellen door een keuze te maken uit verschillende leveringssjablonen:

1. [**Een bericht **](/help/communication-channels/mobile/in-app/broadcast-in-app-message.md)in de app uitzenden voor alle gebruikers van een mobiele app.

   Met dit berichttype kunt u berichten verzenden naar alle gebruikers (huidige of toekomstige) van uw mobiele toepassing, zelfs als deze geen bestaand profiel hebben in Adobe Campagne. Personalisatie is daarom niet mogelijk bij het aanpassen van de berichten omdat het gebruikersprofiel niet noodzakelijkerwijs bestaat in Adobe Campaign.

1. Stel alle gebruikers in op basis van hun profiel voor mobiele apps.

   Met dit berichttype kunt u zich richten op alle bekende of anonieme gebruikers van een mobiele app met een mobiel profiel in Adobe Campagne. Dit berichttype kan worden gepersonaliseerd gebruikend slechts niet-persoonlijke en niet-gevoelige attributen en vereist geen veilige handdruk tussen Mobile SDK en de het overseinendienst van de Campagne van Adobe in-App. De verpersoonlijkingsstrategie is dus gebaseerd op wat u over de gebruikers hebt geleerd van hun interactie met het apparaat. Bijvoorbeeld alle gebruikers die hun app in de afgelopen week meer dan vijf keer hebben gestart.

1. [**Doelgebruikers op basis van hun campagneprofiel **](/help/communication-channels/mobile/in-app/target-users-based-on-campaign-profile.md).

   Met dit berichttype kunt u zich richten op Adobe Campagne-profielen (CRM-profielen) die zijn geabonneerd op uw mobiele toepassing. Het bericht kan met alle beschikbare profielattributen in de Campagne van Adobe worden gepersonaliseerd maar vereist een veilige handdruk tussen Mobile SDK en de het overseinendienst van de Campagne In-App om ervoor te zorgen dat de berichten met persoonlijke en gevoelige informatie door erkende gebruikers slechts worden gebruikt.

Deze sjabloon is handig ter ondersteuning van gevallen waarin gebruikers al op andere kanalen zoals E-mail of Push zijn aangewezen en die op hun reactie zijn gebaseerd, wilt u hen een bericht in de app geven.

## Rapport over uw In-App-leveringen {#report}

Zodra uw levering is gepubliceerd, kunt u [op uw levering](/help/communication-channels/mobile/in-app/in-app-reporting.md)in-app melden.

## Aanvullende bronnen

* [Rapport in app](https://docs.adobe.com/content/help/en/campaign-standard/using/reporting/list-of-reports/in-app-report.html)
* [Een mobiele eigenschap instellen](https://aep-sdks.gitbook.io/docs/getting-started/create-a-mobile-property)
* [Een mobiele toepassing configureren met SDK&#39;s van het Adobe Experience Platform](https://helpx.adobe.com/campaign/kb/configuring-app-sdk.html)
* [Een bericht in de app voorbereiden en verzenden](https://docs.adobe.com/content/help/en/campaign-standard/using/communication-channels/in-app-messaging/preparing-and-sending-an-in-app-message.html)
* [Een bericht in de app aanpassen](https://docs.adobe.com/content/help/en/campaign-standard/using/communication-channels/in-app-messaging/customizing-an-in-app-message.html)
* [Een bericht in de app verzenden binnen een workflow](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/channel-activities/in-app-delivery.html)
* [Levenscyclusmetriek inschakelen](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
