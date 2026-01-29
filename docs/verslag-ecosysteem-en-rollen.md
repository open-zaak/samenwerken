---
layout: default
title: 4) Verslag governance, ecosysteem en rollen
nav_order: 4
---

# Verslag: Governance, Ecosysteem en Rollen


Dit document schetst een visie voor de community, de repo-structuur en de relaties tussen marktpartijen, op basis van de interviews, workshops en bedrijfszekerheidsdoelen.

## Inhoudsopgave
* TOC
{:toc}

## Context: huidige governance- en werkafspraken

De huidige OpenZaak community werkt goed voor snel en informeel werken.

Er is veel informele samenwerking binnen de community, inclusief documentatie met een informeel karakter. 
De G4 vervult een aansturende rol.
Er is veel goodwill en de meeste betrokken partijen zijn tevreden.

Naarmate OpenZaak groeit en breder wordt ingezet, kan de community veranderen.

Gezien de ambitie om van OpenZaak een kerncomponent te maken die op landelijk niveau onder centrale regie wordt geëxploiteerd, kunnen stappen worden gezet om de bedrijfszekerheid van de community te versterken.

## Voorstel: rollen & verantwoordelijkheden

### Ecosysteem/codebase steward

Nu: G4 overleg

Toekomst: Intern vanuit landelijke regie, of gedelegeerd 

#### Rol

Het ophalen van problemen en wensen met betrekking tot de doorontwikkeling van de component en het coördineren van de doorontwikkeling op basis van de afgesproken governance, om de verschillende belangen in balans te houden, tussen aanbieders en afnemers, en tussen bijv. grote en kleine gemeenten, etc.

- Collectief product ownerschap met duidelijke roadmap  
- Portfolio management op alle componenten (en samenhang daartussen)  
- Regie over marktpartijen en samenwerking tussen marktpartijen
- Community managememt

#### Waarom? (design choices)

*  Dit is een landschap met meerdere componenten, dus er moet vanuit landelijke regie toezicht zijn op de onderlinge afhankelijkheden tussen de verschillende componented.

```mermaid
graph LR
    %% Nodes
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Connections
    PO
```

### Uitgeven

Nu: Maykin

Toekomst: Intern vanuit landelijke regie, of gedelegeerd

#### Rol

Langetermijn beschikbaar stellen van component(versies).
Op orde en compliant houden van de opensourcecode van de component(versies).

- Product release management met documentatie 
- upstream repository, (stable) releaes van code, documentatie
- publicatie en archief 
- change log, dependency graph, central issue en bug tracker 
- communicatie van release dates, breaking changes, critical issue
- acceptatie van feature pull request
- installatiehandleiding
- beheershandleiding
- gebruikshandleiding
- regelmatige publicatie van versies

#### Waarom? (design choices)

*  Een centrale repository, in eigendom en beheer van de landelijke regie, met alle (stabiele) versies van alle componenten, maakt beter toezicht en betere regie mogelijk.

```mermaid
graph LR
    %% Nodes
    Upstream["Upstream repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Connections
    PO -.- Upstream
```

### Development

Nu: Maykin

Toekmost: Mogelijk tweede marktpartij met een feature development contract, indien nodig/gewenst

#### Rol

Projectmatig ontwikkelen van een component of een feature van een component.

- new features
- works with review party
- aanbieden aan beheerder als pull request

#### Waarom?

*  Levering aan de centrale repository, onder toezicht van de steward, maakt een duidelijke definitie van “done” en het beheer van features/versies mogelijk.

```mermaid
graph LR
    %% Nodes
    Dev1["Repo:<br/>Dev branch"]
    Upstream["Upstream repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Connections
    PO -.- Upstream
    Dev1 --> Upstream
```

### Reviewen

Nu: Maykin

Toekmost: Mogelijk tweede marktpartij met een review contract

#### Rol

Controleren van de gepubliceerde versies van de component.
Dit in het kader van vier ogen principe én warme kennis bij meer dan één partij.

- quality assurance
- audit (security, tests, documents, Q&A)
- works with feature development party 

#### Waarom?

*  De introductie van een tweede beoordelingspartij zorgt voor meer veerkracht in het ecosysteem, waarbij een tweede partij over warme kennis van de codebase beschikt.

```mermaid
graph LR
    %% Nodes
    Dev1["Repo:<br/>Dev"]
    FeatP1["Partij 1<br/>Feature<br/>branch"]
    ReviewP2["Partij 2<br/>Review"]
    Upstream["Upstream<br/>repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Connections
    
    %% PO Logic (dotted line for oversight)
    PO -.- Upstream

    %% Workflow 1
    Dev1 --> FeatP1
    FeatP1 --> ReviewP2
    ReviewP2 --> Upstream
```

### Beheer/maintenance

Nu: Maykin, als onderdeel van een featurecontract

Toekomst: Maykin met een specifiek onderhoudscontract, mogelijk tweede marktpartij met een specifiek onderhoudscontract

#### Rol

Onderhoud van versies

- maintenance en bug fixes

#### Waarom?

*  Indien gewenst, zou de tweede beoordelingspartij op termijn ook het beheer van de codebase kunnen doen (bijvoorbeeld bij elke andere stabiele release) om zo nog meer kennis van de codebase op te bouwen en daarmee redundantie te waarborgen.

```mermaid
graph LR
    %% Nodes
    Dev1["Repo:<br/>Dev"]
    FeatP1["Partij 1<br/>Feature<br/>branch"]
    ReviewP2["Partij 2<br/>Review"]
    Upstream["Upstream<br/>repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]
    Maint["Onderhoud<br/>stable release"]

    %% Connections
    
    %% PO Logic (dotted line for oversight)
    PO -.- Upstream

    %% Workflow 1
    Dev1 --> FeatP1
    FeatP1 --> ReviewP2
    ReviewP2 --> Upstream
    Upstream --> Maint
```

### Leveren

Nu: Verschillende SaaS aanbieders

Toekmost: SaaS aanbieder onder landelijke regie

#### Rol

Het leveren van een draaiende instantie van de component.

- SaaS
- repots bugs, issues, needs
- optionally with local changes

#### Waarom?

* Een aparte SaaS-aanbieder om de kwaliteit van de codebase, de uitvoerbaarheid door andere partijen, en daarmee de veerkracht van het ecosysteem te waarborgen.

```mermaid
graph LR
    %% Nodes
    Dev1["Repo:<br/>Dev"]
    FeatP1["Partij 1<br/>Feature<br/>branch"]
    ReviewP2["Partij 2<br/>Review"]
    Upstream["Upstream<br/>repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]
    Maint["Onderhoud<br/>stable release"]
    SaaS["Repo:<br/>SaaS provider"]

    %% Connections
    PO -.- Upstream
    Dev1 --> FeatP1
    FeatP1 --> ReviewP2
    ReviewP2 --> Upstream
    Upstream --> Maint
    Upstream --> SaaS
```

### Implementeren

#### Rol

Het inrichten van de instantie van de component voor specifiek gebruik bij een gemeente, het trainen van medewerkers en het beantwoorden van vragen.
 
- local implementations, configuratie, training, helpdesk
- repots bugs, issues, needs
- optionally with local changes
    
## Voorbeeld scenario: marktpartijen met elk 1 development en 1 review verantwoordelijkheid

Doel: meerdere ontwikkelpartijen laten bijdragen aan een landelijke regie-repository, waarbij elke partij verantwoordelijk is voor de ontwikkeling van één component en de review van één component.

```mermaid
graph LR
    %% Nodes
    
    %% Left Side: Components
    Dev1["Component 1:<br/>Dev repo"]
    Dev2["Component 2:<br/>Dev repo"]
    Dev3["Component 3:<br/>Dev repo"]

    %% Reviews
    1FeatP1["Partij 1<br/>Feature<br/>branch"]
    1ReviewP2["Partij 2<br/>Review"]

    2FeatP2["Partij 2<br/>Feature<br/>branch"]
    2ReviewP3["Partij 3<br/>Review"]

    3FeatP3["Partij 3<br/>Feature<br/>branch"]
    3ReviewP1["Partij 1<br/>Review"]

    %% Center: Upstream & Management
    Upstream["Upstream<br/>repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Right Side: SaaS
    SaaS["Repo:<br/>SaaS<br/>provider"]

    %% Connections
    
    %% PO Logic (dotted line for oversight)
    PO -.- Upstream

    %% Component 1
    Dev1 --> 1FeatP1
    1FeatP1 --> 1ReviewP2
    1ReviewP2 --> Upstream

    %% Component 2
    Dev2 --> 2FeatP2
    2FeatP2 --> 2ReviewP3
    2ReviewP3 --> Upstream

    %% Component 3
    Dev3 --> 3FeatP3
    3FeatP3 --> 3ReviewP1
    3ReviewP1 --> Upstream

    %% Downstream / Release
    Upstream --> SaaS
```

## Voorbeeld scenario: dual vendorship

Doel: twee ontwikkelpartijen laten samenwerken om elkaars werk te ontwikkelen en te reviewen.

```mermaid
graph LR
    %% Nodes
    
    %% Left Side: Inputs
    Dev1["Repo:<br/>Dev"]
    Dev2["Repo:<br/>Dev"]
    
    %% Top Stream (P1 works, P2 reviews)
    FeatP1["Partij 1<br/>Feature<br/>branch"]
    ReviewP2["Partij 2<br/>Review"]
    
    %% Bottom Stream (P2 works, P1 reviews)
    FeatP2["Partij 2<br/>Feature<br/>branch"]
    ReviewP1["Partij 1<br/>Review"]

    %% Center: Upstream & Management
    Upstream["Upstream<br/>repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Right Side: Outputs / Maintenance
    MaintP1["Partij 1<br/>Onderhoud<br/>even major<br/>release"]
    MaintP2["Partij 2<br/>Onderhoud<br/>oneven major<br/>release"]
    SaaS["Repo:<br/>SaaS<br/>provider"]

    %% Connections
    
    %% PO Logic (dotted line for oversight)
    PO -.- Upstream

    %% Workflow 1
    Dev1 --> FeatP1
    FeatP1 --> ReviewP2
    ReviewP2 --> Upstream
    
    %% Workflow 2
    Dev2 --> FeatP2
    FeatP2 --> ReviewP1
    ReviewP1 --> Upstream

    %% Downstream / Release
    Upstream --> MaintP1
    Upstream --> MaintP2
    Upstream --> SaaS
```

### Stappenplan voor de introductie van een tweede marktpartij

0. Contract voor "close easy issue": de codebase en documentatie leren kennen  
1. Reviewcontract: een diepgaander begrip van de codebase krijgen en gecoacht worden door de hoofdontwikkelende partij  
2. maintenance contract: verantwoordelijkheid nemen voor de codebase door een stabiele release te onderhouden  
3. Feature-ontwikkelcontract: deelnemen aan de ontwikkeling van de codebase

```

## Rollen, contracten en verantwoordelijkhedem

> ! table to be updated once the above is finalised

| Rollen                     | Verantwoordelijkheden                                                                                  | Contract type                          |
|-----------------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------|
| Ecosysteem/codebase steward | - Collectief product ownerschap<br>- Portfolio management op alle componenten (en samenhang daartussen)<br>- Product release management met duidelijke roadmap, documentatie en release management | Intern vanuit landelijke regie, of gedelegeerd |
| Beheer                      | - Maintenance en bug fixes                                                                               | Maintenance contract                     |
| Uitgeven                    | - Upstream repository, (stable) releases van code, documentatie<br>- Publicatie en archief<br>- Change log, dependency graph, central issue en bug tracker<br>- Communicatie van release dates, breaking changes, critical issue | Intern vanuit landelijke regie, of gedelegeerd |
| Reviewen                    | - Quality assurance<br>- Audit (security, tests, documents, Q&A)<br>- Works with feature development party       | Review contract                          |
| Development                 | - New features<br>- Works with review party                                                                | Feature development contract             |
| Implementeren               | - Local implementations<br>- Repots bugs, issues, needs<br>- Optionally with local changes                       | Implementatie contract                   |
| Leveren                     | - SaaS<br>- Repots bugs, issues, needs<br>- Optionally with local changes                                       | SaaS contract                            |

```