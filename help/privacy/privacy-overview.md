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
ht-degree: 1%

---


# Privacy-aanvragen met de Adobe Campaign Standard-gebruikersinterface

Adobe Campaign biedt gegevensverwerkingsverantwoordelijken drie methoden voor het uitvoeren van privacytoegang en het verwijderen van aanvragen van PII-gegevens in overeenstemming met privacywetten zoals GDPR (General Data Protection Regulation) en CCPA (California Consumer Privacy Act):

* **Via de integratie met de Privacy Core Service:** De verzoeken van de privacy die van [!UICONTROL Privacy Service] aan alle oplossingen van Experience Cloud worden geduwd worden automatisch behandeld door Campagne via een specifieke werkschema. Raadpleeg de [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html) voor meer informatie over het maken van privacyverzoeken van de Privacy Core Service

* **Via de API:** Adobe Campaign biedt een API die het automatische proces van privacyverzoeken met REST mogelijk maakt

* **Via de Adobe Campaign-interface:** voor elke privacyaanvraag maakt de gegevenscontroller een nieuwe privacyaanvraag in Adobe Campaign

>[!NOTE]
>
> **WIJZIGINGEN MET ACS 19.4:**
> 
> De [Privacy Service integratie](https://adobe.io/apis/cloudplatform/gdpr.html) is de methode u voor alle toegang zou moeten gebruiken en verzoeken schrapt. Vanaf 19.4 is het gebruik van de campagne-API en de interface voor toegangs- en verwijderingsverzoeken afgekeurd. Raadpleeg [deze pagina](https://docs.adobe.com/content/help/nl-NL/campaign-standard/using/release-notes/deprecated-features.html)voor meer informatie over afgekeurde en verwijderde functies van Campaign Standard.
>
>**Opt-out voor de verkoop van persoonlijke gegevens**
>
>Beginnend met 19.4, wordt een uit-weg gebied CCPA verstrekt uit-van-de-doos in de interface van de Campagne en API. Voor 19.3 moet u dit veld in Adobe Campaign Standard maken om deze informatie te kunnen gebruiken. Zie de [gedetailleerde documentatie](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa) voor meer informatie.
>
> U kunt uw versie controleren door op te klikken? in de rechterbovenhoek van de interface en het selecteren van Info.

## Video-Tutorials

### Vereisten voor privacyverzoeken

1. [Een naamruimte maken](/help/privacy/namespaces-for-privacy-requests.md)
1. [Aangepaste bronnen wijzigen](/help/privacy/custom-resources-for-privacy-requests.md)

### Privacy-aanvragen maken, bijhouden en uitvoeren via de Adobe Campaign-gebruikersinterface

* [Privacy-aanvragen maken en bijhouden via de gebruikersinterface van Adobe Campaign](/help/privacy/create-and-track-privacy-requests.md)
* [Privacyverzoeken uitvoeren](/help/privacy/execute-privacy-requests.md)

## Aanvullende bronnen

* [Algemene privacyrichtlijnen voor campagnes](https://helpx.adobe.com/campaign/kb/campaign-privacy-overview.html)
* [CCPA voor ACS](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Documentatie Adobe Campaign Standard REST API](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
