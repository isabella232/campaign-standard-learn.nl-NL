---
title: Problemen met het openen van het regelpaneel
description: Met het Configuratiescherm kunt u uw SFTP-opslag op instantie en IP-adressen van lijsten van gewenste personen controleren en beheren.
feature: Control Panel
topics: null
kt: 2938
doc-type: article
activity: use
team: PM
translation-type: tm+mt
source-git-commit: 2f0527f3d9e2248eea68079e00855cce7a96fce4
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 1%

---


# Probleemoplossing voor het [!UICONTROL-configuratiescherm]

Leer hoe u problemen kunt oplossen wanneer u het Configuratiescherm gebruikt.

## Aanmelding en homepage

Problemen met aanmelding en homepage.

### Symptoom: Aanmelden bij Adobe Experience Cloud is niet mogelijk

**Wat moet u doen:**
De gebruiker moet hun [!DNL IMS Org ID] (xxx) vinden. De beheerder moet de gebruiker aan [!UICONTROL product profile] [!DNL “Campaign-xxx-Admins”] voor elke instantie toevoegen die zij zouden willen beheren. Als de gebruiker een beheerder van alle instanties is zouden zij nog kunnen moeten toevoegen als *[!UICONTROL user]*.

### Symptoom: Koppelingen in het [!UICONTROL Adobe Experience Cloud Home] toegangspunt [!UICONTROL Control Panel] worden niet weergegeven voor een gebruiker

**Oorzaak:**
Gebruikers zien de koppelingen pas nadat ze als gebruikers zijn toegevoegd aan [!UICONTROL product profile] `Campaign-xxx-Administrators/Admin`

**Wat moet u doen:**
De beheerder moet de gebruiker aan [!UICONTROL product profile] *[!DNL Campaign-xxx-Admins]* voor elke instantie toevoegen die zij zouden willen beheren. Als de gebruiker een beheerder van alle instanties is zouden zij nog kunnen moeten toevoegen als *[!UICONTROL user]*.

### Symptoom: Een instantie wordt niet vermeld in het dialoogvenster [!UICONTROL Control Panel]

**Oorzaak:**
De meest waarschijnlijke gebruiker moet worden toegevoegd als een *[!UICONTROL user]* productprofiel `!DNL Campaign-xxx-Administrators/Admin` voor de instantie die ontbreekt

**Wat moet u doen:**
De beheerder moet de gebruiker aan het Profiel van het Product `Campaign-xxx-Admins` voor elke instantie toevoegen die zij willen beheren. Als de gebruiker een beheerder van alle instanties is zouden zij nog kunnen moeten toevoegen als *[!UICONTROL user]*.

### Nuttige video&#39;s

>[!VIDEO](https://video.tv.adobe.com/v/27183?quality=12)
*Controle[!DNL IMS Org ID](00:26 min)*

>[!VIDEO](https://video.tv.adobe.com/v/27147?quality=12)
*Hoe te om een beheerder aan toe te voegen[!UICONTROL product profile]om te kunnen gebruiken *[!DNL administrators]*[!UICONTROL Control Panel](01:03 min)*

### Nuttige documentatie

* [Ontdek de [!UICONTROL Control Panel]](https://helpx.adobe.com/campaign/kb/control-panel-overview.html)
* [Machtigingen beheren voor de [!UICONTROL Control Panel]](https://helpx.adobe.com/campaign/kb/control-panel-access.html)

## Verbinding met SFTP-server tot stand brengen (client of API)

Voor verbinding met SFTP-servers is het volgende vereist:

* [!UICONTROL allow listing] het IP-adres waarvan u verbinding maakt met de SFTP-server
* Persoonlijk/openbaar sleutelpaar dat bij Adobe Campaign moet worden geregistreerd
* Als u rechtstreeks verbinding maakt met de SFTP-server, hebt u ook SFTP-clientsoftware nodig

### Nuttige documentatie

* [Aanmelden bij uw SFTP-server](https://helpx.adobe.com/campaign/kb/control-panel-sftp.html#LoggingintoyourSFTPserver)

