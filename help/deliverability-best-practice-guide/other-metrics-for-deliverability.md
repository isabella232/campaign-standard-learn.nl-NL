---
title: Andere maatstaven die van belang zijn voor de leverbaarheid
description: Één van de beste manieren om een verzendende reputatie te identificeren is door de metriek. Laten we eens kijken naar enkele belangrijke resultaten die u kunt controleren en hoe u deze kunt gebruiken om een reputatie-probleem te identificeren.
feature: null
topics: Deliverability
kt: 5256
doc-type: article
activity: understand
team: TM
translation-type: tm+mt
source-git-commit: 7aa32d583ac2ea756945a17634fb477d7b94cb7f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Andere maatstaven die van belang zijn voor de leverbaarheid

Één van de beste manieren om een verzendende reputatie te identificeren is door de metriek. Laten we eens kijken naar enkele belangrijke resultaten die u kunt controleren en hoe u deze kunt gebruiken om een reputatie-probleem te identificeren.

## Bounces

De grenzen zijn het resultaat van een leveringspoging en mislukking waar ISP achtermislukkingsberichten verstrekt. De verwerking van de stuitbehandeling is een kritiek deel van lijsthygiëne. Nadat een bepaalde e-mail meerdere keren achter elkaar is teruggestuurd, wordt deze tijdens dit proces gemarkeerd voor onderdrukking. Het aantal en het type van grenzen die worden vereist om onderdrukking teweeg te brengen variëren van systeem tot systeem. Hierdoor wordt voorkomen dat systemen ongeldige e-mailadressen blijven verzenden. De grenzen zijn één van de belangrijkste stukken van gegevens die ISPs gebruikt om IP reputatie te bepalen. Het is heel belangrijk om deze maatstaf in de gaten te houden. &quot;Geleverd&quot; versus &quot;teruggestort&quot; is waarschijnlijk de meest gebruikelijke manier om de levering van marketingberichten te meten: hoe hoger het geleverde percentage is , hoe beter . We graven in twee verschillende soorten golven.

## Harde vlekken

De harde stegels zijn permanente mislukkingen die worden geproduceerd nadat ISP een postingspoging aan een abonneeadres als niet te leveren niet bepaalt. In Adobe Campaign worden harde golven die als niet-leverbaar zijn gecategoriseerd, aan de quarantaine toegevoegd, wat betekent dat ze niet opnieuw zouden worden geplaatst. In sommige gevallen wordt een harde stuit genegeerd als de oorzaak van de mislukking onbekend is. Hier volgen enkele voorbeelden van harde grenzen:

* Adres bestaat niet
* Account uitgeschakeld
* Ongeldige syntaxis
* Ongeldig domein

## Zachte golven

De zachte grenzen zijn tijdelijke mislukkingen die ISPs produceert wanneer zij moeilijkheden hebben leverend post. Zachte mislukkingen zullen veelvoudige tijden (met variantie afhankelijk van gebruik van douane of uit-van-doos Adobe Campaign leveringsmontages) opnieuw proberen om een succesvolle levering te proberen. Adressen dat voortdurend zachte stuit niet aan quarantaine zal worden toegevoegd tot het maximumaantal herpogingen is geprobeerd (die opnieuw afhankelijk van montages) variëren. Tot de meest voorkomende oorzaken van zachte grenzen behoren:

* Postbus vol
* E-mailserver ontvangen
* Problemen met reputatie van afzender

![stuitertypen](assets/bounce-types.png)

>[!NOTE]
>
>De stuiteringen zijn een zeer belangrijke indicator van een reputatie kwestie omdat zij een slechte gegevensbron (harde stuit) of een reputatie kwestie met ISP (zachte stuit) kunnen benadrukken.
Zachte grenzen treden vaak op als onderdeel van het verzenden van e-mail en moeten tijdens de hertestverwerking kunnen worden opgelost voordat ze worden gekarakteriseerd als een probleem dat werkelijk te leveren is. Als uw soft bounce tarief voor één enkele ISP groter is dan 30 percenten en niet binnen 24 uren oplost, is het een goed idee om een zorg met uw adviseur van de Leesbaarheid van Adobe Campaign te verhogen.

## Klachten

Klachten worden geregistreerd wanneer een gebruiker aangeeft dat een e-mailbericht ongewenst of onverwacht is. Deze abonneeactie wordt typisch het programma geopend door of de e-mailcliënt van de abonnee wanneer zij de spamknoop of via een derdespam rapporterend systeem raken.

### ISP-klacht

De meeste Rij 1 en sommige Rij 2 ISPs verstrekken een spam meldend methode aan hun gebruikers aangezien opt-out en unsubscribe processen in het verleden maliciously zijn gebruikt om een e-mailadres te bevestigen. Adobe Campaign ontvangt deze klachten via ISP FBL&#39;s. Dit wordt gevestigd tijdens het opstellingsproces voor om het even welke ISPs die FBLs verstrekken en staat Adobe Campaign toe om e-mailadressen automatisch toe te voegen die aan de quarantainetabel voor onderdrukking klaagden. De pieken in ISP klachten kunnen een indicator van slechte lijstkwaliteit, minder-dan-optimale methodes van de lijstinzameling, of zwak betrokkenheidsbeleid zijn. Ze worden ook vaak vermeld wanneer de inhoud niet relevant is.

### Klachten van derden

Er zijn verscheidene anti-spamgroepen die voor spamrapportering op een breder niveau toestaan. De gegevens van de klacht die door deze derden worden gebruikt worden gebruikt om e-mailinhoud te etiketteren om spame-mail te identificeren. Dit proces wordt ook wel vingerafdrukken genoemd. Gebruikers van deze methoden voor klachten van derden zijn over het algemeen zuiniger over e-mail, zodat zij een grotere impact kunnen hebben dan andere klachten kunnen hebben als zij niet worden beantwoord.

>[!NOTE]
>
>ISPs verzamelt klachten en gebruikt hen om de algemene reputatie van een afzender te bepalen. Alle klachten moeten worden onderdrukt en niet langer zo snel mogelijk worden benaderd, overeenkomstig de plaatselijke wetten en voorschriften.

## Spam-overvullingen

Een spamval is een adres dat wordt gebruikt om een ongeoorloofde of ongevraagde e-mail te identificeren. Er zijn spamovervullingen om te helpen bij het identificeren van e-mail van frauduleuze afzenders of van personen die de beste praktijken in e-mail niet volgen. Het e-mailadres van de spamtrap is over het algemeen niet openbaar gepubliceerd en is bijna onmogelijk te identificeren. Het leveren van e-mail aan spamvallen kan uw reputatie met variërende graden van strengheid afhankelijk van het type van val en ISP beïnvloeden. Meer informatie over de verschillende typen spamvallen vindt u in de volgende secties.

### Gerecycled

Gerecyclede spamvallen zijn adressen die ooit geldig waren maar niet meer worden gebruikt. Een belangrijke manier om lijsten zo schoon mogelijk te houden, is om regelmatig e-mail naar uw volledige lijst te sturen en de teruggestuurde e-mails op de juiste manier te onderdrukken. Hierdoor kunnen verlaten e-mailadressen in quarantaine worden geplaatst en niet meer worden gebruikt.

In sommige gevallen kan een adres binnen 30 dagen worden gerecycleerd. Regelmatig verzenden is een essentieel aspect van een goede hygiëne van de lijsten en het regelmatig onderdrukken van inactieve gebruikers. Regeneratiecampagnes maken doorgaans deel uit van geavanceerde e-mailmarketingprogramma&#39;s. Met deze campagnestijl kan de afzender proberen gebruikers terug te winnen die anders niet meer via e-mail zouden worden verzonden.

### Typo

Een spamval voor typefamilies is een adres dat een spelfout of misvorming bevat. Dit gebeurt vaak met bekende spelfouten in belangrijke domeinen zoals [!DNL Gmail] (bijvoorbeeld: [!DNL gmail] is een algemene typefout). ISPs en andere blok-lijst exploitanten zullen bekende slechte domeinen registreren die als spamtrap moeten worden gebruikt om spammers te identificeren en afzendergezondheid te meten. De beste manier om typefamilie te verhinderen vallen is een dubbel opt-in proces voor lijstinzameling te gebruiken.

### Pristine

Een ongerepte spamval is een adres dat geen eindgebruiker heeft en nog nooit een eindgebruiker heeft gehad. Dit is een adres dat is gemaakt om spamemail te identificeren. Dit is het meest onheilspellende type spamval omdat het vrijwel onmogelijk is om te identificeren en een aanzienlijke inspanning zou vergen om van uw lijst schoon te maken. De meeste zwarte lijsten gebruiken ongerepte spamvallen om onbetrouwbare afzenders op te nemen. De enige manier om ongerepte spamvallen te voorkomen dat uw bredere e-maillijst voor marketing wordt geïnfecteerd, is door een dubbel aanmeldingsproces te gebruiken voor het verzamelen van lijsten.

## Opsomming

Opsommend is de levering van post in spam of junk omslag van ISP. Het is herkenbaar wanneer een lage-dan-normale open tarief (en soms kliktarief) met een hoge geleverde tarief wordt gecombineerd. De oorzaken waarom e-mails worden gepeld variëren per ISP. In het algemeen geldt echter dat als berichten in de bulkmap worden geplaatst, een vlag die van invloed is op het verzenden van reputatie (bijvoorbeeld hygiëne van lijsten) opnieuw moet worden geëvalueerd. Het is een signaal dat de reputatie afneemt. Dit is een probleem dat onmiddellijk moet worden verholpen voordat het verdere campagnes beïnvloedt. Werk samen met uw Adobe Campaign-consultant voor de leveringsmogelijkheden om eventuele bulkproblemen op te lossen, afhankelijk van uw situatie.

## Blokkeren

Een blok komt voor wanneer de spamindicatoren merkgebonden ISP drempels bereiken en ISP begint post (merkbaar door het bellen pogingen) van een afzender te blokkeren. Er zijn verschillende typen blokken. Over het algemeen, komen de blokken specifiek voor een IP adres voor, maar zij kunnen ook op het verzendende domein of entiteitniveau voorkomen. Voor het oplossen van een blok is specifieke expertise vereist. Neem daarom contact op met uw Adobe Campaign-consultant voor te bereiden voor hulp.

## Blackvermelding

Een zwarte lijst wordt weergegeven wanneer een externe blacklist-manager spammergedrag registreert dat bij een afzender hoort. De oorzaak van een zwarte lijst wordt soms gepubliceerd door de zwarte lijst. Een lijst is over het algemeen gebaseerd op IP adres, maar in ernstigere gevallen kan het door IP waaier of zelfs een verzendend domein zijn. Als je een zwarte lijst oplost, moet je hiervoor ondersteuning vragen van je Adobe Campaign-consultant, zodat je aanbiedingen volledig kunt oplossen en voorkomen. Sommige aanbiedingen zijn extreem ernstig en kunnen langdurige problemen met de reputatie veroorzaken die moeilijk te verhelpen zijn. Het resultaat van een zwarte lijst varieert per zwarte lijst, maar kan de levering van alle e-mail beïnvloeden.

## Aanvullende resources

* [Typen leveringsfouten en redenen](https://docs.adobe.com/content/help/en/campaign-standard/using/testing-and-sending/monitoring-messages/understanding-delivery-failures.html#delivery-failure-types-and-reasons)
