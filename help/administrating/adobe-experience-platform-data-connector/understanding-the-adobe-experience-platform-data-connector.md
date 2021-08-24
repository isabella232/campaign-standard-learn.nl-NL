---
title: Adobe Experience Platform Data Connector begrijpen
description: Adobe Experience Platform Data Connector helpt bestaande klanten hun gegevens op Adobe Experience Platform beschikbaar te maken door XTK-gegevens (gegevens die in Campaign worden opgenomen) toe te wijzen aan XDM-gegevens (Experience Data Model) op Adobe Experience Platform.
feature: Integratie van de People Core-service
kt: 2826
thumbnail: 27304.jpg
doc-type: feature video
activity: understand
team: TM
exl-id: 686961f9-5374-4cc6-8b36-7ee0584ea720
source-git-commit: 344b8d8bb216489db586b030c71fd84d273968d9
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 8%

---

# De Adobe Experience Platform [!UICONTROL Data Connector]

>[!NOTE]
>
>Deze mogelijkheid wordt momenteel in bèta aangeboden en kan zonder voorafgaande kennisgeving regelmatig worden bijgewerkt en gewijzigd.
>
>Neem contact op met [!UICONTROL Adobe Customer Support] als u van plan bent deze functie te implementeren.

## Overzicht

Met Adobe Experience Platform [!UICONTROL Data Connector] kunnen bestaande klanten hun gegevens op Adobe Experience Platform beschikbaar maken door XTK-gegevens (gegevens die in Adobe Campaign worden ingevoerd) toe te wijzen aan [!DNL Experience Data Model] (XDM)-gegevens op Adobe Experience Platform.

De connector is in één richting en verzendt de gegevens van Adobe Campaign Standard naar Adobe Experience Platform. De gegevens worden nooit van de Adobe Experience Platform naar Adobe Campaign Standard verzonden.

Adobe Experience Platform [!UICONTROL Data Connector] is bedoeld voor gegevensengineers die Adobe Campaign Standard [!UICONTROL custom resources] begrijpen en begrijpen hoe het algemene gegevensschema van de klant zich in Adobe Experience Platform moet bevinden.

>[!VIDEO](https://video.tv.adobe.com/v/27304?quality=12)

*Deze video geeft een overzicht over de Adobe Experience Platform  [!UICONTROL Data Connector] (9:35 min)*

>[!NOTE]
>
>De out-of-the-box overdracht van [!UICONTROL subscription events] wordt niet ondersteund. Om [!UICONTROL subscription events] over te brengen, kunt u overeenkomstige XDM en dataset op Adobe Experience Platform tot stand brengen, dan een afbeelding van douanegegevens voor deze gegevens vormen.
>
>Bestaande [!UICONTROL experience events] kan niet in Adobe Experience Platform worden opgenomen, maar doorlopende gegenereerde [!UICONTROL experience events] wordt naar Adobe Experience Platform gestreamd.

## Belangrijke stappen voor het uitvoeren van een gegevenstoewijzing

De volgende zelfstudies beschrijven de belangrijkste stappen voor het uitvoeren van een gegevenstoewijzing tussen Campaign Standard en Adobe Experience Platform:

1. [Aangepaste bronnen toewijzen](/help/administrating/adobe-experience-platform-data-connector/mapping-custom-resources.md)
2. [Experience-gebeurtenissen toewijzen](/help/administrating/adobe-experience-platform-data-connector/mapping-experience-events.md)
3. [Tabelgegevens toewijzen](/help/administrating/adobe-experience-platform-data-connector/mapping-seed-table-data.md)
4. [De gegevenstoewijzing wijzigen](/help/administrating/adobe-experience-platform-data-connector/modifying-data-mapping.md)
5. [De status van taken voor gegevensinvoer controleren](/help/administrating/adobe-experience-platform-data-connector/checking-status-of-data-ingestion-jobs.md)

## Aanvullende bronnen

* [Informatie over de Adobe Experience Platform-gegevensconnector](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-about-data-connector.html)
* [Overzicht van het ervaringsgegevensmodel](https://docs.adobe.com/content/help/en/campaign-standard/using/administrating/mapping-campaign-and-aep-data/aep-data-model-overview.html)
* [Toewijzingsdefinitie](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/adobe-experience-platform/data-connector/aep-mapping-definition.html)
* [Toewijzingsactivering](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/adobe-experience-platform/data-connector/aep-mapping-activation.html)
* [Data-opname via API&#39;s activeren](https://experienceleague.adobe.com/docs/campaign-standard/using/integrating-with-adobe-cloud/adobe-experience-platform/data-connector/aep-triggering-data-ingestion.html)
