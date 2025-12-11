---
layout: default
---

# Verslag: OpenZaak Bedrijfszekerheidsdoelen

16/10/2025

Dit document bevat een beknopt voortgangsrapport over de OpenZaak-pilot.

Het omvat
1) context bij de pilot
2) een kort overzicht van de tot op heden verrichte werkzaamheden 
3) de geïdentificeerde bedrijfszekerheidsdoelstellingen waar verder op gewerkt wordt

## Inhoudsopgave
* TOC
{:toc}

## Context voor de pilot 

### Achtergrond

De G4-steden werken aan een reeks open source-componenten die kunnen worden gecombineerd tot een platform op basis van ‘zaakgericht werken’. Op termijn wil de G4 een professioneel en uniform kader definiëren voor het beheer/governance van deze open source-componenten.

Met dit doel voor ogen heeft de G4 een pilot gestart rondom OpenZaak, met nadruk op:
* Het governance/beheer van OpenZaak  
* Codereview-proces van bestaande en nieuwe bijdragen

De ambitie is om samen met de huidige gemeenschap het volgende te verfijnen en te documenteren:
* Het governance/beheer van OpenZaak (inclusief codebase gerelateerde standaarden, werkafspraken en best practices via bijvoorbeeld de governance file, contributor guidelines, enz.)  
* Het proces van codereview van bestaande en nieuwe bijdragen aan OpenZaak (inclusief het proces van codebase stewardship)  
* Het implementeren, testen en verbeteren van dit governance- en reviewproces in de praktijk   
* Duidelijk maken hoe het bovenstaande beheerd zal worden

Het is de ambitie om dit op een breed toepasbare manier te doen, en met een zodanige kwaliteitsniveau, zodat  gedocumenteerde werkmethoden en normen kunnen worden hergebruikt:
* Voor andere componenten  
* Door andere gemeenten of overheden  
* Door andere potentiële nieuwe leveranciers

Deze pilot richt zich niet op de centrale regie die in de toekomst zal worden ingericht, noch op de VNG-standaard, noch op de wijze waarop nieuwe leveranciers en gemeenten zich bij de samenwerking kunnen aansluiten.

## Uitgevoerde activiteiten

- 11 interviews met vertegenwoordigers van Utrecht, Den Haag, Rotterdam, VNG, Maykin, Worth en Ritense.  
- Analyse van huide documentatie rondom OpenZaak ter ondersteuning van de bevindingen.  
- Workshop gericht op governance doelen:  
  - het afstemmen over de huidige stand van zaken binnen het OpenZaak-ecosysteem,  
  - het in kaart brengen van sterktes, zwaktes, kansen en bedreigingen, en  
  - het opbouwen van een gedeeld begrip van de kern governancedynamieken binnen het ecosysteem

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
