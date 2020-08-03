---
title: Externe signaalactiviteit - Een workflow met parameters aanroepen
description: De externe signaalactiviteit wordt gebruikt om verschillende processen te organiseren en te ordenen die deel van de zelfde klantenreis in verschillende werkschema's uitmaken. Het staat toe om één werkschema van een andere te beginnen, toelatend om complexere klantenreizen te steunen, terwijl het kunnen beter controleren en reageren in geval van kwestie.
feature: External Signal Activity
topics: Workflows
kt: 2750
doc-type: feature video
activity: use
team: TM
translation-type: tm+mt
source-git-commit: 9b1d8c5fb895d84da14a0402ec1f130b90a991b0
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---


# [!UICONTROL External Signal activity ]- Een workflow met parameters bellen

Het [!UICONTROL External Signal activity] wordt gebruikt om verschillende processen te organiseren en te ordenen die deel van de zelfde klantenreis in verschillende werkschema&#39;s uitmaken. Het staat toe om één werkschema van een andere te beginnen, toelatend om complexere klantenreizen te steunen, terwijl het kunnen beter controleren en reageren in geval van kwestie.

In ACS 19.2 [!UICONTROL External Signal activity] kan het niet alleen een werkschema roepen, maar ook parameters tot het werkschema overgaan (een publieksnaam aan doel, een dossier - naam om in te voeren, een deel van berichtinhoud, enz.) vanuit een andere workflow of via een REST API-aanroep om te integreren met uw externe systemen.

Dit omvat ook een nieuwe Activiteit van de **Test** waar u tests op deze functionaliteit kunt in werking stellen.

In de volgende video worden de vereiste configuratiestappen uitgelegd:

1. **Ontvang externe parameters** van een extern systeem, zoals een systeem van het inhoudsbeheer (CRM):
   * De parameters in de externe signaalactiviteit declareren
   * Configureer de API-aanroep om de parameters te definiëren en de workflow Externe signaalactiviteit te activeren. Voor meer informatie over hoe te om een API vraag te vormen gelieve te zien het [Teweegbrengen van een Activiteit](https://docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#triggering-a-signal-activity)van het Signaal.

1. **Een workflow aanpassen met externe parameters** (gebeurtenisvariabelen):
Nadat de workflow is geactiveerd, worden de parameters opgenomen in de gebeurtenisvariabelen van de workflow en kunnen deze binnen de workflow worden gebruikt. Zie de [documentatie](https://helpx.adobe.com/campaign/standard/automating/using/calling-a-workflow-with-external-parameters.html) voor alle activiteiten die met gebeurtenisvariabelen kunnen worden aangepast:

   * De testactiviteit configureren (nieuw in 19.2)
   * Activiteit voor leespubliek en e-maillevering configureren

1. **Vorm een Activiteit** van het Eind om een werkschema met externe parameters te roepen

>[!VIDEO](https://video.tv.adobe.com/v/27249/?quality=12)

## Aanvullende bronnen

* [Extern signaal (documentatie)](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/data-management-activities/external-api.html)
