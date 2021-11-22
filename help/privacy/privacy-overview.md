---
title: Verzoeken om toegang tot persoonsgegevens via Adobe Campaign Standard (ACS) - overzicht
description: In de tutorial wordt uitgelegd hoe u verzoeken om toegang tot persoonsgegevens maakt via de interface van Adobe Campaign Standard.
feature: Privacy Tools
kt: 1480
doc-type: feature video
activity: use
team: TM
exl-id: fb766403-694c-4a7b-b3d1-4a418df85891
source-git-commit: 481cbdcc9ac7446cc36fbff6e3d6e43fe333d30b
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 100%

---

# Verzoeken om toegang tot persoonsgegevens via de gebruikersinterface van Adobe Campaign Standard

Adobe Campaign biedt gegevenscontrollers drie manieren voor het verwerken van verzoeken om toegang tot persoonsgegevens of verzoeken om persoonsgegevens te verwijderen, in overeenstemming met privacywetgeving zoals de AVG (Algemene verordening gegevensbescherming) en de CCPA (California Consumer Privacy Act):

* **Via de integratie met de Privacy-kernservice:** verzoeken om toegang tot persoonsgegevens die van [!UICONTROL Privacy Service] naar alle Experience Cloud-oplossingen worden gestuurd, worden door Campaign automatisch afgehandeld via een speciale workflow. Meer informatie over het maken van privacyverzoeken van de Privacy Core Service vindt u in de [Privacy Service in Adobe Experience Platform](https://www.adobe.io/apis/experienceplatform/gdpr.html)

* **Via de API:** Adobe Campaign beschikt over een REST-API die verzoeken om toegang tot persoonsgegevens automatiseert

* **Via de Adobe Campaign-interface:** voor elk verzoek om toegang tot persoonsgegevens maakt de gegevenscontroller een nieuw dergelijk verzoek in Adobe Campaign

>[!NOTE]
>
> **WIJZIGINGEN MET ACS 19.4:**
> 
> De [Privacy Service-integratie](https://www.adobe.io/apis/experienceplatform/gdpr.html) is de methode die u moet gebruiken voor alle toegangs- en verwijderingsverzoeken. Met ingang van versie 19.4 is het gebruik van de Campaign-API en -interface voor toegangs- en verwijderingsverzoeken afgeschaft. Raadpleeg [deze pagina](https://experienceleague.adobe.com/docs/campaign-standard/using/release-notes/deprecated-features.html?lang=nl) voor meer informatie over Campaign Standard-functies die zijn afgeschaft en verwijderd.
>
>**Opt-out voor de verkoop van persoonlijke gegevens (CCPA)**
>
> Er wordt een gebruiksklaar CCPA-veld voor opt-out meegeleverd in de interface en API van Campaign.
>
> U kunt uw versie controleren door op het **?**-pictogram te klikken in de rechterbovenhoek van de interface en Over te selecteren.

## Videotutorials

### Vereisten voor verzoeken om toegang tot persoonsgegevens

1. [Een naamruimte maken](/help/privacy/namespaces-for-privacy-requests.md)
1. [Aangepaste bronnen wijzigen](/help/privacy/custom-resources-for-privacy-requests.md)

### Verzoeken om toegang tot persoonsgegevens maken, bijhouden en uitvoeren via de Adobe Campaign-gebruikersinterface

* [Verzoeken om toegang tot persoonsgegevens maken en bijhouden via de Adobe Campaign-gebruikersinterface](/help/privacy/create-and-track-privacy-requests.md)
* [Verzoeken om toegang tot persoonsgegevens uitvoeren](/help/privacy/execute-privacy-requests.md)

## Aanvullende bronnen

* [Algemene richtlijnen op het gebied van privacy voor Campaign](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-management.html?lang=nl#getting-started)
* [CCPA voor ACS](https://experienceleague.adobe.com/docs/campaign-standard/using/getting-started/privacy/privacy-requests.html?lang=nl#privacy-requests)
* [Adobe Experience Platform Privacy Service](https://www.adobe.io/apis/experienceplatform/gdpr.html)
* [Documentatie voor de REST-API van Adobe Campaign Standard](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
