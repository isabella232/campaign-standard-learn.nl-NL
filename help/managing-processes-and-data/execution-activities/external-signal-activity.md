---
title: Externe signaalactiviteit - Een workflow met parameters aanroepen
description: '"Leer hoe te om één werkschema van een andere te beginnen om complexere klantenreizen te steunen, terwijl het kunnen beter controleren en op kwesties reageren."'
feature: Uitvoeringsactiviteit
topics: Workflows
kt: 2750
thumbnail: 27249
doc-type: feature video
activity: use
team: TM
exl-id: d3996185-681c-4906-85f0-0543ab767519
role: Business Practitioner, Developer
level: Experienced
translation-type: tm+mt
source-git-commit: 5d2bc8bd3a3a0fdb5e2f1ef75af2ab60b8f6abc8
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 9%

---

# [!UICONTROL External Signal activity ]- Een workflow met parameters bellen

De [!UICONTROL External Signal activity] wordt gebruikt om verschillende processen te organiseren en te ordenen die deel van de zelfde klantenreis in verschillende werkschema&#39;s uitmaken. Deze activiteit maakt het mogelijk een workflow te starten vanuit een andere workflow ter ondersteuning van complexere klanttrajecten, terwijl u in geval van problemen gemakkelijker kunt opvolgen en reageren.

In ACS 19.2 [!UICONTROL External Signal activity] kan niet alleen een werkschema roepen, maar ook parameters tot het werkschema (een publieksnaam aan doel, een dossier - naam aan invoer, een deel van berichtinhoud, enz.) overgaan vanuit een andere workflow of via een REST API-aanroep om te integreren met uw externe systemen.

Dit omvat ook een nieuwe **Test** Activiteit waar u tests op deze functionaliteit kunt in werking stellen.

In de volgende video worden de vereiste configuratiestappen uitgelegd:

1. **Ontvang externe** parameters van een extern systeem, zoals een systeem van het inhoudsbeheer (CRM):

   * De parameters in de externe signaalactiviteit declareren
   * Configureer de API-aanroep om de parameters te definiëren en de workflow Externe signaalactiviteit te activeren. Voor meer informatie over hoe te om een API vraag te vormen te zien [Triggerend een Activiteit van het Signaal](https://docs.campaign.adobe.com/doc/standard/en/api/ACS_API.html#triggering-a-signal-activity).

1. **Een workflow aanpassen met externe parameters**  (gebeurtenisvariabelen):

   Nadat de workflow is geactiveerd, worden de parameters opgenomen in de gebeurtenisvariabelen van de workflow en kunnen deze binnen de workflow worden gebruikt. Zie de [documentatie](https://helpx.adobe.com/campaign/standard/automating/using/calling-a-workflow-with-external-parameters.html) voor alle activiteiten die met gebeurtenisvariabelen kunnen worden aangepast:

   * De testactiviteit configureren (nieuw in 19.2)
   * Activiteit voor leespubliek en e-maillevering configureren

1. **Vorm een** Activiteit van het Eind om een werkschema met externe parameters te roepen

>[!VIDEO](https://video.tv.adobe.com/v/27249/?quality=12)

## Aanvullende bronnen

* [Extern signaal (documentatie)](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/calling-workflow-external-parameters/calling-a-workflow-with-external-parameters.html)
