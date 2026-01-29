---
layout: default
title: De rol van Codebase Stewardship
nav_order: 2
---

# De rol van Codebase Stewardship

Dit document bevat de initiele reflecties op het karakter van de OpenZaak community en de rol van codebase stewardship binnen OpenZaak.
Deze kunnen worden doorgetrokken naar de zaakgerichte componenten in het algemeen.

## Inhoudsopgave
* TOC
{:toc}

## Inleiding: oorspronkelijke hypothese uit de marktconsultatie  

De governance van OpenZaak was ontworpen om meerdere zelfgemotiveerde partijen in staat te stellen deel te nemen aan de OpenZaak-community.

Dit gebeurde door open technische overleggen en product­stuurgroepvergaderingen te organiseren waaraan de community kon deelnemen.

Deze opzet was gebaseerd op de aanname dat marktpartijen zich proactief zouden inzetten als onderdeel van hun business development, en zo hun marktaandeel rond OpenZaak zouden vergroten.

Daarbij werd verondersteld dat overheden meerdere, relatief kleine opdrachten zouden uitschrijven die openstonden voor verschillende leveranciers, bijvoorbeeld voor ontwikkeling, onderhoud, hosting, implementatie en ondersteuning.

## Wat zijn de karakteristieken van de OpenZaak-community?

Open-sourcegemeenschappen verschillen sterk van karakter. Sommige bestaan uit samenwerkingen tussen grote multinationals, andere uit vrijwillige individuen, en weer andere uit gemeenschappen die samenwerken aan het product van één bedrijf. Elk van deze modellen kent zijn eigen dynamiek en governancevorm.

OpenZaak is een duidelijk afgebakende component, specifiek voor de Nederlandse context, onder beheer van de overheid en met een overzichtelijk aantal marktpartijen. Het primaire doel is momenteel niet om zo veel mogelijk bijdragen van zo veel mogelijk partijen te verzamelen, met de codebase als centraal coördinatiepunt.

De nadruk ligt op ecosysteembeheer: gecoördineerd opdrachtgeverschap met één (of in de toekomst meerdere) marktpartij(en), waarbij ook afstemming met andere componenten essentieel is.

Dit verklaart waarom deze gemeenschap geen typische open community-governance kent. De ambitie is bovendien om het bestuur in de toekomst vanuit landelijke regie te organiseren, de componenten gezamenlijk te exploiteren en de samenhang tussen componenten te waarborgen.

Daarom wordt het merendeel van de ontwikkeling uitgevoerd door partijen die daartoe contractueel zijn aangesteld.

## Hoe beïnvloedt deze vorm codebase stewardship?

### Codebase stewardship – ‘vanilla’-variant

Open source als samenwerkingsmodel wordt vaak en met succes ingezet om samenwerking te faciliteren tussen partijen met uiteenlopende belangen. Dit kan gaan om duizenden vrijwillige ontwikkelaars, maar ook om drie tot vijf grote bedrijven die elk hun eigen commerciële belangen nastreven of zelfs met elkaar concurreren.

In dergelijke situaties is codebase stewardship gericht op het beschermen van de belangen van de codebase en de gemeenschap als geheel, los van de belangen van individuele deelnemers.

Bij MariaDB bijvoorbeeld gebruiken partijen als Amazon, Tencent, Alibaba en Microsoft dezelfde databasesoftware. Zij profiteren van elkaars investeringen in verbeteringen, terwijl zij tegelijkertijd elk hun eigen commerciële agenda hebben. De MariaDB Foundation beheert de codebase vanuit een relatief onafhankelijke positie (met een bestuur dat wordt aangewezen door de betrokken bedrijven) om machtsconcentratie te voorkomen en samenwerking duurzaam te houden. Vergelijkbare modellen bestaan bij onder andere de Linux Foundation.

De Foundation for Public Code hanteerde een vergelijkbaar perspectief: als Nederlandse codebases worden hergebruikt door bijvoorbeeld Frankrijk, Duitsland en Italië, hoe voorkom je dan dat de belangen van één partij de samenwerking verstoren?

Ook tijdens de OpenZaak-marktconsultatie was dit een relevant uitgangspunt: open samenwerking tussen Maykin, implementatiepartners en andere ontwikkelpartijen – elk met hun eigen belangen – vraagt om een neutraal perspectief dat beslissingen neemt in het belang van de codebase als geheel, wat uiteindelijk ook de gemeenten ten goede komt.

### Codebase stewardship – ‘landelijke voorziening’-variant

Bij landelijke regie en gezamenlijk exploiteren geldt bovenstaande benadering niet één-op-één voor Common Ground-componenten, om de volgende redenen:

* er is sprake van één gecoördineerd opdrachtgeverschap; governance vindt niet uitsluitend op codebase-niveau plaats, maar ook op het niveau van landelijke regie en het componentportfolio  
* er bestaan nauwe afhankelijkheden tussen componenten; zij staan of groeien niet volledig zelfstandig  
* sommige componenten implementeren Nederlandse wet- en regelgeving en zijn daarmee territoriaal gebonden  
* gezien het bovenstaande is het onwaarschijnlijk dat bedrijven spontaan een zelfstandig businessmodel rond een component ontwikkelen (al kan dit voor sommige componenten wel het geval zijn)

Dit betekent dat de ‘landelijke voorziening’-variant van codebase stewardship onder meer omvat:

* collectief producteigenaarschap (het verzamelen en prioriteren van behoeften, verzoeken en financiering)  
* portfoliomanagement van componenten (afhankelijkheden, groeipaden, integratie)  
* release management (roadmaps, planning, breaking changes)  
* regie over het vendor-ecosysteem (samenwerking tussen ontwikkelpartij, reviewpartij, onderhoudspartij en SaaS-aanbieder, inclusief contract- en relatiemanagement)  
* het beoordelen van de strategische importantie en volwassenheid van componenten om de benodigde mate van redundantie en bedrijfszekerheid te bepalen (bijvoorbeeld een tweede leverancier)  
* het inschatten van realistisch schaalbaarheids- en hergebruikspotentieel, evenals het verwachte bijdragepotentieel van de community (wat richting geeft aan hoe open issue-trackers, roadmaps en besluitvorming worden ingericht)

Voor sommige componenten kan het voorkomen dat:
a) één of meerdere marktpartijen direct diensten aan gemeenten willen aanbieden (bijvoorbeeld lokale versnelling of een specifieke feature voor één gemeente), of  
b) een niet-gemeentelijke of internationale partij wil deelnemen.

In zulke gevallen moet worden geëvalueerd of deelname aan de samenwerking de codebase versterkt (meer investeringen en kennis) of juist belemmert (meer complexiteit dan de opbrengst rechtvaardigt). Deze afweging zal per component en per gemeenschap moeten worden gemaakt.

Wanneer landelijke regie en gezamenlijk exploiteren de uitgangspunten zijn, is de klassieke kernwaarde van codebase stewardship – het beschermen van de codebase tegen de invloed van één dominante partij – geen primair optimalisatiedoel.

Er is immers één duidelijk leidend belang: dat van de landelijke regie.

Wel kan ruimte worden gelaten voor deelname door andere partijen (bijvoorbeeld andere Nederlandse of buitenlandse overheidsinstellingen), voor zover het de moeite waard is om hun belangen te bemiddelen met die van de landelijke regieorganisatie. In dat geval kan ‘vanilla’ codebase stewardship alsnog relevant zijn, maar dan eerder op platformniveau (bijvoorbeeld via een entiteit als de *Stichting Platform Zaakgericht Werken*) dan op het niveau van individuele componenten.

### Centrale git-hostingplatform?

Het lijkt zinvol dat vanuit landelijke regie wordt voorzien in:

* één centrale plek met een overzicht van alle componenten en hun versies  
* een expliciete beschrijving van afhankelijkheden tussen componenten  
* gestructureerde communicatie richting implementatie- en hostingpartners over releases, breaking changes en roadmaps  

Dit biedt een kans om een proof of concept te ontwikkelen rond *portfoliomanagement van componenten binnen één git-hostingplatform*:

* het beschikbaar maken van de laatste stabiele releases van alle componenten (bijvoorbeeld als downstream clones)  
* het expliciet modelleren van afhankelijkheden tussen versies  
* het verkennen van effectieve vormen van communicatie richting hergebruikers  

## Hoe beïnvloedt dit de governance binnen OpenZaak?

Dit alles betekent dat de governance binnen OpenZaak afwijkt van die van een klassiek (‘vanilla’) open-sourceproject.

Zie ook: Verslag governance ecosysteem en rollen
