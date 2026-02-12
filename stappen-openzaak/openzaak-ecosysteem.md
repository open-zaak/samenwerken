---
layout: default
title: OpenZaak ecosysteem
parent: Stappen
nav_order: 1
---

# OpenZaak ecosysteem

Dit document bevat inkooprichtlijnen voor OpenZaak, met met de intentie op regie vanuit landelijke voorziening.

## Inhoudsopgave
* TOC
{:toc}

##  Inleiding

Hieronder staan conceptteksten die gebruikt kunnen worden om OpenZaak onder de regie van landelijke voorziening te brengen.

## Ecosysteembeschrijvingen voor OpenZaak

Drie stappen voor het ecosysteem om volledige regie bij de landelijke voorziening te bereiken

### Huidige staat: een marktpartij die verantwoordelijk is

```mermaid
graph LR
    %% Nodes
    Dev1["Marktijpartij"]
    PO["Product owner:<br/>G4 en kopgroep"]

    %% Connections
    PO -.- Dev1 
```

### Tussen staat: landelijke regie verantwoordelijk voor de publicatie van stable releases, een marktpartij verantwoordelijk voor de development en onderhoud van de code, geassisteerd door een review partij

```mermaid
graph LR
    %% Nodes
    Dev1["Marktijpartij"]
    ReviewP2["Reviewpartij"]
    Upstream["Publicatie branch"]
    PO["Product owner:<br/>Landelijke regie"]

    %% Connections
    PO -.- Upstream
    Dev1 --> ReviewP2
    ReviewP2 --> Upstream
```

### Beoogde staat: volle regie vanuit landenlijke voorziening met mogelijkheid (indien gewenst) voor verschillende development, review, SaaS- en onderhoud-partijen 

```mermaid
graph LR
    %% Nodes
    Dev1["Marktijpartij"]
    ReviewP1["Reviewpartij"]
    Dev2["Marktijpartij"]
    Review2["Reviewpartij"]
    Upstream["Publicatie branch"]
    PO["Product owner:<br/>Landelijke regie"]
    SaaS["SaaS provider"]
    Maint["Onderhoud<br/>stable release"]

    %% Connections
    PO -.- Upstream
    Dev1 --> ReviewP1
    ReviewP1 --> Upstream
    Dev2 --> Review2
    Review2 --> Upstream
    Upstream --> Maint
    Maint --> Upstream
    Upstream --> SaaS
```

## Text op te nemen in contract en governance.md

De algemene voorwaarden van de GIBIT zijn van toepassing.

De algemene voorwaarden van de Common Ground-principes zijn van toepassing. Deze zijn te verkrijgen via [insert link].

De huidige staat van dit ecosysteem is te vinden in [repo/governance.md].

## Rollen en taken per staat


### Staat 1



### Staat 2



### Staat 3

