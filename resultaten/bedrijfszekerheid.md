---
layout: default
title: Bedrijfszekerheid als primaire doel voor OpenZaak
parent: Resultaten
nav_order: 1
---

# Bedrijfszekerheid als primaire doel voor OpenZaak

Dit document belicht de bedrijfszekerheidsdoelen die tijdens het traject naar voren zijn gekomen vanuit de stakeholders.

## Inhoudsopgave
* TOC
{:toc}

## Korte samenvatting van bevindingen

Opensourcewerken is in deze context geen doel op zich, maar de gekozen werkvorm die aansluit op bredere doelstellingen: digitale soevereiniteit, transparantie en kosteneffectiviteit.

Het betreft geen klassiek opensourceproject waarin wordt gestuurd op zo veel mogelijk bijdragen van zo veel mogelijk partijen met de codebase als primair coördinatiepunt.

OpenZaak is een duidelijk afgebakende component, specifiek ontwikkeld voor de Nederlandse context, onder beheer van de overheid, met een beperkt aantal marktpartijen (*het ecosysteem*).

De nadruk ligt daardoor nu op de **borging van bedrijfszekerheid door middel van strategische regie over het ecosysteem als geheel**.

In dat licht richt de verbetering van de governance rondom OpenZaak zich op:
* het versterken van de bedrijfszekerheid van het OpenZaak-ecosysteem, met nadruk op:  
  * productmanagement,  
  * communitymanagement, en  
  * broncodebeheer en codebase-governance;  
* en op de vraag hoe deze functies kunnen worden ingekocht en uitgevoerd, mede met het oog op een toekomstige overgang naar centrale, landelijke regie.  

## Geïdentificeerde bedrijfszekerheidsdoelstellingen voor deze pilot

### Documentatie

Goede documentatie is essentieel voor de bedrijfszekerheid van OpenZaak, omdat deze:
* zorgt voor minder afhankelijkheid van specifieke organisaties en experts ([busfactor](https://en.wikipedia.org/wiki/Bus_factor));
* zorgt voor lagere kosten en kortere doorlooptijd voor onboarding van zowel nieuwe partijen als nieuwe medewerkers bij bestaande partijen.

**Verbeteringsdoelen OpenZaak.org**
* herintroductie van OpenZaak.org als centrale toegang tot en overzicht van het ecosysteem (single point of entry / single source of truth);
* actualiseren van bestaande informatie waar nodig;
* bieden van een duidelijke wegwijzer naar alle bestaande documentatie en huidige spelers in het ecosysteem;
* een verbeterd overzicht en uitnodiging voor gemeenten, hostingproviders en andere betrokkenen, inclusief uitleg over governance.

**Verbeteringsdoelen documentatie voor hostingproviders**
* samenwerken met bestaande hostingproviders om documentatie te controleren en waar nodig te actualiseren en verhelderen;
* op termijn: een doorlopend contract met een partij om niet-feature-specifieke documentatie te onderhouden of te coördineren.

### Ecosysteemcoördinator
Het OpenZaak-ecosysteem is voortdurend in ontwikkeling.

Een coördinator die het ecosysteem gestructureerd volgt en bijstuurt, draagt bij aan de bedrijfszekerheid door onder meer:
* het opbouwen, behouden en verbeteren van relaties en samenwerking tussen partijen;
* het signaleren, voorkomen en oplossen van spanningen en conflicten;
* het identificeren van risico’s en kansen;
* aandacht te hebben voor onderwerpen waarvoor geen expliciete eigenaar is.

**Verbeteringsdoelen**
* eenmalig een actueel beeld van de stand van zaken opstellen en op basis daarvan interventies bepalen (Workshop 1);
* organiseren van halfjaarlijkse ecosysteem retrospective (ecosysteem mapping), waarin alle stakeholders gezamenlijk kijken naar bedrijfszekerheidsfactoren, toekomstscenario’s en relevante dynamieken en mogelijke ingrepen.

### Financieringsstromen
Bewust ingerichte financieringsstromen dragen bij aan bedrijfszekerheid door:
* inzichtelijk te maken welk werk wordt (en moet worden) uitgevoerd, door wie dit wordt uitgevoerd en door wie dit wordt gefinancierd;
* het eenvoudiger te maken om werk te (her)verdelen wanneer dat nodig is;
* continuïteit te bieden voor uitvoerende partijen, en daarmee ook voor het ecosysteem als geheel en de afnemers.

**Verbeteringsdoelen**
* werk opdelen in duidelijke, (zo veel mogelijk) onafhankelijke contracten, met eenduidige labels voor werkzaamheden;  
* structureel, noodzakelijk werk borgen via specifieke, doorlopende contracten.

### Eigenaarschap
Duidelijkheid over het eigenaarschap van de codebase:
* voorkomt onzekerheid bij externe partijen; 
* verkleint juridische onduidelijkheid;
* reduceert het risico op toekomstige conflicten.

**Verbeteringsdoelen**
* het laten opstellen van een verduidelijkende tekst over de EUPL voor de website, de codebase en/of de governance file.

### Branchbeheer en merge rights
Heldere afspraken over waar en hoe code wordt toegevoegd zijn van belang voor:
* technische bedrijfszekerheid, bijvoorbeeld bij het wegvallen van een repository van de ontwikkelpartij;
* duidelijk controlemoment op codekwaliteit;
* duidelijke vindplaats voor gecontroleerde versies (in samenhang met andere componenten) voor service delivery.

**Verbeteringsdoelen**
* het inrichten van een aparte, gemeente-only repository voor release-branches (bijvoorbeeld als archief, backup en publicatieplaats voor de ‘landelijke voorziening’).

### Rollen in het ecosysteem
Een duidelijke, mogelijk wisselende rolverdeling met kwaliteitscontrole binnen het OpenZaak-ecosysteem draagt bij aan bedrijfszekerheid door:
* het borgen van warme kennis bij meerdere partijen (de ontwikkelaar, de beheerder en de reviewpartij, optioneel afwisselend);
* meer perspectieven op implementatie en kwaliteit;
* noodzaak tot betere documentatie om kennis overdraagbaar te maken, waardoor het ecosysteem toegankelijker wordt voor nieuwe partijen;
* betere terugkoppeling van bugs en verbeteringen door verschillende typen gebruikers van de code (implementatie, hosting, etc.);
* een ecosysteemstructuur die samenwerking ondersteunt en bijpassend georganiseerde codebase en repository ([Conway’s Law](https://en.wikipedia.org/wiki/Conway%27s_law)).

**Verbeteringsdoelen**
* in [Workshop 2](/aanpak/workshop-2-governance-proposals/) gezamenlijk mogelijke samenwerkingspatronen en vervolgstappen onderzoeken, bijvoorbeeld rond het bijdragen aan en meekijken in het ontwikkelproces door meerdere partijen.
