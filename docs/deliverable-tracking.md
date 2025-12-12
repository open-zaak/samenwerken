---
layout: default
---

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

Zie [Verslag codebase stewarship OpenZaak](verslag-codebase-stewardship)

* Review van de huidige formele governance- en werkafspraken

Zie [Verslag codebase stewarship OpenZaak](verslag-codebase-stewardship)

### Bestaande 'issues' met governance (‘beheer’) en het codereviewproces in kaart brengen

Korte 1-op-1-gesprekken met 4 gemeenten en 3 leveranciers (7 in totaal) & in kaart brengen van  
* ongeschreven/de facto werkafspraken
* ambities  
* pijnpunten

```
De interviews waren vertrouwelijk om openheid en kwetsbaarheid te waarborgen, en de directe output is niet openbaar.

Hieronder een korte samenvatting van de bevindingen:

## Werkafspraken

* De Community functioneert momenteel zeer goed, gekenmerkt door:
    * Veel vertrouwen.
    * Korte lijntjes en directe communicatie.
    * Proactiviteit en een sterk gevoel van verantwoordelijkheid.
* Marktpartijen communiceren direct met elkaar om problemen op te lossen.

## Ambities

* De bedrijfszekerheid van het ecosysteem verbeteren.
* Zich voorbereiden op centrale regie en samen exploiteren.

## Pijnpunten

### Documentatie en Onderhoud

* Documentatie kan verbeteren: deze is enigszins versnipperd en verouderd.
* Het onderhoud van generieke (niet-feature-specifieke) documentatie valt niet onder bestaande contracten.
* Essentiële en continue onderhoudstaken worden momenteel opgenomen in tijdsgebonden doorontwikkelingscontracten. De continuïteit en bedrijfszekerheid zouden beter geborgd zijn door een apart en continu contract.

### Regie en Continuïteit

* Het pad naar regie is gevoelig, aangezien dit de huidige manier van werken zal veranderen.
* Het is belangrijk om de bestaande goedwil niet te verstoren. Zekerheid is cruciaal voor continuïteit.

### Codebase en Eigenaarschap

* Onzekerheid over het eigenaarschap van de codebase, inclusief de licentie en auteursrechten.
* Repository-rechten (admin, branchbeheer en merge-rechten) kunnen met meer intentie en structuur worden ingericht.
* Er is geen duidelijk pad om een tweede marktpartij te betrekken en zo de codebase te borgen.

```

* Review met de Standard for Public Code om aanvullende aandachtspunten te identificeren  

```
todo
```

* Opstellen van pull requests om ongeschreven afspraken expliciet te maken, en/of tekortkomingen van bestaande praktijken te documenteren

```
Aangezien dit project minder op codebase niveau, en meer op ecosysteem niveau is gaan zitten, zijn geen pull requests gemaakt.
```

### Prioriteiten stellen voor verbeteringen in governance en codereview

* Opstellen van issues rond verbetering van governance op basis van ambities en pijnpunten

```
Aangezien dit project minder op codebase niveau, en meer op ecosysteem niveau is gaan zitten, zijn geen issues gemaakt maar wel een verslag document.
```

Zie [Verslag bedrijfszekerheid OpenZaak](verslag-bedrijfszekerheidsdoelen)

* Community uitnodigen om deze te beoordelen en aan te vullen  

```
In twee workshops en bilateraal met verschillende partijen
G4 vrijdag overleg heeft sturing gegeven op prioritiseren van doelen en ambities 
```

* Gezamenlijke workshop om de belangrijkste issues rond verbetering van governance te selecteren en verfijnen

Zie [Workshop 1](workshop-1-governance-goals/index)

### Documentatie voor governance en codereview opstellen en consolideren

* Verbeteringen voorstellen met betrekking tot governance en codereview  
    * Deze voorstellen aanleveren via pull requests  
```
Niet in de vorm van pull requests. Zie verslagen hieronder
```
* Tweede gezamenlijke workshop om voorgestelde wijzigingen te beoordelen en verfijnen 

Zie [Workshop 2](workshop-2-governance-proposals/index)
Zie [Verslag Ecosysteem En Rollen](verslag-ecosysteem-en-rollen)

* Herziening en implementatie van de voorstellen

```
Geen extra documentatie 
```

Onderwerpen die hierbij aan bod komen:
* Aansprakelijkheid, licenties, intellectueel eigendom, overdracht van auteursrechten, handelsmerken  

Zie [verslag-EUPL-verklarende-text](verslag-EUPL-verklarende-text)

* Richtlijnen voor inkoop (inclusief leveranciersselectie) 

```
to do 

```
Zie [Verslag Ecosysteem En Rollen](verslag-ecosysteem-en-rollen)

* Documentatie van processen  
* Wijzigingsprocedures voor codebase stewardship  
* Proces voor het accepteren van bijdragen  

Zie [Verslag codebase stewardship](verslag-codebase-stewardship)

* Eventueel voorzitterschap/deelname bij meetings waar nodig

```
Niet nodig geweest
```

## Fase 2: Toepassen en verbeteren van nieuw governance en codereview

### Iteratief toepassen van nieuwe governance- en codereviewprocessen

* Conceptoplossingen uitvoeren met gerichte feedbackloops  
* Evaluatie van kosten, risico’s en kansen bij de toepassing ervan

```
Geen extra documentatie
```

### Duurzaamheid van governance- en codereviewprocessen op lange termijn

* Voorstellen hoe codebase stewardship na de pilot wordt voortgezet
* Voorstellen voor financiering codebase stewardship 
* Voorstellen voor het beheer van de processen die voorkomen uit deze pilot
* Voorstellen voor afstemming tussen de zaakgericht werken componenten 

Zie [Verslag codebase stewardship](verslag-codebase-stewardship)

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

```
todo - pull requests op openzaak repo, website en readthedocs
```

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
