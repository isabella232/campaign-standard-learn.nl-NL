---
title: Problemen oplossen met het Configuratiescherm
description: Met het Configuratiescherm kunt u uw SFTP-opslag per instantie controleren en beheren en IP-adressen op lijsten van gewenste adressen plaatsen.
feature: Control Panel
topics: null
kt: 2938
doc-type: article
activity: use
team: PM
translation-type: tm+mt
source-git-commit: f120eaf237378db3ddd5833930c0222ee028941d
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 100%

---


# Het oplossen van problemen met het [!UICONTROL Control Panel]

Leer hoe u problemen met het gebruik van het Configuratiescherm kunt oplossen.

## Aanmelding en startpagina

Problemen met aanmelding en de startpagina.

### Probleem: Kan niet aanmelden bij Adobe Experience Cloud

**Oplossing:**
De gebruiker moet zijn of haar [!DNL IMS Org ID] (xxx) opzoeken. De beheerder moet de gebruiker toevoegen aan het [!UICONTROL product profile] [!DNL “Campaign-xxx-Admins”] voor elke instantie die de gebruiker wil beheren. Als de gebruiker een beheerder van alle instanties is, moet hij of zij zichzelf mogelijk toch nog toevoegen als *[!UICONTROL user]*.

### Probleem: Gebruiker ziet de koppelingen in [!UICONTROL Adobe Experience Cloud Home] voor toegang tot het [!UICONTROL Control Panel] niet

**Oorzaak:**
Gebruikers zien de koppelingen pas nadat ze als gebruikers zijn toegevoegd aan [!UICONTROL product profile] `Campaign-xxx-Administrators/Admin`

**Oplossing:**
De beheerder moet de gebruiker toevoegen aan het [!UICONTROL product profile] *[!DNL Campaign-xxx-Admins]* voor elke instantie die de gebruiker wil beheren. Als de gebruiker een beheerder van alle instanties is, moet hij of zij zichzelf mogelijk toch nog toevoegen als *[!UICONTROL user]*.

### Probleem: Een instantie wordt niet vermeld in het [!UICONTROL Control Panel]

**Oorzaak:**
Waarschijnlijk moet de gebruiker worden toegevoegd als een *[!UICONTROL user]* Productprofiel`Campaign-xxx-Administrators/Admin` voor de instantie die ontbreekt

**Oplossing:**
De beheerder moet de gebruiker toevoegen aan het Productprofiel `Campaign-xxx-Admins` voor elke instantie die de gebruiker wil beheren. Als de gebruiker een beheerder van alle instanties is, moet hij of zij zichzelf mogelijk toch nog toevoegen als *[!UICONTROL user]*.

### Nuttige video’s

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)

*[!DNL IMS Org ID] controleren (00:26 min)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)

*Een beheerder toevoegen aan het [!UICONTROL product profile] [!DNL administrators] om het [!UICONTROL Control Panel] te kunnen gebruiken (01:03 min)*

### Handige documentatie

* [Het [!UICONTROL Control Panel] ontdekken](https://helpx.adobe.com/nl/campaign/kb/control-panel-overview.html)
* [Toestemmingen beheren voor het [!UICONTROL Control Panel]](https://helpx.adobe.com/nl/campaign/kb/control-panel-access.html)

## Verbinding met SFTP-server tot stand brengen (client of API)

Voor verbinding met SFTP-servers is het volgende vereist:

* [!UICONTROL allow listing] het IP-adres waarvan u verbinding maakt met de SFTP-server
* Privé/openbaar sleutelpaar dat bij Adobe Campaign moet worden geregistreerd
* Als u rechtstreeks verbinding maakt met de SFTP-server, hebt u ook SFTP-clientsoftware nodig

### Handige documentatie  {#helpful-docs}

* [Aanmelden bij uw SFTP-server](https://docs.adobe.com/content/help/nl-NL/control-panel/using/control-panel-home.html#LoggingintoyourSFTPserver)

