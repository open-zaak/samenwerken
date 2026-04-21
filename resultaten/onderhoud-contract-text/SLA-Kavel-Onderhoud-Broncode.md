---
layout: default
title: Voorbeeld SLA Kavel Onderhoud
parent: Onderhoud
nav_order: 4
---

## Inleiding

Aanpassingen aan `Voorbeeld SLA Kavel Beheren Broncode Versie 0.92`

## 1 Definities

Broncode onderhoud

Beheer van broncode wordt als volgt gedefinieerd: onderhoud van broncode, gericht op de technische gezondheid, veiligheid en stabiliteit van (bepaalde releases van) de code, documentatie en tests.

## 2.2 Open source
`naam applicatie` is een open source product. Om een open source product succesvol te gebruiken,
moet het product kwalitatief goed zijn en blijven. Hiervoor is onderhoud van broncode nodig. Dit wordt
gedaan door de onderhouder. In deze SLA is aangegeven hoe de onderhouder hiervoor zorgt.

## 2.6 Documentatie
De leverancier biedt actuele documentatie t.b.t. veiligheid, tests, lifecycle van ondersteunde releases, communicatie van beveiligingskwetsbaarheden en bugs, en het beheren van afhankelijkheden en licentie-compliance aan. De documentatie is open source en wordt publiek aangeboden.

## 3.1. Onderhouder 
Onderhouder zegt toe om:

```
Vanuit Informatieblad bijdragen voor broncodebeheer 2026:

3) minimaal dagelijks image en code beveiligingsscans uitvoeren en bevindingen oplossen,  
5) een responsible disclosure programma onderhouden, inclusief een e-mailadres voor beveiligingsproblemen,  
6) CVE's publiceren voor gevalideerde beveiligingsproblemen,  
7) gerapporteerde bugs valideren en beoordelen op prioriteit,  
8) gevalideerde en geprioriteerde bugs oplossen in patch-releases,  
9) koppelingen compatible houden met patches en minor versiewijzigingen in het betreffende koppelvlak (major versiewijzigingen vallen expliciet onder doorontwikkeling),  
19) streven naar backwards compatibiliteit in kleine releases en daarmee installatie/implementatie-upgrades vereenvoudigen,  
21) geschikte Helm charts publiceren voor het product,  
22) een CI pipeline onderhouden inclusief geautomatiseerde testen met een testcoverage van 80% of hoger, teneinde de kwaliteit te waarborgen,  
24) gebruikte componenten van derden ('afhankelijkheden' of 'software bibliotheken') bijhouden, beoordelen op kwaliteit, veiligheid, volwassenheid en naleving van de open source-licenties,  
25) zorg dragen voor compatibiliteit met de meest recente, grote, browsers,
```

```
Bijkomend:

* De codebase (of nieuwe stable releases daarvan) beoordelen op beheerbaarheid, onderhoudbaarheid en overdraagbaarheid voordat structureel onderhoud wordt aanvaard,
* Monitoren van afgesproken aantal stable releases op bugs, security en performance issues
* Documentatie bijhouden over lifecycle-keuzes, migraties en end-of-life trajecten,  
* Documenteren van van onderhoudsactiviteiten voor relevante stakeholders
```

Hoofdbeheerder zal:  
1. het product en/of onderdelen daarvan niet vervangen, beëindigen of stopzetten, behalve zoals uiteengezet in Bijlage (Ondersteuningsbeleid voor Versiebeheer van Open Source Software  ).  
2. alles in het werk stellen, in het geval van licenties of rechten op Intellectueel Eigendom van derden, Intellectuele Eigendomsrechten, Technologie of Open-Source Software, om dergelijke Rechten van Derden na te leven.  
3. een formeel beveiligingsprogramma te gebruiken en maatregelen te treffen en te handhaven die zijn ontworpen om bedreigingen of veiligheidsrisico's, ongeoorloofd, onopzettelijk of onwettig verlies van, toegang tot of openbaarmaking van gegevens die zijn opgeslagen in het IB-product te beschermen en te voorkomen. Een dergelijk beveiligingsprogramma voldoet aan ISO 27001 of een opvolger (indien van toepassing) dat substantieel gelijkwaardig is en gevalideerd is door onafhankelijke auditors.  
4. onmiddellijk eventuele beveiligings-, veiligheids-, gegevensbeschermings- of gegevensprivacykwesties in het product aanpakken als zij zich bewust wordt van een dergelijk probleem en de klant hiervan gelijktijdig op de hoogte stellen.  
5. De Opdrachtgever begrijpt en stemt ermee in:
        a. dat het product niet zal worden gebruikt voor de bediening en/of controle van of gebruik binnen een High-Risk-systeem als de werking van een dergelijk High-Risk-systeem afhankelijk is van het product. 
```
?
        b. dat zij het risico dragen van het selecteren van de juiste bedieningsmodus, beschikbaarheid en beveiligingsopties voor het product, evenals de parametrisering, configuratie en gebruik van dergelijke diensten in het product, tenzij anders overeengekomen tussen de partijen.
```

## 3.2 Onderhouden
Binnen de overeenkomst vallen de volgende diensten:  
1. Correctief onderhoud: Het oplossen van gemelde problemen met een of meer van de geleverde diensten.   
2. Preventief onderhoud: Aanpassen en/of bijwerken van de geleverde diensten in het geval er beveiligingsupdates beschikbaar zijn voor deze software en/of afhankelijke componenten.  

Het onderhoud omvat de meest recente (stable) versie van de broncode en de 1-na-laatste versie van de broncode. 

## 3.3 Kwaliteitscriteria

```
?
Voor broncode onderhoud zijn kwaliteitscriteria opgesteld. Broncode beheer dient te voldoen aan deze kwaliteitscriteria. Hiervoor is een eerste opzet gemaakt. Zie bijlage “Basisset 1.0”1, kolom ‘broncode beheer’. 

De eisen voor broncode onderhoud zijn sterk afhankelijk van de opgeleverde software voor een product (common ground component). De primaire verantwoordelijkheid voor het voldoen aan de non-functionals ligt grotendeels bij de initiële ontwikkelaar van software. De eisen zijn voor de volledigheid wel aangegeven in de basisset.

Er vindt periodiek (tenminste één keer per kwartaal) een kwaliteitsgesprek plaats, met onder andere als onderwerpen: sluit opdracht nog aan, hoe is de voortgang van de opdracht, hoe staat het ervoor met kwaliteit van software etc.?
```

(Niet van toepassing: `Bijlage: Ondersteuningsbeleid voor Versiebeheer van Open Source Software`)