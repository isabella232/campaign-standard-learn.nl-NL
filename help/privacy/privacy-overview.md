---
title: Privacy-aanvragen met de Adobe Campagnestandaard (ACS) - Overzicht
description: In de zelfstudie wordt uitgelegd hoe u privacyverzoeken maakt via de interface van Adobe Campagne Standard (ACS).
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
ht-degree: 0%

---


# Privacy-aanvragen met de standaardgebruikersinterface van Adobe Campagne

De Campagne van Adobe biedt gegevenscontrolemechanismen drie methodes om de toegang van de Privacy uit te voeren en verzoeken van PII gegevens te schrappen in overeenstemming met privacywetten zoals GDPR (Algemene Verordening van de Bescherming van Gegevens) en CCPA (de Wet van de Consumentenprivacy van Californië):

* **Via de integratie met de Privacy Core Service:** De privacyverzoeken die van [!UICONTROL Privacy Service] naar alle oplossingen van de Wolk van de Ervaring worden geduwd worden automatisch behandeld door Campagne via een specifieke werkschema. Raadpleeg de [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html) voor meer informatie over het maken van privacyverzoeken van de Privacy Core Service

* **Via de API:** Adobe Campaign biedt een API die het automatische proces van privacyverzoeken met REST mogelijk maakt

* **Via de Adobe Campagne-interface:** voor elke privacyaanvraag maakt de gegevenscontroller een nieuwe privacyaanvraag in Adobe Campagne

>[!NOTE]
>
> **WIJZIGINGEN MET ACS 19.4:**
> 
> De integratie [van de Dienst van de](https://adobe.io/apis/cloudplatform/gdpr.html) Privacy is de methode u voor alle toegang en schrappingsverzoeken zou moeten gebruiken. Vanaf 19.4 is het gebruik van de campagne-API en de interface voor toegangs- en verwijderingsverzoeken afgekeurd. Raadpleeg [deze pagina](https://helpx.adobe.com/campaign/kb/acs-deprecated-and-removed-features.html)voor meer informatie over afgekeurde en verwijderde functies van de campagnestandaard.
>
>**Opt-out voor de verkoop van persoonlijke gegevens**
>
>Beginnend met 19.4, wordt een uit-weg gebied CCPA verstrekt uit-van-de-doos in de interface van de Campagne en API. Voor 19.3 moet u dit veld maken in Adobe Campaign Standard om deze informatie te kunnen gebruiken. Zie de [gedetailleerde documentatie](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa) voor meer informatie.
>
> U kunt uw versie controleren door op te klikken? in de rechterbovenhoek van de interface en het selecteren van Info.

## Videozelfstudies

### Vereisten voor privacyverzoeken

1. [Een naamruimte maken](/help/privacy/namespaces-for-privacy-requests.md)
1. [Aangepaste bronnen wijzigen](/help/privacy/custom-resources-for-privacy-requests.md)

### Privacy-aanvragen maken, bijhouden en uitvoeren via de Adobe Campagne-gebruikersinterface

* [Privacy-aanvragen maken en bijhouden via de gebruikersinterface van Adobe Campagne](/help/privacy/create-and-track-privacy-requests.md)
* [Privacyverzoeken uitvoeren](/help/privacy/execute-privacy-requests.md)

## Aanvullende bronnen

* [Algemene privacyrichtlijnen voor campagnes](https://helpx.adobe.com/campaign/kb/campaign-privacy-overview.html)
* [CCPA voor ACS](https://helpx.adobe.com/campaign/kb/acs-privacy.html#ccpa)
* [Adobe Experience Platform Privacy Service](https://adobe.io/apis/cloudplatform/gdpr.html)
* [Adobe Campagne Standard REST API-documentatie](https://final-docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#privacy-management)
