---
title: Problemen oplossen met het Configuratiescherm
description: Met het Configuratiescherm kunt u uw SFTP-opslag op instantie controleren en beheren en IP-adressen van lijsten van gewenste personen beheren.
feature: Control Panel
kt: 2938
doc-type: article
activity: use
team: PM
recommendations: noDisplay
exl-id: f546f791-a69b-4586-abfa-3e626b8feb17
source-git-commit: 57dbf456625d22cd2e4526d92e5a8c20a048d339
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 47%

---

# Het oplossen van problemen met het [!UICONTROL Control Panel]

Leer hoe u problemen met het gebruik van het Configuratiescherm kunt oplossen.

## Aanmelding en startpagina

Problemen met aanmelding en de startpagina.

### Symptoom: Aanmelden bij Adobe Experience Cloud is mislukt

**Wat moet u doen:**
De gebruiker moet hun [!DNL IMS Org ID] (xxx). De beheerder moet de gebruiker aan de [!UICONTROL product profile] [!DNL “Campaign-xxx-Admins”] voor elke instantie die zij willen beheren. Als de gebruiker een beheerder van alle instanties is, moeten zij toevoegen zoals *[!UICONTROL user]*.

### Probleem: Gebruiker ziet de koppelingen in [!UICONTROL Adobe Experience Cloud Home] voor toegang tot het [!UICONTROL Control Panel] niet

**Oorzaak:**
Gebruikers zien de koppelingen pas nadat ze als gebruikers zijn toegevoegd aan [!UICONTROL product profile] `Campaign-xxx-Administrators/Admin`

**Wat moet u doen:**
De beheerder moet de gebruiker aan de [!UICONTROL product profile] *[!DNL Campaign-xxx-Admins]* voor elke instantie die zij willen beheren. Als de gebruiker een beheerder van alle instanties is, moeten zij toevoegen zoals *[!UICONTROL user]*.

### Symptoom: Een instantie wordt niet vermeld in het [!UICONTROL Control Panel]

**Oorzaak:**
Meest waarschijnlijke gebruiker moet worden toegevoegd als een *[!UICONTROL user]* Productprofiel `Campaign-xxx-Administrators/Admin` voor de instantie die ontbreekt

**Wat moet u doen:**
De beheerder moet de gebruiker toevoegen aan het productprofiel `Campaign-xxx-Admins` voor elke instantie die zij willen beheren. Als de gebruiker een beheerder van alle instanties is, moeten zij toevoegen zoals *[!UICONTROL user]*.

### Nuttige video’s

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)

*[!DNL IMS Org ID] controleren (00:26 min)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)

*Een beheerder toevoegen aan het [!UICONTROL product profile] [!DNL administrators] om het [!UICONTROL Control Panel] te kunnen gebruiken (01:03 min)*

### Handige documentatie

* [Het [!UICONTROL Control Panel] ontdekken](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=nl)
* [Toestemmingen beheren voor het [!UICONTROL Control Panel]](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)

## Verbinding met SFTP-server tot stand brengen (client of API)

Voor verbinding met SFTP-servers is het volgende vereist:

* [!UICONTROL allow listing] het IP-adres waarvan u verbinding maakt met de SFTP-server
* Persoonlijk/openbaar sleutelpaar dat bij Adobe Campaign moet zijn geregistreerd
* Als u rechtstreeks verbinding maakt met de SFTP-server, hebt u SFTP-clientsoftware nodig

### Handige documentatie {#helpful-docs}

* [Aanmelden bij uw SFTP-server](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=en)
