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
todo
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
Zie hierboven, niet in de vorm van pull requests
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

Onderwerpen die hierbij aan bod komen:
* Aansprakelijkheid, licenties, intellectueel eigendom, overdracht van auteursrechten, handelsmerken  

```
EUPL verklarende text
```

* Richtlijnen voor inkoop (inclusief leveranciersselectie) 

```

```

* Documentatie van processen  
* 
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
