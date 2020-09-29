---
title: Overgangsproces - Overschakelen van e-mailplatforms
description: 'Bij het verplaatsen van e-mailserviceproviders (ESP''s) is het niet mogelijk om ook een overgang te maken naar uw bestaande, gevestigde IP-adressen. Het is belangrijk dat u de beste praktijken volgt voor het ontwikkelen van een positieve reputatie wanneer u opnieuw begint. Omdat de nieuwe IP adressen u nog zal gebruiken geen reputatie hebben, kan ISPs niet volledig de post vertrouwen die uit hen komt en moet voorzichtig zijn in wat zij toestaan om aan hun klanten worden geleverd. '
feature: null
topics: Deliverability
kt: null
doc-type: article
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: f4dbccc1fea3db4dbddec0d4329b359993b62d20
workflow-type: tm+mt
source-wordcount: '1686'
ht-degree: 0%

---


# Overgangsproces - Overschakelen van e-mailplatforms

Bij het verplaatsen van e-mailserviceproviders (ESP&#39;s) is het niet mogelijk om ook een overgang te maken naar uw bestaande, gevestigde IP-adressen. Het is belangrijk dat u de beste praktijken volgt voor het ontwikkelen van een positieve reputatie wanneer u opnieuw begint. Omdat de nieuwe IP adressen u nog zal gebruiken geen reputatie hebben, kan ISPs niet volledig de post vertrouwen die uit hen komt en moet voorzichtig zijn in wat zij toestaan om aan hun klanten worden geleverd.

Denk na over wat u doet wanneer u iemand nieuw ontmoet. Doorgaans moet u vertrouwen opbouwen in plaats van ze meteen te vertrouwen. Denk niet dat uw merk automatisch zal helpen met dat vertrouwen, omdat spammers uw naam zullen gebruiken om slechte dingen te doen. ISPs moet uw verzendende praktijken herschatten, aangezien de actie het meest in e-mailleverbaarheid het vertellen is.

Het vestigen van een positieve reputatie is een proces. Maar als deze eenmaal is vastgesteld, zullen kleine negatieve indicatoren minder effect hebben op u en uw postbestelling.

![Het overgangsproces](assets/transition-process.png)

De hoeveelheid tijd om uw IP adressen en domeinen op te warmen kan variëren, maar tot een 8 weken benchmark is gemeenschappelijk voor typische afzenders om een reputatie bij meeste Rij 1 ISPs ([!DNL Gmail], [!DNL Microsoft], [!DNL Verizon]/[!DNL Yahoo]/[!DNL AOL], enz.) te vestigen.
In de volgende secties onderzoeken we enkele belangrijke gebieden waarop de aandacht op de juiste wijze aan boord moet worden gericht.

## Infrastructuur

Succesvolle prestaties zijn afhankelijk van een sterke basis. E-mailinfrastructuur is een kernelement. Een goed geconstrueerde e-mailinfrastructuur omvat meerdere componenten, namelijk domein(en) en IP-adres(sen). Deze onderdelen zijn vergelijkbaar met de machines achter de e-mails die u verzendt. Vaak vormen ze het anker van het verzenden van reputatie. Consultants voor de aflevering zorgen ervoor dat deze elementen tijdens de implementatie op de juiste wijze worden ingesteld, maar vanwege het faam-element is het belangrijk dat u over deze basiskennis beschikt.

### Instellen en strategie van domeinen

De tijden zijn veranderd, en sommige ISPs (als [!DNL Gmail] en [!DNL Yahoo]) neemt domeinreputatie nu als extra punt op wanneer het aangaat om het vastmaken van e-mailreputatie aan een afzender. Uw domeinreputatie is gebaseerd op uw verzendend domein in plaats van uw IP adres. Dit betekent dat uw merk belangrijkheid neemt wanneer het over ISP het filtreren besluiten komt.

Een deel van het instapproces voor nieuwe afzenders op Adobe Campaign omvat het opzetten van uw verzendende domeinen en het controleren of uw infrastructuur correct is geïnstalleerd. U zou met een deskundige moeten werken op welke domeinen u op lange termijn van plan bent te gebruiken. Hier volgen enkele tips die een goede domeinstrategie vormen:

* Maak het merk zo duidelijk en reflecterend mogelijk met het domein dat u kiest, zodat gebruikers de post niet verkeerd als spam herkennen. Sommige voorbeelden zijn [!DNL newsletter.foo.com], [!DNL receipts.foo.com]enzovoort.
* U moet uw bovenliggende domein of bedrijfsdomein niet gebruiken omdat dit van invloed kan zijn op de verzending van e-mail van uw organisatie naar ISP&#39;s.
* U kunt overwegen een subdomein van het bovenliggende domein te gebruiken om het verzendende domein te legitimeren.
* Scheid uw subdomeinen voor transactie en marketing berichtcategorieën. Dit zal uw e-mailverkeer op een betrouwbaardere basis helpen stromen aangezien ISPs deze verzendende methode zoekt, die een bekende e-mailbeste praktijk is en hoogst geadviseerd.

### IP-strategie

Het is belangrijk om een goed gestructureerde IP strategie te vormen helpen een positieve reputatie vestigen. Het aantal IPs en de opstelling varieert afhankelijk van uw bedrijfsmodel en marketing doelstellingen. Werk samen met een deskundige om een duidelijke strategie te ontwikkelen om van rechts te beginnen. Houd rekening met het volgende:

* Te veel IPs kan reputatiekwesties teweegbrengen aangezien het een gemeenschappelijke tactiek van spammers aan sneeuwschoen is, die een tactiek is door spammers wordt gebruikt waar het verkeer over vele IPs wordt verspreid om de levering van spampost te maximaliseren. Hoewel u geen spammer bent, zou u als één kunnen kijken als u teveel IPs gebruikt, vooral als die IPs geen vroeger verkeer heeft gehad.
* Te weinig IPs kan productiekwesties veroorzaken en potentieel reputatiekwesties teweegbrengen. De productie varieert door ISP. Hoeveel en hoe snel ISP bereid is om te aanvaarden is typisch gebaseerd op hun infrastructuur en het verzenden van reputatiedrempels.
* Het scheiden van verkeer voor overseinentypen is zeer belangrijk. Het is belangrijk om, op een minimum te houden, afzonderlijke marketing en transactionele post op afzonderlijke IP pools.
* Afhankelijk van uw poststrategie, kan het ook raadzaam zijn om verschillende producten of marketing stromen op verschillende IP pools te scheiden als uw reputatie drastisch verschillend is. Sommige markten segmenteren ook per regio. Het scheiden van IP voor verkeer met een lagere reputatie zal niet de reputatie kwestie oplossen, maar het zal kwesties met uw &quot;goede&quot;reputatie e-mailleveringen verhinderen. U wilt uw goede publiek immers niet opofferen voor een riskantere doelgroep.

### Feedbackloops

Achter de schermen verwerkt Adobe Campaign gegevens over stormen, klachten, afmelden en nog veel meer. De opstelling van deze terugkoppelt lijnen is een belangrijk aspect aan leverbaarheid. Klachten kunnen een reputatie schaden, dus u moet e-mailadressen verwijderen die klachten registreren bij uw doelgroep. Het is belangrijk om op te merken dat deze gegevens [!DNL Gmail] niet worden teruggestuurd. De lijst unsubscribe kopballen en overeenkomst het filtreren zijn vooral belangrijk voor [!DNL Gmail] abonnees, die nu de meerderheid van abonneegegevensbestanden vormen.

### Verificatie

De authentificatie is het proces dat ISPs gebruikt om de identiteit van een afzender te bevestigen. De twee gemeenschappelijkste authentificatieprotocollen zijn [!DNL Sender Policy Framework (SPF)] en [!DNL DomainKeys Identified Mail] (DKIM). Deze zijn niet zichtbaar aan het eind - gebruiker maar helpen ISPs filtere-mail van geverifieerde afzenders. [!DNL Domain-based Message Authentication Reporting and Conformance] (DMARC) wint populariteit, hoewel zijn beleid nog niet door alle ISP&#39;s in hun reputatie wordt opgenomen.

#### **SPF**

[!DNL Sender Policy Framework (SPF)] is een authentificatiemethode die de eigenaar van een domein toestaat om te specificeren welke postservers zij gebruiken om post van dat domein te verzenden.

#### **DKIM**

[!DNL Domain Keys Identified Mail (DKIM)] is een authentificatiemethode die wordt gebruikt om vervalste afzenderadressen (algemeen genoemd [!DNL spoofing]) te ontdekken. Als DKIM wordt toegelaten, staat het de ontvanger toe om te bevestigen of de afzender gemachtigd is om post van dat domein te verzenden.

#### **DMARC**

[!DNL Domain-based Message Authentication, Reporting and Conformance (DMARC)] is een authentificatiemethode die domeineigenaars de capaciteit geeft om hun domein tegen onbevoegd gebruik te beschermen. DMARC gebruikt SPF of DKIM of allebei om een domeineigenaar toe te staan om te controleren wat met post gebeurt die authentificatie ontbreekt: geleverd, in quarantaine geplaatst of geweigerd.

## Doelcriteria

Wanneer het verzenden van nieuw verkeer, slechts richt uw hoogst betrokken gebruikers tijdens de vroege fasen van IP opwarming. Dit helpt een positieve reputatie van get-go te vestigen om vertrouwen effectief te bouwen alvorens in uw minder betrokken publiek te rollen. Hier volgt een basisformule voor betrokkenheid:

![Formule voor milieubeheer](assets/formula-for-enagement.png)

Doorgaans is een betrokkenheidspercentage gebaseerd op een specifieke periode. Deze metrische waarde kan drastisch variëren afhankelijk van als de formule op algemeen niveau of voor specifieke postingstypes of campagnes wordt toegepast. De specifieke het richten criteria moeten worden verstrekt door met uw de leveringsconsultant van Adobe Campaign te werken, aangezien elke afzender en ISP varieert en gewoonlijk een aangepast plan vereist.

## ISP-specifieke overwegingen tijdens IP-opwarming

ISPs heeft verschillende regels en verschillende manieren om hun verkeer te bekijken. Bijvoorbeeld, [!DNL Gmail] is één van de meest verfijnde ISPs omdat zij betrokkenheid zeer strikt (opent en klikt) naast alle andere reputatiemaatregelen bekijken. Dit vereist een aangepast plan dat slechts op de hoogste betrokken gebruikers bij de aanvang richt. Andere ISPs kan het zelfde ook vereisen. Werk voor een specifiek plan samen met uw Adobe Campaign-consultant voor leveringsmogelijkheden.

## Volume

Het volume van de post u verzendt is kritiek om een positieve reputatie te vestigen. Zet jezelf in de schoenen van een internetprovider — als je een ton verkeer ziet van iemand die je niet kent, zou dat alarmerend zijn. Het direct verzenden van grote hoeveelheden post is riskant en zeker om reputatie kwesties te veroorzaken die vaak moeilijk zijn op te lossen. Het kan frustrerend, tijdrovend en kostbaar zijn om uzelf uit slechte reputatie te halen en problemen op te lossen die het gevolg zijn van te veel te vroeg verzenden.

De volumedrempels variëren door ISP en kunnen ook afhankelijk van uw gemiddelde betrokkenheidsmetriek variëren. Sommige afzenders hebben een zeer lage en langzame oprijsnelheid nodig, terwijl andere een steile oprijplaat mogelijk maken. We raden u aan samen te werken met een expert, zoals een Adobe Campaign-consultant voor te bereiden op levering, om een aangepast volumeplan te ontwikkelen.

Hier volgt een lijst met tips en tips voor een vloeiende overgang:

* **Toestemming** is de basis van elk succesvol e-mailprogramma.
* **Lage en langzame start** met lage verzendende volumes en vergroot vervolgens naarmate u uw reputatie van de afzender verkrijgt.
* Met een **mailingstrategie** voor gelijktijdige verzending kunt u het volume tijdens de campagne opvoeren zonder dat dit ten koste gaat van uw huidige ESP-systeem.
* **Betrokkenheid** is belangrijk - begin met de abonnees die uw e-mails regelmatig openen en klikken.
* **Volg het plan** — onze aanbevelingen hebben honderden campagneklanten geholpen hun e-mailprogramma&#39;s met succes op te zetten.
* **Controleer uw e-mailaccount**. Het is een slechte ervaring voor uw klant om te gebruiken [!DNL nore-ply@xyz.com] of niet te antwoorden.
* Inactieve adressen kunnen een negatief effect op de leesbaarheid hebben. **Reactiveer en geef opnieuw toestemming** op uw huidige platform, niet uw nieuwe IPs.
* **Domeinen** - gebruik een verzendend domein dat een subdomein is van het werkelijke domein van uw bedrijf. Bijvoorbeeld, als uw bedrijfdomein is [!DNL xyz.com], [!DNL email.xyz.com] verstrekt meer geloofwaardigheid aan ISPs dan [!DNL xyzemail.com]
* **Transparantie** : de registratiegegevens voor uw e-maildomein moeten openbaar zijn en mogen niet privé zijn.

In veel gevallen volgt transactionele post niet de traditionele opwarmingsmethode. Het is duidelijk moeilijk om het volume in transactie-mail te beheren vanwege de aard ervan, aangezien hiervoor doorgaans een gebruikersinteractie nodig is om de e-mailaanraking te activeren. In sommige gevallen, kan de transactionele post eenvoudig zonder een formeel plan worden overgebracht. In andere gevallen, zou het beter kunnen zijn om elk berichttype over tijd over te gaan om het volume langzaam te groeien. U kunt bijvoorbeeld als volgt een overgang maken:

1. Bevestigingen aanschaffen - hoge betrokkenheid over het algemeen
2. Afmelden van winkelwagentje - middelgrote betrokkenheid over het algemeen
3. Welkom-e-mails - hoge betrokkenheid maar kunnen slechte adressen bevatten, afhankelijk van de methoden die u in uw lijst gebruikt
4. E-mails met Win-back - lagere betrokkenheid over het algemeen

## Aanvullende resources

* [Een nieuw platform starten](https://docs.adobe.com/content/help/en/campaign-standard/using/testing-and-sending/managing-deliverability/starting-new-platform.html)
