---
title: Werken met de gegevensconnector van het Adobe Experience Platform
description: Met de Adobe Experience Platform Data Connector kunnen bestaande klanten hun gegevens beschikbaar maken op het Adobe Experience Platform door XTK-gegevens (gegevens die in Campaign worden opgenomen) toe te wijzen aan Experience Data Model (XDM)-gegevens op het Adobe Experience Platform.
feature: Adobe Experience Platform Data Connector
topics: ACoP
kt: 2826
doc-type: feature video
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: cb5d5bc58137fd374eafe165c6ea13288a60d7db
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---


# Werken met het Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Deze mogelijkheid wordt momenteel in bèta aangeboden en kan zonder voorafgaande kennisgeving regelmatig worden bijgewerkt en gewijzigd.
>Neem contact op met [!UICONTROL Adobe Customer Support] als u deze functie wilt implementeren.

## Overzicht

Met het Adobe Experience Platform kunnen bestaande klanten hun gegevens beschikbaar maken op het Adobe Experience Platform door XTK-gegevens (gegevens die in Adobe Campaign worden opgenomen) toe te wijzen aan [!UICONTROL Data Connector] [!DNL Experience Data Model] (XDM) gegevens op het Adobe Experience Platform.

De connector is in één richting en verzendt de gegevens van Adobe Campaign Standard naar Adobe Experience Platform. De gegevens worden nooit van het Adobe Experience Platform naar Adobe Campagne Standard verzonden.

Adobe Experience Platform [!UICONTROL Data Connector] is bedoeld voor gegevensengineers die Adobe Campaign Standard begrijpen [!UICONTROL custom resources] en begrijpen hoe het algemene gegevensschema van de klant zich in het Adobe Experience Platform moet bevinden.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*Deze video geeft een overzicht van het Adobe Experience Platform[!UICONTROL Data Connector](9:35 min)*

>[!NOTE]
>
>De out-of-the-box overdracht van [!UICONTROL subscription events] wordt niet ondersteund. Om over te brengen [!UICONTROL subscription events], kunt u overeenkomstige XDM en dataset op het Platform van de Ervaring van Adobe tot stand brengen, dan een afbeelding van douanegegevens voor deze gegevens vormen.
>Bestaande bestanden [!UICONTROL experience events] kunnen niet worden opgenomen in het Adobe Experience Platform, maar de gegenereerde gegevens [!UICONTROL experience events] worden gestreamd naar het Adobe Experience Platform.

## Belangrijke stappen voor het uitvoeren van een gegevenstoewijzing

In de volgende zelfstudies worden de belangrijkste stappen beschreven voor het uitvoeren van gegevenstoewijzing tussen Campaign Standard en Adobe Experience Platform:

1. [Aangepaste bronnen toewijzen](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Toewijzingsgebeurtenissen](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Tabelgegevens toewijzen](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [De gegevenstoewijzing wijzigen](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [De status van taken voor gegevensinvoer controleren](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Aanvullende bronnen

* [Info over Adobe Experience Platform Data Connector](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-about-data-connector.html)
* [Overzicht van het ervaringsgegevensmodel](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-data-model-overview.html)
* [Toewijzingsdefinitie](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-definition.html)
* [Toewijzingsactivering](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-mapping-activation.html)
* [Gegevensinvoer via API&#39;s activeren](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-triggering-data-ingestion.html)
