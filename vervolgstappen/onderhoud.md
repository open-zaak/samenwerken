---
layout: default
title: Onderhoud
parent: Vervolgstappen
nav_order: 5
---

# Onderhoud

## Beschrijving

Als onderhouder ben je verantwoordelijk voor de technische gezondheid en stabiliteit van (bepaalde releases van) de code, documentatie en tests.

Je werkt transparant en in het openbaar: open CI-pipelines, publieke CVE-publicaties en een actief responsible disclosure-programma zijn niet alleen technische instrumenten, maar ook signalen van betrouwbaarheid.

Je werkt samen met de uitgever om de onderhoudbaarheid van nieuwe (stable) releases te beoordelen, eer je er verantwoordelijkheid voor neemt.

Je overziet:
* het continu monitoren en oplossen van beveiligingskwetsbaarheden en bugs
* het beheren van afhankelijkheden
* de CI/CD-pipeline en geautomatiseerde testsuite
* de lifecycle van ondersteunde releases, inclusief migratie- en end-of-life trajecten
* de communicatie van beveiligingsbevindingen via responsible disclosure en CVE-publicaties
* de licentie-compliance van afhankelijkheden 

Je bent niet verantwoordelijk voor nieuwe functionaliteit of architecturale keuzes — dat valt onder doorontwikkeling.

Je draagt wel zorg voor de overdraagbaarheid en beheerbaarheid van de codebase, en je documenteert je werkzaamheden zodat andere partijen hierop kunnen vertrouwen.

## Werkafspraken (voorbeeld) 

Vanuit Informatieblad bijdragen voor broncodebeheer 2026:

```
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

Bijkomende:

```
* De codebase (of nieuwe stable releases daarvan) beoordelen op beheerbaarheid, onderhoudbaarheid en overdraagbaarheid voordat structureel onderhoud wordt aanvaard,
* Monitoren van afgesproken aantal stable releases op bugs, security en performance issues
* Documentatie bijhouden over lifecycle-keuzes, migraties en end-of-life trajecten,  
* Documenteren van van onderhoudsactiviteiten voor relevante stakeholders
```