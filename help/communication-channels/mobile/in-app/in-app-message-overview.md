---
title: Inleiding tot in-app-berichten
description: Leer hoe u de gebruiker contextafhankelijke berichten in de app kunt presenteren als reactie op het realtime gedrag van de klant in de mobiele toepassing.
feature: In App
kt: 1911
doc-type: feature video
activity: use
team: TM
exl-id: c51716eb-7239-4fc0-9ccf-9f5f0a5fae65
role: User
level: Beginner
source-git-commit: 57dbf456625d22cd2e4526d92e5a8c20a048d339
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 21%

---

# Inleiding tot [!UICONTROL In-App] berichten {#introduction}

De [!UICONTROL In-App Messaging] kunt u een bericht weergeven wanneer de gebruiker actief is in de mobiele toepassing. Voor dit kanaal moeten mobiele toepassingen worden geïntegreerd met [!UICONTROL Adobe Experience Platform SDK].

In deze zelfstudie worden de stappen beschreven die nodig zijn om de mobiele eigenschappen in te stellen. [!UICONTROL Launch] voor de [!UICONTROL In-App Messaging] kanaal, en hoe te voorbereidingen te treffen, aan te passen en te verzenden [!UICONTROL In-App] berichten in Adobe Campaign Standard. De koppelingen leiden naar de videozelfstudies over elk van de gemarkeerde onderwerpen.

## Vereisten {#prerequisites}

1. Zorg ervoor dat u toegang hebt tot de **[!UICONTROL In-App]** kanaal. Neem contact op met uw accountteam als u geen toegang hebt tot deze kanalen.
1. Controleer of uw **user** de nodige **machtigingen** in Adobe Campaign Standard en [!UICONTROL Launch].

   1. Zorg er in Adobe Campaign Standard voor dat de IMS-gebruiker deel uitmaakt van de [!UICONTROL Standard User] en [!UICONTROL Administrator] groepen.

      Met deze stap kan de gebruiker zich aanmelden bij Adobe Campaign Standard, naar de pagina voor de mobiele app van de SDK van het Experience Platform navigeren en de eigenschappen van de mobiele app bekijken die u in [!UICONTROL Launch].

   1. In [!UICONTROL Launch], zorgt u ervoor dat uw IMS-gebruiker deel uitmaakt van een [!UICONTROL Launch] productprofiel. Met deze stap kan de gebruiker zich aanmelden bij [!UICONTROL Launch] om de eigenschappen te maken en weer te geven. In het productprofiel, zou er geen toestemmingen moeten zijn die op het bedrijf of de eigenschappen worden geplaatst, maar de gebruiker zou nog login moeten kunnen.

1. In Adobe Experience Platform Launch:

   1. Maak de mobiele toepassing door een mobiele eigenschap te maken en gebruik de SDK van het Experience Platform voor uw mobiele app.
   1. Installeer de **Adobe Campaign Standard** voor uw mobiele toepassing.

Voor meer informatie over extensies raadpleegt u [Campaign Standard-extensie configureren in Adobe Launch](https://aep-sdks.gitbook.io/docs/using-mobile-extensions/adobe-campaign-standard) in de documentatie.

## Stappen die moeten worden ingesteld [!UICONTROL In-App] berichten {#steps-to-set-up}

1. [Een mobiele applicatie configureren met behulp van de Adobe Experience Platform SDK](/help/communication-channels/mobile/configure-mobile-apps-using-aep-sdk.md).
1. [Gebeurtenissen configureren](/help/communication-channels/mobile/in-app/configure-events.md).

## Maken, beheren en publiceren [!UICONTROL In-App] Leveringen {#create-manage-publish}

U kunt eenmalige In-App-leveringen maken door op de knop **[!UICONTROL Create an In-App Message]** kaart van de homepage, van de [!UICONTROL Marketing Activities]of u kunt [Een levering in de app maken binnen een workflow](/help/communication-channels/mobile/in-app/in-app-activity.md).

Wanneer u de levering instelt, hebt u drie opties om uw gebruikers als doel in te stellen door uit verschillende leveringssjablonen te kiezen:

1. [**Een bericht in de app uitzenden**](/help/communication-channels/mobile/in-app/broadcast-in-app-message.md) om alle gebruikers van een mobiele app als doel in te stellen.

   Met dit berichttype kunt u berichten verzenden naar alle (huidige of toekomstige) gebruikers van uw mobiele applicatie, zelfs als ze geen bestaand profiel hebben in Adobe Campaign. Personalisatie is daarom niet mogelijk wanneer de berichten worden aangepast omdat het gebruikersprofiel niet noodzakelijkerwijs bestaat in Adobe Campaign.

1. Stel alle gebruikers in op basis van hun profiel voor mobiele apps.

   Met dit berichttype kunt u zich richten op alle bekende of anonieme gebruikers van een mobiele app met een mobiel profiel in Adobe Campaign. Dit berichttype kan worden gepersonaliseerd met alleen niet-persoonlijke en niet-gevoelige kenmerken en vereist geen veilige handshake tussen Mobile SDK en de in-app-berichtenservice van Adobe Campaign. Dus, is de verpersoonlijkingsstrategie gebaseerd op wat u over de gebruikers van hun interactie met het apparaat hebt geleerd. Bijvoorbeeld alle gebruikers die hun app in de afgelopen week meer dan vijf keer hebben gestart.

1. [**Gebruikers doelgericht benaderen op basis van hun Campaign-profiel**](/help/communication-channels/mobile/in-app/target-users-based-on-campaign-profile.md).

   Met dit berichttype kunt u zich richten op Adobe Campaign-profielen (CRM-profielen) die zijn geabonneerd op uw mobiele applicatie. Het bericht kan worden gepersonaliseerd met alle beschikbare profielkenmerken in Adobe Campaign. Het vereist een veilige handdruk tussen Mobiele SDK en de het overseinendienst van de Campagne in-App om ervoor te zorgen dat de berichten met persoonlijke en gevoelige informatie door erkende gebruikers slechts worden gebruikt.

Deze sjabloon is handig ter ondersteuning van gevallen waarin gebruikers al zijn aangewezen op andere kanalen, zoals E-mail of Push. Gebaseerd op hun reactie, wilt u hen dan met een bericht in-app in dienst nemen.

## Rapport over uw In-App-leveringen {#report}

Zodra uw levering is gepubliceerd, kunt u [rapport over uw levering in de app](/help/communication-channels/mobile/in-app/in-app-reporting.md).
