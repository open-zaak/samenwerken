---
layout: default
title: Verslag codebase stewarship OpenZaak
nav_order: 2
---

# Verslag: OpenZaak codebase stewardship

Status: DRAFT

Dit document reflecteert op het karakter van de OpenZaak community en de rol van codebase stewardship binnen OpenZaak.
Deze kunnen worden doorgetrokken naar de zaakgerichte componenten in het algemeen.

## Inhoudsopgave
* TOC
{:toc}

## Context: oorspronkelijke hypothese uit de marktconsultatie  

De governance van OpenZaak was ontworpen om meerdere zelfgemotiveerde partijen in staat te stellen deel te nemen aan de OpenZaak-community.

Dit gebeurde door open technische en product­stuurgroepvergaderingen op te zetten waaraan de community kon deelnemen.

Dit was gebaseerd op de aanname dat marktpartijen zich proactief zouden inzetten als onderdeel van hun business development en zo hun marktaandeel rond OpenZaak zouden vergroten.

Dit veronderstelde op zijn beurt dat overheden meerdere kleine opdrachten zouden gaan uitschrijven die openstonden voor verschillende leveranciers, bijvoorbeeld voor ontwikkeling, onderhoud, hosting, implementatie en ondersteuning.

## Wat zijn de characteristieken van de OpenZaak community?

Open-sourcegemeenschappen verschillen sterk van karakter.
Sommige zijn een samenwerking tussen grote multinationals, andere bestaan uitsluitend uit vrijwillige individuen, en weer andere vormen een gemeenschap die samenwerkt aan het product van een bedrijf.
Elk van deze gemeenschappen heeft een ander karakter.

OpenZaak is een duidelijk afgebakend component, specifiek voor de Nederlandse context, onder beheer van de overheid en met een overzichtelijk aantal marktpartijen.
Het doel is momenteel niet om zo veel mogelijk bijdragen van zo veel mogelijk partijen te verzamelen, met de codebase als centraal coördinatiepunt.

De nadruk ligt hier op ecosysteembeheer: gecoördineerd opdrachtgeverschap met één (of in de toekomst meerdere) marktpartij(en), waarbij ook afstemming met andere componenten van belang is.

Dit is de reden dat deze gemeenschap geen typische open community-governance heeft. Het is ambitie is ook om in de toekomst het bestuur uit te voeren door landelijke regie, samen te exploiteren, en de samenhang tussen componenten te waarborgen.

Daarom wordt het merendeel van de ontwikkeling uitgevoerd door partijen die daartoe contractueel zijn aangesteld.

## Hoe beinvloed deze vorm codebase stewardship?

### Codebase stewardship ‘vanilla’-variant

Open source als manier van samenwerken wordt vaak gebruikt, en is zeer effectief, bij het faciliteren van samenwerking tussen partijen met uiteenlopende belangen.
Denk aan duizenden vrijwillige ontwikkelaars, of 3–5 grote bedrijven die elk hun eigen business nastreven of zelfs met elkaar concurreren.  

In zo’n situatie is codebase-stewardship een activiteit die de belangen van de codebase en de gemeenschap als geheel beschermt, onafhankelijk van de belangen van individuele leden van die gemeenschap.  

In het geval van MariaDB bijvoorbeeld: Amazon, Tencent, Alibaba, Microsoft, enz. gebruiken de databasesoftware, en profiteren allemaal van elkaars investeringen in het verbeteren van de software, *EN* hebben elk hun eigen commerciële belangen.
De MariaDB Foundation beheert de codebase vanuit een onafhankelijke positie (het bestuur bestaat uit mensen die door de grote bedrijven worden aangewezen) om het in het midden te houden, en te voorkomen dat één luide stem de overhand krijgt of dat de samenwerking fragmentarisch wordt bij conflicten.
Idem bvb bij Linux Foundation etc.

De Foundation for Public Code hanteerde een vergelijkbaar perspectief – als Nederlandse codebases worden hergebruikt door Frankrijk, Duitsland en Italië, hoe zorgen we dat de belangen van één partij de samenwerking niet breken.
En tijdens de OpenZaak-marktconsultatie – zodat de open samenwerking tussen Maykin, de implementatiepartners, andere ontwikkelpartijen, allemaal met hun eigen belangen, kan worden gemedieerd vanuit een neutraal perspectief dat beslissingen neemt in het beste belang van de codebase, wat op zijn beurt ten goede komt aan iedereen (inclusief de gemeenten).  

### Codebase stewardship ‘landelijke voorziening’-variant

Bij landelijke regie en samen exploiteren geldt het bovenstaande niet direct voor de Common Ground-componenten, simpelweg omdat:  

* er één gecoördineerd opdrachtgeverschap is – governance vindt niet (alleen) op codebase-niveau plaats, maar op niveau van landelijke regie en componentportfolio  
* er een zeer nauwe afhankelijkheid tussen componenten is – ze staan of groeien niet zelfstandig 
* sommige componenten de implementatie van Nederlandse wet bevatten – territoriaal gebonden 
* gezien het bovenstaande is het onwaarschijnlijk dat een bedrijf spontaan zal komen en een businessmodel rond een component zal ontwikkelen (kan voor sommige componenten wel gebeuren)

Dit betekent dat de ‘landelijke voorziening’-variant van codebase-stewardship omvat:  

* collectief producteigenaarschap (behoeften/verzoeken/financiering verzamelen)  
* portfoliomanagement van componenten (afhankelijkheden, groeipaden, integratie)  
* release management (roadmaps, planning, breaking changes, etc.)  
* regie over het vendor-ecosysteem (samenwerking ontwikkelpartij, reviewpartij, onderhoudscontract en SaaS-aanbieder en alle contract- en relatiemanagement die daarbij hoort)
* de strategische belangrijkheid en volwassenheid van een component evalueren om te bepalen hoeveel redundantie en bedrijfszekerheid nodig is (bijv. een tweede leverancier)
* het realistische schaalbaarheids- en herbruikbaarheidspotentieel van de component beoordelen, evenals het realistische potentieel voor bijdragen door de community (wat beslissingen kan ondersteunen over hoe open issue-trackers, roadmaps, besluitvorming, enz. ingericht moeten worden.)

Voor sommige componenten kan
a) een paar marktpartijen direct diensten aan gemeenten willen aanbieden (bijvoorbeeld lokaal versnellen of een specifieke één-gemeente feature) of
b) een niet-gemeentelijke of internationale partij willen deelnemen.

In dat geval moet worden geëvalueerd of deelname aan de samenwerking voordelig is voor de codebase (meer mensen investeren erin) of juist een remmende factor is (meer complexiteit dan het waard is).
Dit zal per component/gemeenschap beoordeeld moeten worden.

In elk geval, als landelijke regie en samen exploiteren de uitgangspunten zijn, dan is de kernwaarde van codebase-stewardship (het beschermen van de belangen van de codebase onafhankelijk van één enkele partij) geen doel om op te optimaliseren.

Er is een duidelijke enkele partij - het belang van landelijke regie.

Er kan een deur open worden gelaten voor anderen om deel te nemen (bvb andere Nederlandse of buitenlandse overheidsinstellingen), in die mate dat het de moeite waard is om te bemiddelen tussen hun behoeften en die van de landelijke regieorganisatie – dan heeft ‘vanilla’ codebase-stewardship wel zin - en dan waarschijnlijk voor het platform als geheel, via de "Stichting Platform Zaakgericht Werken" of iets dergelijks, en niet op componentniveau.

### Centrale git-hosting platform?

Het lijkt nuttig dat er vanuit landelijke regie:

* een centrale plek is met een overzicht van alle componenten (en hun versies)  
* een manier is om dependencies tussen de componenten duidelijk te beschrijven  
* communicatie plaatsvindt naar implementatie/hostingpartners over breaking changes, releases, roadmaps, etc.  

Er lijkt dus een kans om een proof of concept te doen rond 'portfolio management van componenten in één git-hosting platform':
* daar de laatste stable release van alle componenten beschikbaar te hebben (voor nu als downstream clones)  
* en de oefening uit te voeren om dependencies tussen versies te beschrijven, te verkennen hoe communicatie naar hergebruikers zou kunnen verlopen

## Hoe beinvloed dit governance binnen OpenZaak

Dit betekent dat de governance binnen OpenZaak ook iets anders zal zijn dan bij een vanilla open source-project.

Zie [Verslag governance ecosysteem en rollen](verslag-ecosysteem-en-rollen)

