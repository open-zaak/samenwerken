---
layout: default
---
# Samenwerken aan Open Zaak

*OpenZaak is productiewaardig API platform die de API standaard voor zaakgericht werken implementeert (de ZGW-API’s). Met OpenZaak wordt het voor gemeenten mogelijk om veilige en betrouwbare diensten aan te kunnen bieden aan haar inwoners en bedrijven. Omdat OpenZaak gebruik maakt van de Zaakgerichtwerken standaard wordt het uitwisselen van gegevens met andere gemeenten en/of applicaties eenvoudiger en veiliger. OpenZaak is open source software. Dat betekent dat iedereen vrij is deze software te hergebruiken of aan te passen aan haar wensen.*

bron: [https://openzaak.org/](https://openzaak.org/)

## Inhoudsopgave
* TOC
{:toc}

## Inleiding

De G4-steden werken aan een reeks open source-componenten die kunnen worden gecombineerd tot een platform op basis van ‘zaakgericht werken’.

Op termijn wil de G4 een professioneel en uniform kader definiëren voor het beheer/governance van deze open source-componenten.

## Scope van het huidige voorgestelde project 

De G4 start een pilot rondom OpenZaak, met nadruk op:
* Het governance/beheer van OpenZaak  
* Codereview-proces van bestaande en nieuwe bijdragen

Deze pilot is uitsluitend gericht op de huidige community, bestaande uit:
* Gemeenten: Amsterdam, Rotterdam, Den Haag en Utrecht  
* Leveranciers: Ritense, Maykin, Worth

Deze pilot bouwt voort op het werk dat is verricht tijdens de [OpenZaak-marktconsultatie](https://github.com/open-zaak/open-zaak-market-consultation) in samenwerking met de Foundation for Public Code. 

## Ambitie

De ambitie is om samen met de huidige gemeenschap het volgende te verfijnen en te documenteren:
* Het governance/beheer van OpenZaak (inclusief codebase gerelateerde standaarden, werkafspraken en best practices via bijvoorbeeld de governance file, contributor guidelines, enz.)  
* Het proces van codereview van bestaande en nieuwe bijdragen aan OpenZaak (inclusief het proces van codebase stewardship)  
* Het implementeren, testen en verbeteren van dit governance- en reviewproces in de praktijk   
* Duidelijk maken hoe het bovenstaande beheerd zal worden

Het is de ambitie om dit op een breed toepasbare manier te doen, en met een zodanige kwaliteitsniveau, zodat  gedocumenteerde werkmethoden en normen kunnen worden hergebruikt:
* Voor andere componenten  
* Door andere gemeenten of overheden  
* Door andere potentiële nieuwe leveranciers

## Fase 1: Beoordeling en verbetering van governance (‘beheer’) en codereview

### Benchmark van de huidige stand van zaken op het gebied van governance (‘beheer’) en codereview

* Review van de oorspronkelijke hypothese uit de marktconsultatie  

```
De governance was ontworpen om meerdere zelfgemotiveerde partijen in staat te stellen deel te nemen aan de OpenZaak-community. Dit gebeurde door open technische en product­stuurgroepvergaderingen op te zetten waaraan de community kon deelnemen.

Dit was gebaseerd op de aanname dat marktpartijen zich proactief zouden inzetten als onderdeel van hun business development en zo hun marktaandeel rond OpenZaak zouden vergroten. Dit veronderstelde op zijn beurt dat overheden meerdere kleine opdrachten zouden gaan uitschrijven die openstonden voor verschillende leveranciers, bijvoorbeeld voor ontwikkeling, onderhoud, hosting, implementatie en ondersteuning.
```

* Review van de huidige formele governance- en werkafspraken

```
- Veel informele samenwerking, inclusief informele documentatie.
- Overleggen op vrijdag en dinsdag.
- Aansturing door de G4, maar zonder formele budgettering.
- Regie-organisatie in het vooruitzicht.
- Veel goodwill en tevreden partijen.
- Ambitie om zaken beter te borgen — niet uit wantrouwen, maar om de robuustheid te vergroten.
- Documentatie verouderd
- Eerst dachten op codebase, maar eigenlijk is het ecosysteem - minder op github issues
```


### Bestaande 'issues' met governance (‘beheer’) en het codereviewproces in kaart brengen

Korte 1-op-1-gesprekken met 4 gemeenten en 3 leveranciers (7 in totaal) & in kaart brengen van  
* ongeschreven/de facto werkafspraken

```
Community werkt momenteel heel goed met veel vertrouwen, korte lijntjes, proactiviteit en gevoel van verantwoordelijkheid

Markt partijen communiceren direct met elkaar om problemen op te lossen


```

* ambities  

```
Bedrijfszekerheid van ecosysteem te verbeteren
Voorbereiden op centrale regie en samen exploiteren
```

 * pijnpunten

```
Documentatie kan verbeteren - iets versplintered en verouderd, onderhoud van generieke (niet feature specifieke) documentatie valt niet onder bestaande contracten

Essentiele en continue taken van onderhoud worden nu opgenomen in tijdsgebonden doorontwikkel contracten - continuiteit en bedrijfszekerheid beter geborgd door apart en continue contract 

Pad naar regie is gevoelig, gaat manier van werken veranderen - belangrijk om goedwil niet te verstoren. Zekerheid is belangrijk voor continuiteit.

Onzekerheid over eigenaarschap van de codebase; incl de licensie en auteursrechten

Repository rights (admin, branchbeheer en merge rights) kunnen met meer intentie ingericht worden

Geen duidelijk pad om een tweede marktpartij te betrekken en zo de codebase te borgen

```

* Review met de Standard for Public Code om aanvullende aandachtspunten te identificeren  

```
todo
```

* Opstellen van pull requests om ongeschreven afspraken expliciet te maken, en/of tekortkomingen van bestaande praktijken te documenteren

```
## Update voor readme/governance/contributing file?

Open-sourcegemeenschappen verschillen sterk van karakter. Sommige zijn een samenwerking tussen grote multinationals, andere bestaan uitsluitend uit vrijwillige individuen, en weer andere vormen een gemeenschap die samenwerkt aan het product van een bedrijf. Elk van deze gemeenschappen heeft een ander karakter.

OpenZaak is een duidelijk afgebakend component, specifiek voor de Nederlandse context, onder beheer van de overheid en met een overzichtelijk aantal marktpartijen. Het doel is momenteel niet om zo veel mogelijk bijdragen van zo veel mogelijk partijen te verzamelen, met de codebase als centraal coördinatiepunt.

De nadruk ligt hier op ecosysteembeheer: gecoördineerd opdrachtgeverschap met één (of in de toekomst meerdere) marktpartij(en), waarbij ook afstemming met andere componenten van belang is.

Dit is de reden dat deze gemeenschap geen open community-governance heeft – het bestuur wordt uitgevoerd door landelijke regie om samenwerking in exploitatie en samenhang tussen componenten te waarborgen.

Daarom wordt het merendeel van de ontwikkeling uitgevoerd door partijen die daartoe contractueel zijn aangesteld.

Bijdragen zijn welkom, maar houd er rekening mee dat deze onderhevig zijn aan de bovenstaande dynamiek.

## Bestaande documentatie 

- ZGW discussies op Gemma Zaken - https://github.com/VNG-Realisatie/gemma-zaken/issues/2549
- OpenZaak website - https://openzaak.org/ (openzaak.nl bestaan, maar weet niet van wie)
- Github organisatie - https://github.com/open-zaak
    - Github repository met README - https://github.com/open-zaak/open-zaak
    - en andere repo met info (eg marketconsultation en samenwerken)
- Backlog in Notion omgeving - https://platformvoordienstverlening.notion.site/e9375da1960249bba23c49d038d3c888?v=774cd20f3c9040658e7b7fa008858075
- Readthedocs - https://open-zaak.readthedocs.io/en/stable/
- Gitbook Common Ground - https://dienstverleningsplatform.gitbook.io/platform-generieke-dienstverlening-public/introductie/overzicht-functioneel
- Diverse informatie op CommonGround.nl - https://commonground.nl/file/download/79c73952-5274-4139-8d18-56f7c2839644/15816724882020-02-14%20-%20presentatie%20open%20zaak%20at%20live2020.pdf



```

### Prioriteiten stellen voor verbeteringen in governance en codereview

* Opstellen van issues rond verbetering van governance op basis van ambities en pijnpunten

```
Aangezien dit project minder op codebase niveau, en meer op ecosysteem niveau is gaat zitten, zijn geen issues gemaakt maar wel een verslag document.

## Korte samenvatting van bevindingen

Open source is hier geen doel op zich. Het is gekozen als de beste werkvorm om de overkoepelende doelstellingen zijn digitale soevereiniteit, transparantie en kosteneffectiviteit te behalen.

Het betreft hier geen typisch open-sourceproject waarin wordt gestreefd naar zoveel mogelijk bijdragen van een zo groot mogelijk aantal partijen, met de centrale coördinatie rond de codebase. 

Het is namelijk een duidelijk afgebakend component, specifiek ontwikkeld voor de Nederlandse context, onder beheer van de overheid en met een overzichtelijk aantal marktpartijen.  

De nadruk ligt daardoor meer op de **borging van bedrijfszekerheid door strategische regie van het ecosysteem als geheel**.

In dat licht richt de verbetering van de governance rondom OpenZaak zich op:  
- het versterken van de bedrijfszekerheid van het OpenZaak-ecosysteem, met nadruk op:  
  - productmanagement,  
  - communitymanagement, en  
  - broncodebeheer / codebase-governance;  
- en op de vraag hoe deze functies kunnen worden ingekocht en uitgevoerd, mede met het oog op de komende overgang naar centrale, landelijke regie.

## Geïdentificeerde bedrijfszekerheidsdoelstellingen voor dit pilot

### Documentatie

Documentatie is essentieel voor de bedrijfszekerheid van OpenZaak:  
* vermindert het risico op een busfactor bij deskundige individuen en deelnemende organisaties  
* verlaagt de kosten en tijd voor onboarding van nieuwe individuen en partijen  

**Verbeteringsdoelen OpenZaak.org – single point of entry/truth**  
* herintroductie OpenZaak.org als entree naar het ecosysteem
* huidige informatie updaten waar nodig  
* handleiding naar alle bestaande documentatie en huidige spelers in het ecosysteem  
* verbeterd overzicht van en uitnodiging voor gemeenten, hostingproviders, etc. met uitleg over governance  

**Verbeteringsdoelen documentatie hostingproviders**  
* samenwerken met huidige hostingproviders om documentatie te controleren  
* documentatie verfrissen  
* in de toekomst: continu contract met een partij om niet-feature-specifieke documentatie in stand te houden (of te coördineren)  

### Ecosysteemcoördinator

Het OpenZaak-ecosysteem verandert continu.  

Een coördinator die gestructureerd het ecosysteem bijstuurt, helpt de bedrijfszekerheid te borgen, bijvoorbeeld:  
* goede samenwerking in stand houden en verbeteren 
* opsporen, voorkomen en oplossen van spanningen en conflicten tussen partijen  
* risico’s en kansen identificeren  
* oog hebben voor zaken waar niemand anders verantwoordelijk voor is  

**Verbeteringsdoelen**  
* eenmalig stand van zaken in kaart brengen, actualiseren en interventies bepalen (workshop 1)  
* opstarten van 6-maandelijkse review met Miro-board voor retrospectieve, bedrijfszekerheidsfactoren en toekomstscenario’s, en dynamieken + ingrepen bespreken  

### Financieringsstromen

Bewuste financieringsstromen verbeteren de bedrijfszekerheid door:  
* inzichtelijk te maken welk werk gedaan (en nodig) is, en wie het betaald heeft  
* het gemakkelijker maken om werk te verdelen waar nodig  
* continuïteit te garanderen voor de uitvoerende, en daarmee ook voor de afnemende partijen  

**Verbeteringsdoelen**  
* werk opdelen in duidelijke, onafhankelijke contracten (duidelijke labels voor al het werk)  
* continu noodzakelijk werk borgen met een specifiek en continu contract  

### Eigenaarschap

Duidelijkheid rondom eigenaarschap van de codebase:  
* voorkomt onzekerheid bij externe partijen  
* voorkomt wettelijke onzekerheid  
* voorkomt mogelijke toekomstige conflicten  

**Verbeteringsdoelen**  
* verduidelijkende tekst laten schrijven voor de website/codebase/governance file over EUPL  

### Branchbeheer en merge rights

Werkelijk beheer van welke code waar wordt toegevoegd:  
* technische bedrijfszekerheid voor goede code  
* bedrijfszekerheid van service delivery  

**Verbeteringsdoelen**  
* aparte gemeente-only repo voor release branches (archief/backup/publicatieplaats/"landelijke voorziening")  

### Rollen in het ecosysteem

Het goed verdelen van rollen rondom OpenZaak helpt de bedrijfszekerheid door:  
* warme kennis bij verschillende partijen  
* meer ogen en perspectieven  
* ecosysteem ingericht op samenwerking is toegankelijker voor nieuwe partijen  
* betere documentatie, omdat het voor een ander wordt gedocumenteerd  
* gebruikers van de code (implementatie/hosting/etc.) geven gevonden bugs en verbeteringen door, die daardoor beter navolgbaar zijn  
* inrichten van het ecosysteem op samenwerking zorgt voor een codebase/repository die beter georganiseerd is voor samenwerking (Conway's Law)  

**Verbeteringsdoelen**  
* in Workshop 2 onderzoeken we gezamenlijk mogelijke samenwerkingspatronen en stappen, bijv. over hoe meerdere partijen kunnen bijdragen/meekijken in het ontwikkelproces.


```

* Community uitnodigen om deze te beoordelen en aan te vullen  

```
In twee workshops en bilateraal met verschillende partijen
G4 vrijdag over heeft sturing gegeven op prioritiseren van doelen en ambities 
```

* Gezamenlijke workshop om de belangrijkste issues rond verbetering van governance te selecteren en verfijnen

```

# Workshop 1 - Governance Goals

## Agenda

Introduction (10 min)
Reflections (10 min)
Huidig OpenZaak ecosysteem (30 min)
Pauze (10 min)
-
SWOT op huidige ecosysteem (25 min)
Dynamieken binnen huidig ecoystem (30 min)
Closing & next steps (5 min)


```


### Documentatie voor governance en codereview opstellen en consolideren

* Verbeteringen voorstellen met betrekking tot governance en codereview  
    * Deze voorstellen aanleveren via pull requests  

```
Niet in de vorm van pull requests. Wel een Miro board.

@todo - hier miroboard van voorstel?

```

* Tweede gezamenlijke workshop om voorgestelde wijzigingen te beoordelen en verfijnen 

```
# Workshop 2 - Governance Proposals

## Agenda

We gaan tijdens de workshop aan de slag met a) rollen binnen het ecosysteem, b) branch en merge rights, c) eigenaarschap en beheer. 

## Praktisch

Tijd: 10.15-10.30: Inloop & koffie, 10.30-12.30: Workshop
Locatie: Common Ground Field Lab, WTC Utrecht

## Agenda

- Resultaten vorige workshop en highlights verslag
- Voorstelvisie ecosysteem
- Breakouts
  - Praktische werkbaarheid & developersperspectief 
  - Budget, planning en contracten
  - Toepasbaarheid op andere componenten
- Closing & vervolgstappen

```

* Herziening en implementatie van de voorstellen

```
Geen extra documentatie 
```


Onderwerpen die hierbij aan bod komen:
* Aansprakelijkheid, licenties, intellectueel eigendom, overdracht van auteursrechten, handelsmerken  

```
EUPL verklarende text
```

* Richtlijnen voor inkoop (inclusief leveranciersselectie) 

```

```

* Documentatie van processen  
  
```

```

* Wijzigingsprocedures voor codebase stewardship  

```

```

* Proces voor het accepteren van bijdragen  

```

```

* Eventueel voorzitterschap/deelname bij meetings waar nodig

```

```

## Fase 2: Toepassen en verbeteren van nieuw governance en codereview

### Iteratief toepassen van nieuwe governance- en codereviewprocessen

* Conceptoplossingen uitvoeren met gerichte feedbackloops  
* Evaluatie van kosten, risico’s en kansen bij de toepassing ervan

### Duurzaamheid van governance- en codereviewprocessen op lange termijn

* Voorstellen hoe codebase stewardship na de pilot wordt voortgezet

```
## Codebase stewardship ‘vanilla’-variant

Open source als manier van samenwerken wordt vaak gebruikt, en is zeer effectief, bij het faciliteren van samenwerking tussen partijen met uiteenlopende belangen. Denk aan duizenden vrijwillige ontwikkelaars, of 3–5 grote bedrijven die elk hun eigen business nastreven of zelfs met elkaar concurreren.  

In zo’n situatie is codebase-stewardship een activiteit die de belangen van de codebase en de gemeenschap als geheel beschermt, onafhankelijk van de belangen van individuele leden van die gemeenschap.  

In het geval van MariaDB bijvoorbeeld: Amazon, Tencent, Alibaba, Microsoft, enz. gebruiken de databasesoftware, en profiteren allemaal van elkaars investeringen in het verbeteren van de software, *EN* hebben elk hun eigen commerciële belangen. De MariaDB Foundation beheert de codebase vanuit een onafhankelijke positie (het bestuur bestaat uit mensen die door de grote bedrijven worden aangewezen) om het in het midden te houden, en te voorkomen dat één luide stem de overhand krijgt of dat de samenwerking fragmentarisch wordt bij conflicten. Idem bvb bij Linux Foundation etc.

De Foundation for Public Code hanteerde een vergelijkbaar perspectief – als Nederlandse codebases worden hergebruikt door Frankrijk, Duitsland en Italië, hoe zorgen we dat de belangen van één partij de samenwerking niet breken. En tijdens de OpenZaak-marktconsultatie – zodat de open samenwerking tussen Maykin, de implementatiepartners, andere ontwikkelpartijen, allemaal met hun eigen belangen, kan worden gemedieerd vanuit een neutraal perspectief dat beslissingen neemt in het beste belang van de codebase, wat op zijn beurt ten goede komt aan iedereen (inclusief de gemeenten).  

## Codebase stewardship ‘common ground’-variant

Bij landelijke regie en samen exploiteren geldt het bovenstaande niet direct voor de Common Ground-componenten, simpelweg omdat:  

* er één gecoördineerd opdrachtgeverschap is – governance vindt niet (alleen) op codebase-niveau plaats, maar op niveau van landelijke regie en componentportfolio  

* er een zeer nauwe afhankelijkheid tussen componenten is – ze staan of groeien niet zelfstandig  

* sommige componenten de implementatie van Nederlandse wet bevatten – territoriaal gebonden  

* gezien het bovenstaande is het onwaarschijnlijk dat een bedrijf spontaan zal komen en een businessmodel rond een component zal ontwikkelen (kan voor sommige componenten wel gebeuren)

Dit betekent dat de Common Ground-variant van codebase-stewardship (als we het zo blijven noemen) omvat:  

* collectief producteigenaarschap (behoeften/verzoeken/financiering verzamelen)  

* portfoliomanagement van componenten (afhankelijkheden, groeipaden, integratie)  

* release management (roadmaps, planning, breaking changes, etc.)  

* regie over het vendor-ecosysteem (samenwerking ontwikkelpartij, reviewpartij, onderhoudscontract en SaaS-aanbieder en alle contract- en relatiemanagement die daarbij hoort)

* de strategische belangrijkheid en volwassenheid van een component evalueren om te bepalen hoeveel redundantie en bedrijfszekerheid nodig is (bijv. een tweede leverancier)

Ik zie hier wel een zekere hybriditeit. Voor sommige componenten kan a) een paar marktpartijen direct diensten aan gemeenten willen aanbieden (bijvoorbeeld lokaal versnellen of een specifieke één-gemeente feature) of b) een niet-gemeentelijke of internationale partij willen deelnemen. In dat geval moet worden geëvalueerd of deelname aan de samenwerking voordelig is voor de codebase (meer mensen investeren erin) of juist een remmende factor is (meer complexiteit dan het waard is). Mijn gevoel is dat dit per component/gemeenschap beoordeeld zal moeten worden.

In elk geval, als landelijke regie en samen exploiteren de uitgangspunten zijn, dan is de kernwaarde van codebase-stewardship (het beschermen van de belangen van de codebase onafhankelijk van één enkele partij) geen doel om op te optimaliseren. Er is een duidelijke enkele partij - het belang van landelijke regie. Er kan een deur open worden gelaten voor anderen om deel te nemen, en als plotseling andere Nederlandse ministeries of buitenlandse gemeenten instappen, in die mate dat het de moeite waard is om te bemiddelen tussen hun behoeften en die van de landelijke regieorganisatie – dan heeft ‘vanilla’ codebase-stewardship wel zin - en dan waarschijnlijk voor het platform als geheel, via de "Stichting Platform Zaakgericht Werken" of iets dergelijks, en niet op componentniveau.

Dus ik zou misschien het bovenstaande lijstje aanvullen met:
* het realistische schaalbaarheids- en herbruikbaarheidspotentieel van de component beoordelen, evenals het realistische potentieel voor bijdragen door de community (wat beslissingen kan ondersteunen over hoe open issue-trackers, roadmaps, besluitvorming, enz. ingericht moeten worden.)


Zoals genoemd in de OpenZaak-workshop lijkt het ons nuttig dat er vanuit landelijke regie:

* een centrale plek is met een overzicht van alle componenten (en hun versies)  

* een manier is om dependencies tussen de componenten duidelijk te beschrijven  

* communicatie plaatsvindt naar implementatie/hostingpartners over breaking changes, releases, roadmaps, etc.

Er lijkt dus een kans om een proof of concept te doen rond 'portfolio management van componenten in één git-hosting platform':

* één (of meerdere) git-hostingplatformen te kiezen als test  

* daar de laatste stable release van alle componenten beschikbaar te hebben (voor nu als downstream clones)  

* en de oefening uit te voeren om dependencies tussen versies te beschrijven, te verkennen hoe communicatie naar hergebruikers zou kunnen verlopen, enzovoort

```


* Voorstellen voor financiering codebase stewardship 
* Voorstellen voor het beheer van de processen die voorkomen uit deze pilot
* Voorstellen voor afstemming tussen de zaakgericht werken componenten 

### Afronden van hoogwaardige, herbruikbare documentatie van governance en codereview

Onderdeel hiervan zijn updates op:
* Algemeen inleidend overzicht van de opbouw van de OpenZaak-gemeenschap  
* Richtlijnen voor nieuwe deelnemende gemeenten  
* `GOVERNANCE.md`  
* `CONTRIBUTING.md`  
* `code_of_conduct.md`  
* OpenZaak-website  
* Definitieve documentatie van het pilotproces, inclusief reflecties  
* Opzetten van verschillende repositories die door anderen kunnen worden hergebruikt

Deze documentatie moet bevatten:
* Duidelijke verklaringen over aansprakelijkheid, licenties, intellectueel eigendom, overdracht van auteursrechten, handelsmerken  
* Duidelijke instructies over aanbestedingsrichtlijnen (inclusief leveranciersselectie)

## Fase 3: Uitbreiding naar andere codebases

* Uitbreiding van het raamwerk, best practices en richtlijnen naar andere codebases en communities
* Codebase stewardship op andere codebases mogelijk maken en faciliteren

### Werkprincipes 

* Werk zoveel mogelijk in het open (issues en pull requests) om ervoor te zorgen dat alle stappen open zijn
* Leer van best practices in en buiten de EU 

## Tijdlijn

Start fase 1 - 21 juli 2025  
Workshop 1 - eind september 2025  
Workshop 2 - mid november 2025  
Start fase 2 - eind november 2025  
Einde fase 2 - januari 2026  

## Afhankelijkheden

Minimum vereisten:  
- 10-16 uur van elke leverancier (1 interview, 2 workshops, en schriftelijke feedback op issues en pull requests)  
- 10-16 uur van elke gemeente (1 interview, 2 workshops, en schriftelijke feedback op issues en pull requests)

## Relevante bronnen: 

* Standard for Public Code - https://www.standardforpubliccode.org/
* Dutch Translation for the Standard - https://www.standaardvoorpubliekecode.nl/
* OpenZaak Market Consultation - https://github.com/open-zaak/open-zaak-market-consultation
* Governance Game - https://github.com/governance-game/
