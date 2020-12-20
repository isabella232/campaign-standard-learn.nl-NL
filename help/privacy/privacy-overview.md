---
title: Privacy-aanvragen bij de Adobe Campaign Standard (ACS) - Overzicht
description: In de zelfstudie wordt uitgelegd hoe u privacyverzoeken maakt via de interface van Adobe Campaign Standard (ACS).
feature: GDPR, CCAP
topic: Privacy
kt: 1480
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 556bff4c94e16d3a94561dee1ccb311bc003b631
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 20%

---


# Privacy-aanvragen met de Adobe Campaign Standard-gebruikersinterface

Adobe Campaign biedt gegevensverwerkingsverantwoordelijken drie methoden voor het uitvoeren van privacytoegang en het verwijderen van aanvragen van PII-gegevens in overeenstemming met privacywetten zoals GDPR (General Data Protection Regulation) en CCPA (California Consumer Privacy Act):

* **Via de integratie met de Privacy Core Service:** privacyverzoeken die van  [!UICONTROL Privacy Service] naar alle Experience Cloud-oplossingen worden geduwd, worden automatisch door Campagne afgehandeld via een speciale workflow. Raadpleeg [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html) voor meer informatie over het maken van privacyverzoeken van de Privacy Core Service

* **Via de API:** Adobe Campaign beschikt over een API die het automatisch proces van privacyverzoeken met REST mogelijk maakt

* **Via de Adobe Campaign-interface:** voor elke privacyaanvraag maakt de gegevenscontroller een nieuwe privacyaanvraag in Adobe Campaign

>[!NOTE]
>
> **WIJZIGINGEN MET ACS 19.4:**
> 
> De [Privacy Service integratie](https://adobe.io/apis/cloudplatform/gdpr.html) is de methode u voor alle toegang zou moeten gebruiken en verzoeken schrapt. Vanaf 19.4 is het gebruik van de campagne-API en de interface voor toegangs- en verwijderingsverzoeken afgekeurd. Raadpleeg [deze pagina](https://docs.adobe.com/content/help/nl-NL/campaign-standard/using/release-notes/deprecated-features.html) voor meer informatie over afgekeurde en verwijderde functies van Campaign Standard.
>
>**Opt-out voor de verkoop van persoonlijke gegevens (CCPA)**
>
>Vanaf versie 19.4 wordt een gebruiksklaar CCPA-veld voor afmelden meegeleverd in de interface en API van Campaign. Voor 19.3 moet u dit veld in Adobe Campaign Standard maken om deze informatie te kunnen gebruiken. Zie [gedetailleerde documentatie](https://helpx.adobe.com/nl/campaign/kb/acs-privacy.html#ccpa) voor meer informatie.
>
> U kunt uw versie controleren door te klikken op het pictogram ? in de rechterbovenhoek van de interface en Info te selecteren.

## Video-Tutorials

### Vereisten voor privacyverzoeken

1. [Een naamruimte maken](/help/privacy/namespaces-for-privacy-requests.md)
1. [Aangepaste bronnen wijzigen](/help/privacy/custom-resources-for-privacy-requests.md)

### Privacy-aanvragen maken, bijhouden en uitvoeren via de Adobe Campaign-gebruikersinterface

* [Privacy-aanvragen maken en bijhouden via de gebruikersinterface van Adobe Campaign](/help/privacy/create-and-track-privacy-requests.md)
* [Privacyverzoeken uitvoeren](/help/privacy/execute-privacy-requests.md)

## Aanvullende bronnen

* [Algemene richtlijnen op het gebied van privacy voor Campaign](https://helpx.adobe.com/nl/campaign/kb/campaign-privacy-overview.html)
* [CCPA voor ACS](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Documentatie Adobe Campaign Standard REST API](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
