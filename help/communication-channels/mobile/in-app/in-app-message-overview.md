---
title: Inleiding tot in-app-berichten
description: '"Leer hoe u de gebruiker contextafhankelijke berichten in de app kunt presenteren als reactie op het realtime gedrag van de klant in de mobiele toepassing."'
feature: In app
topics: Mobile
kt: 1911
doc-type: feature video
activity: use
team: TM
exl-id: c51716eb-7239-4fc0-9ccf-9f5f0a5fae65
role: Business Practitioner
level: Beginner
translation-type: tm+mt
source-git-commit: 07c2696cbdc72e24563c5d1442bf5c39b22d5a22
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 21%

---

# Inleiding tot [!UICONTROL In-App] berichten {#introduction}

Met het kanaal [!UICONTROL In-App Messaging] kunt u een bericht weergeven wanneer de gebruiker actief is in de mobiele toepassing. Voor dit kanaal moeten mobiele toepassingen worden geïntegreerd met [!UICONTROL Adobe Experience Platform SDK].

In deze zelfstudie worden de stappen beschreven die nodig zijn voor het instellen van de mobiele eigenschappen, de extensie [!UICONTROL Launch] voor het [!UICONTROL In-App Messaging]-kanaal en voor het voorbereiden, aanpassen en verzenden van [!UICONTROL In-App]-berichten in Adobe Campaign Standard. De koppelingen leiden u naar de videozelfstudies over elk van de gemarkeerde onderwerpen.

## Vereisten {#prerequisites}

1. Zorg ervoor u tot **[!UICONTROL In-App]** kanaal kunt toegang hebben. Neem contact op met uw accountteam als u geen toegang hebt tot deze kanalen.
1. Controleer of uw **gebruiker** de vereiste **toestemmingen** in Adobe Campaign Standard en [!UICONTROL Launch] heeft.

   1. Zorg er in Adobe Campaign Standard voor dat de IMS-gebruiker deel uitmaakt van de groepen [!UICONTROL Standard User] en [!UICONTROL Administrator].\
      Met deze stap kan de gebruiker zich aanmelden bij Adobe Campaign Standard, naar de pagina voor de mobiele app van de SDK van het Experience Platform navigeren en de eigenschappen van de mobiele app weergeven die u hebt gemaakt in [!UICONTROL Launch].
   1. Controleer in [!UICONTROL Launch] of uw IMS-gebruiker deel uitmaakt van een [!UICONTROL Launch]-productprofiel.\
      Met deze stap kan de gebruiker zich aanmelden bij [!UICONTROL Launch] om de eigenschappen te maken en weer te geven. Zie [Uw productprofiel maken](https://docs.adobelaunch.com/launch-reference/administration/user-permissions#3-create-your-product-profile) voor meer informatie over productprofielen in [!UICONTROL Launch]. In het productprofiel, zou er geen toestemmingen moeten zijn die op het bedrijf of de eigenschappen worden geplaatst, maar de gebruiker zou nog login moeten kunnen.

1. In Adobe Experience Platform Launch:

   1. Maak de mobiele toepassing door een mobiele eigenschap te maken en gebruik de SDK van het Experience Platform voor uw mobiele app.
   1. Installeer de extensie **Adobe Campaign Standard** voor uw mobiele toepassing.

Raadpleeg voor meer informatie over extensies de extensie [Campaign Standard configureren in Adobe Launch](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-campaign-standard) in [!UICONTROL Adobe Launch ]documentatie.

## Stappen voor het instellen van [!UICONTROL In-App]-berichten {#steps-to-set-up}

1. [Een mobiele applicatie configureren met behulp van de Adobe Experience Platform SDK](/help/communication-channels/mobile/configure-mobile-apps-using-aep-sdk.md).

1. [Configureer gebeurtenissen](/help/communication-channels/mobile/in-app/configure-events.md).

## [!UICONTROL In-App] Leveringen {#create-manage-publish} maken, beheren en publiceren

U kunt of één keer leveringen in-app door op **[!UICONTROL Create an In-App Message]** kaart van de homepage, van [!UICONTROL Marketing Activities] te klikken, of u kunt [een levering in-app binnen een werkschema creëren](/help/communication-channels/mobile/in-app/in-app-activity.md).

Bij het instellen van de levering hebt u drie mogelijkheden om uw gebruikers als doel in te stellen door een keuze te maken uit verschillende leveringssjablonen:

1. [**Een bericht in de app uitzenden**](/help/communication-channels/mobile/in-app/broadcast-in-app-message.md) om alle gebruikers van een mobiele app te bereiken.

   Met dit berichttype kunt u berichten verzenden naar alle (huidige of toekomstige) gebruikers van uw mobiele applicatie, zelfs als ze geen bestaand profiel hebben in Adobe Campaign. Personalisatie is daarom niet mogelijk wanneer de berichten worden aangepast omdat het gebruikersprofiel niet noodzakelijkerwijs bestaat in Adobe Campaign.

1. Stel alle gebruikers in op basis van hun profiel voor mobiele apps.

   Met dit berichttype kunt u zich richten op alle bekende of anonieme gebruikers van een mobiele app met een mobiel profiel in Adobe Campaign. Dit berichttype kan worden gepersonaliseerd met alleen niet-persoonlijke en niet-gevoelige kenmerken en vereist geen veilige handshake tussen Mobile SDK en de in-app-berichtenservice van Adobe Campaign. De verpersoonlijkingsstrategie is dus gebaseerd op wat u over de gebruikers hebt geleerd van hun interactie met het apparaat. Bijvoorbeeld alle gebruikers die hun app in de afgelopen week meer dan vijf keer hebben gestart.

1. [**Gebruikers doelgericht benaderen op basis van hun Campaign-profiel**](/help/communication-channels/mobile/in-app/target-users-based-on-campaign-profile.md).

   Met dit berichttype kunt u zich richten op Adobe Campaign-profielen (CRM-profielen) die zijn geabonneerd op uw mobiele applicatie. Het bericht kan met alle beschikbare profielattributen in Adobe Campaign worden gepersonaliseerd maar vereist een veilige handdruk tussen Mobile SDK en de het overseinendienst van de Campagne In-App om ervoor te zorgen dat de berichten met persoonlijke en gevoelige informatie door erkende gebruikers slechts worden gebruikt.

Deze sjabloon is handig ter ondersteuning van gevallen waarin gebruikers al op andere kanalen zoals E-mail of Push zijn aangewezen en die op hun reactie zijn gebaseerd, wilt u hen een bericht in de app geven.

## Rapport over uw in-app leveringen {#report}

Zodra uw levering is gepubliceerd, kunt u [op uw levering in-app ](/help/communication-channels/mobile/in-app/in-app-reporting.md) melden.

## Aanvullende bronnen

* [Rapport in app](https://docs.adobe.com/content/help/en/campaign-standard/using/reporting/list-of-reports/in-app-report.html)
* [Een mobiele eigenschap instellen](https://aep-sdks.gitbook.io/docs/getting-started/create-a-mobile-property)
* [Een mobiele toepassing configureren met Adobe Experience Platform SDK&#39;s](https://helpx.adobe.com/nl/campaign/kb/configuring-app-sdk.html)
* [Een in-app-bericht voorbereiden en verzenden](https://docs.adobe.com/content/help/en/campaign-standard/using/communication-channels/in-app-messaging/preparing-and-sending-an-in-app-message.html)
* [Een in-app-bericht aanpassen](https://docs.adobe.com/content/help/en/campaign-standard/using/communication-channels/in-app-messaging/customizing-an-in-app-message.html)
* [Een in-app-bericht verzenden binnen een workflow](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/channel-activities/in-app-delivery.html)
* [Levenscyclusmetriek inschakelen](https://aep-sdks.gitbook.io/docs/getting-started/initialize-the-sdk#enable-lifecycle-metrics)
