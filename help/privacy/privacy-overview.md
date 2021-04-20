---
title: Verzoeken om toegang tot persoonsgegevens via Adobe Campaign Standard (ACS) - overzicht
description: In de tutorial wordt uitgelegd hoe u verzoeken om toegang tot persoonsgegevens maakt via de interface van Adobe Campaign Standard (ACS).
feature: GDPR, CCAP
topic: Privacy
kt: 1480
doc-type: feature video
activity: use
team: TM
translation-type: ht
source-git-commit: 556bff4c94e16d3a94561dee1ccb311bc003b631
workflow-type: ht
source-wordcount: '371'
ht-degree: 100%

---


# Verzoeken om toegang tot persoonsgegevens via de gebruikersinterface van Adobe Campaign Standard

Adobe Campaign biedt gegevenscontrollers drie manieren voor het verwerken van verzoeken om toegang tot persoonsgegevens of verzoeken om persoonsgegevens te verwijderen, in overeenstemming met privacywetgeving zoals de AVG (Algemene verordening gegevensbescherming) en de CCPA (California Consumer Privacy Act):

* **Via de integratie met de Privacy-kernservice:** verzoeken om toegang tot persoonsgegevens die van [!UICONTROL Privacy Service] naar alle Experience Cloud-oplossingen worden gestuurd, worden door Campaign automatisch afgehandeld via een speciale workflow. Raadpleeg de [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html) om te ontdekken hoe u verzoeken om toegang tot persoonsgegevens kunt maken vanuit de Privacy-kernservice

* **Via de API:** Adobe Campaign beschikt over een REST-API die verzoeken om toegang tot persoonsgegevens automatiseert

* **Via de Adobe Campaign-interface:** voor elk verzoek om toegang tot persoonsgegevens maakt de gegevenscontroller een nieuw dergelijk verzoek in Adobe Campaign

>[!NOTE]
>
> **WIJZIGINGEN MET ACS 19.4:**
> 
> De [Privacy Service-integratie](https://adobe.io/apis/cloudplatform/gdpr.html) is de methode die u moet gebruiken voor alle toegangs- en verwijderingsverzoeken. Met ingang van versie 19.4 is het gebruik van de Campaign-API en -interface voor toegangs- en verwijderingsverzoeken afgeschaft. Raadpleeg [deze pagina](https://helpx.adobe.com/nl/campaign/kb/acs-deprecated-and-removed-features.html) voor meer informatie over Campaign Standard-functies die zijn afgeschaft en verwijderd.
>
>**Opt-out voor de verkoop van persoonlijke gegevens (CCPA)**
>
>Vanaf versie 19.4 wordt een gebruiksklaar CCPA-veld voor afmelden meegeleverd in de interface en API van Campaign. Als u deze informatie in versie 19.3 wilt gebruiken, moet u dit veld in Adobe Campaign Standard maken. Raadpleeg de [gedetailleerde documentatie](https://helpx.adobe.com/nl/campaign/kb/acs-privacy.html#ccpa) voor meer informatie.
>
> U kunt uw versie controleren door te klikken op het pictogram ? in de rechterbovenhoek van de interface en Info te selecteren.

## Videotutorials

### Vereisten voor verzoeken om toegang tot persoonsgegevens

1. [Een naamruimte maken](/help/privacy/namespaces-for-privacy-requests.md)
1. [Aangepaste bronnen wijzigen](/help/privacy/custom-resources-for-privacy-requests.md)

### Verzoeken om toegang tot persoonsgegevens maken, bijhouden en uitvoeren via de Adobe Campaign-gebruikersinterface

* [Verzoeken om toegang tot persoonsgegevens maken en bijhouden via de Adobe Campaign-gebruikersinterface](/help/privacy/create-and-track-privacy-requests.md)
* [Verzoeken om toegang tot persoonsgegevens uitvoeren](/help/privacy/execute-privacy-requests.md)

## Aanvullende bronnen

* [Algemene richtlijnen op het gebied van privacy voor Campaign](https://helpx.adobe.com/nl/campaign/kb/campaign-privacy-overview.html)
* [CCPA voor ACS](https://helpx.adobe.com/nl/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Documentatie voor de REST-API van Adobe Campaign Standard](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
