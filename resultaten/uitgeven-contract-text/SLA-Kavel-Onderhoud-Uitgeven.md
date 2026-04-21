---
layout: default
title: Voorbeeld SLA Kavel Uitgeven
parent: Uitgeven
nav_order: 4
---

## Inleiding

Aanpassingen aan `Voorbeeld SLA Kavel Beheren Broncode Versie 0.92`

## 1 Definities
Broncode uitgeven
Uitgven van broncode wordt als volgt gedefinieerd: het (langtermijn) beschikbaar maken van de broncode en bijhorende documentatie.

## 2.2 Open source
Open Formulieren is open source product. Om een open source product succesvol te gebruiken,
moet het product kwalitatief goed zijn en blijven. Hiervoor is uitgeven van broncode nodig. Dit wordt
gedaan door de uitgever. In deze SLA is aangegeven hoe de hoofdbeheerder hiervoor zorgt.

## 2.6 Documentatie
De leverancier borgt voor de qwaliteit van documentatie t.b.t. change logs, release dates, breaking changes, critical issues, patches versies, en installatie-, beheers, en gebruiks-handleiding. De documentatie is open source en wordt publiek aangeboden.

## 3.1. Uitgever
Uitgever zegt toe om:

```
Vanuit Informatieblad bijdragen voor broncodebeheer 2026:

2) zorg dragen voor de beschikbaarheid van de broncode en images (momenteel op Github en DockerHub),  
4) een openbare issue-tracker bijhouden die mogelijke bugs en suggesties van iedereen accepteert,  
10) relevante documentatie bijhouden en openbaar beschikbaar maken,  
11) community contributies aan de open source codebase verwelkomen,  
12) community contributies ("pull requests") monitoren op kwaliteit, veiligheid, herbruikbaarheid en architecturale fit,  
13) community contributie richtlijnen opstellen en onderhouden,  
14) zorg dragen dat alle bijdragen voldoen aan de licentievoorwaarden van de Europese Unie Publieke Licentie (EUPL) versie 1.2 of hoger,  
15) een versie controlemechanisme voor productcode onderhouden,  
16) versiebeheer toepassen (Productversies en ondersteuning),  
17) openbaar beschikbare release-notes bijhouden om o.a. gebruikers te helpen bij het upgraden,  
18) openbare mailinglijst bijhouden waarop gebruikers geïnformeerd worden over releases en relevant nieuws rondom het product,  
19) een compatibiliteitsmatrix bijhouden om devops- en implementatie-ontwikkelaars te ondersteunen bij hun werk,  
20) nieuwe gebruikers op weg helpen door gemakkelijk toegankelijke, eenvoudig te gebruiken voorbeelden beschikbaar hebben,  
22) actief meewerken om het product compliant te maken en houden met de relevante en toepasselijke standaarden,  
23) het 'VNG groeipact' onderschrijven en bijdragen bij aan verbeteringen van VNG-standaarden,  
25) inzetten om volledig compliant te zijn en blijven met de Standard for Public Code,  
26) indien van toepassing, de Applicatie TPM-verklaring beschikbaar te stellen aan Broncodebeheerpartner, en deze – indien nodig, tegen kosten – op naam te laten zetten.
```

```
Bijkomende:

* Communiceren van release dates, versiebeheer, breaking changes en critical issues naar relevante stakeholders (rg hosting- en implementatiepartijen)  
* Het archiveren van alle stabiele releases van de broncode en images, zodat eerdere versies beschikbaar blijven
* Zorgen voor uniforme inrichting van repositories, toegangsrechten en bijdrageprocessen in de centrale codevoorziening  
```

Verantwoordelijkheden

Uitgever zal:
1. het product en/of onderdelen daarvan niet vervangen, beëindigen of stopzetten, behalve
zoals uiteengezet in Bijlage (Ondersteuningsbeleid voor Versiebeheer van Open Source Soft-
ware ).
2. alles in het werk stellen, in het geval van licenties of rechten op Intellectueel Eigendom van
derden, Intellectuele Eigendomsrechten, Technologie of Open-Source Software, om derge-
lijke Rechten van Derden na te leven.
3. een formeel beveiligingsprogramma te gebruiken en maatregelen te treffen en te handha-
ven die zijn ontworpen om bedreigingen of veiligheidsrisico's, ongeoorloofd, onopzettelijk of
onwettig verlies van, toegang tot of openbaarmaking van gegevens die zijn opgeslagen in het
IB-product te beschermen en te voorkomen. Een dergelijk beveiligingsprogramma voldoet
aan ISO 27001 of een opvolger (indien van toepassing) dat substantieel gelijkwaardig is en
gevalideerd is door onafhankelijke auditors.
4. onmiddellijk eventuele beveiligings-, veiligheids-, gegevensbeschermings- of gegevenspriva-
cykwesties in het product aanpakken als zij zich bewust wordt van een dergelijk probleem en
de klant hiervan gelijktijdig op de hoogte stellen.
5. De Opdrachtgever begrijpt en stemt ermee in:
a. Hoofdbeheerder kan het product updaten, upgraden en onderhouden in de normale
gang van zaken door middel van releases zonder de functionaliteit en/of beveili-
gingsfuncties te verminderen. Als de release een ingrijpende wijziging veroorzaakt,
raadpleeg dan Bijlage (Ondersteuningsbeleid voor Versiebeheer van Open Source
Software) voor het relevante beleid hierin.
b. dat het product niet zal worden gebruikt voor de bediening en/of controle van of
gebruik binnen een High-Risk-systeem als de werking van een dergelijk High-Risk-
systeem afhankelijk is van het product.

```
?
c. dat zij het risico dragen van het selecteren van de juiste bedieningsmodus, beschik-
baarheid en beveiligingsopties voor het product, evenals de parametrisering, confi-
guratie en gebruik van dergelijke diensten in het product, tenzij anders overeenge-
komen tussen de partijen.
```

## 3.3 Kwaliteitscriteria

```
?
Voor broncode beheer zijn kwaliteitscriteria opgesteld. Broncode beheer dient te voldoen aan deze
kwaliteitscriteria. Hiervoor is een eerste opzet gemaakt. Zie bijlage “Basisset 1.0” 1, kolom ‘broncode
beheer’.

De eisen voor broncodebeheer zijn sterk afhankelijk van de opgeleverde software voor een product
(common ground component). De primaire verantwoordelijkheid voor het voldoen aan de non-functionals ligt grotendeels bij de initiële ontwikkelaar van software. De eisen zijn voor de
volledigheid wel aangegeven in de basisset.
```

Er vindt periodiek (tenminste één keer per kwartaal) een kwaliteitsgesprek plaats, met onder andere
als onderwerpen: sluit opdracht nog aan, hoe is de voortgang van de opdracht, hoe staat het ervoor
met kwaliteit van software etc.?