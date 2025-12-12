---
layout: default
---

# Introductie 

Status: Draft

De huidige OpenZaak community voorziet in de behoefte aan snel en informeel handelen.
Naarmate OpenZaak volwassen wordt en opschaalt, kan het karakter van de community veranderen.

Gezien de ambitie om van OpenZaak een kerncomponent te maken die op landelijk niveau onder centrale regie wordt geëxploiteerd, kunnen stappen worden gezet om de bedrijfszekerheid van de community te versterken.

Op basis van de interviews, workshops en bedrijfszekerheidsdoelen schetst onderstaand document een visie voor de community, de repo-structuur en de relaties tussen marktpartijen.

## Rollen & verantwoordelijkheden

### Ecosysteem/codebase steward

Het ophalen van problemen en wensen met betrekking tot de doorontwikkeling van de component en het coördineren van de doorontwikkeling op basis van de afgesproken governance, om de verschillende belangen in balans te houden, tussen aanbieders en afnemers, en tussen bijv. grote en kleine gemeenten, etc.

- Collectief product ownerschap met duidelijke roadmap  
- Portfolio management op alle componenten (en samenhang daartussen)  
- Regie over marktpartijen en samenwerking tussen marktpartijen
- Community managememt

### Beheer

Onderhoud van versies

- maintenance en bug fixes

### Uitgeven

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

### Reviewen

Controleren van de gepubliceerde versies van de component. Dit in het kader van vier ogen principe én warme kennis bij meer dan één partij.

- quality assurance
- audit (security, tests, documents, Q&A)
- works with feature development party 

### Development

Projectmatig ontwikkelen van een component of een feature van een component.

- new features
- works with review party
- aanbieden aan beheerder als pull request

### Implementeren

Het inrichten van de instantie van de component voor specifiek gebruik bij een gemeente, het trainen van medewerkers en het beantwoorden van vragen.
 
- local implementations, configuratie, training, helpdesk
- repots bugs, issues, needs
- optionally with local changes

### Leveren

Het leveren van een draaiende instantie van de component.

- SaaS
- repots bugs, issues, needs
- optionally with local changes


## Rollen & contracten

### Ecosysteem/codebase steward

Intern vanuit landelijke regie, of gedelegeerd 

### Beheer

Maintenance contract

### Uitgeven

Intern vanuit landelijke regie, of gedelegeerd

### Reviewen

Review contract

### Development

Feature development contract

### Implementeren

Implemetatie contract

### Leveren

SaaS contract

## Rollen, contracten en verantwoordelijkhedem

| Rollen                     | Verantwoordelijkheden                                                                                  | Contract type                          |
|-----------------------------|--------------------------------------------------------------------------------------------------------|----------------------------------------|
| Ecosysteem/codebase steward | - Collectief product ownerschap<br>- Portfolio management op alle componenten (en samenhang daartussen)<br>- Product release management met duidelijke roadmap, documentatie en release management | Intern vanuit landelijke regie, of gedelegeerd |
| Beheer                      | - Maintenance en bug fixes                                                                               | Maintenance contract                     |
| Uitgeven                    | - Upstream repository, (stable) releases van code, documentatie<br>- Publicatie en archief<br>- Change log, dependency graph, central issue en bug tracker<br>- Communicatie van release dates, breaking changes, critical issue | Intern vanuit landelijke regie, of gedelegeerd |
| Reviewen                    | - Quality assurance<br>- Audit (security, tests, documents, Q&A)<br>- Works with feature development party       | Review contract                          |
| Development                 | - New features<br>- Works with review party                                                                | Feature development contract             |
| Implementeren               | - Local implementations<br>- Repots bugs, issues, needs<br>- Optionally with local changes                       | Implementatie contract                   |
| Leveren                     | - SaaS<br>- Repots bugs, issues, needs<br>- Optionally with local changes                                       | SaaS contract                            |

## Voorbeeld repo structuur

```mermaid
graph LR
    %% Nodes
    Dev1["Repo:<br/>Dev branch"]
    Dev2["Repo:<br/>Dev branch"]
    SaaS["Repo:<br/>SaaS provider"]
    
    Upstream["Upstream repo: (VNG?)<br/>release branch &<br/>'release next'"]

    %% Connections
    Dev1 --> Upstream
    Dev2 --> Upstream
    Upstream --> SaaS
```

## Voorbeeld scenario: dual vendorship

```mermaid
graph LR
    %% Nodes
    
    %% Left Side: Inputs
    Dev1["Repo:<br/>Dev"]
    Dev2["Repo:<br/>Dev"]
    
    %% Top Stream (P1 works, P2 reviews)
    FeatP1["P1<br/>Feature<br/>branch"]
    ReviewP2["P2<br/>Review"]
    
    %% Bottom Stream (P2 works, P1 reviews)
    FeatP2["P2<br/>Feature<br/>branch"]
    ReviewP1["P1<br/>Review"]

    %% Center: Upstream & Management
    Upstream["Upstream<br/>repo: (VNG?)<br/>release branch &<br/>'release next'"]
    PO["Product<br/>owner (versie<br/>beheer: planning<br/>en acceptatie)"]

    %% Right Side: Outputs / Maintenance
    MaintP1["P1<br/>Onderhoud<br/>even major<br/>release"]
    MaintP2["P2<br/>Onderhoud<br/>oneven major<br/>release"]
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

## Stappenplan voor de introductie van een tweede marktpartij

0. Contract voor "close easy issue"  
1. Review contract  
2. Maintenance contract  
3. Feature development contract  

## Voorbeeld scenario: marktpartijen met elk 1 development en 1 review verantwoordelijkheid

```mermaid
graph LR
    %% Nodes
    
    %% Left Side: Components
    Dev1["Component 1:<br/>Dev repo"]
    Dev2["Component 2:<br/>Dev repo"]
    Dev3["Component 3:<br/>Dev repo"]

    %% Reviews
    1FeatP1["Partij1<br/>Feature<br/>branch"]
    1ReviewP2["Partij2<br/>Review"]

    2FeatP2["Partij2<br/>Feature<br/>branch"]
    2ReviewP3["Partij3<br/>Review"]

    3FeatP3["Partij3<br/>Feature<br/>branch"]
    3ReviewP1["Partij1<br/>Review"]

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

