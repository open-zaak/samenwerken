---
layout: default
title: Stappen voor OpenZaak ecosysteem 
parent: Resultaten
nav_order: 6
---

# Stappen voor OpenZaak ecosysteem 

Status: Draft

Dit document bevat mogelijke beoogde stappen voor de OpenZaak ecosysteem, met de intentie op regie vanuit landelijke voorziening.

## Inhoudsopgave
* TOC
{:toc}

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
    Maint["Onderhoud partij (van stable releases)"]

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


## Rollen en taken per staat

