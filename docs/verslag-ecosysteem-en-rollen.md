---
layout: default
---

## Inhoudsopgave
* TOC
{:toc}

## Rollen & verantwoordelijkheden 

### Ecosysteem/codebase steward

- Collectief product ownerschap  
- Portfolio management op alle componenten (en samenhang daartussen)  
- Product release management met duideljike roadmap, documentatie en release management

### Beheer

- maintenance en bug fixes

### Uitgeven

- upstream repository, (stable) releaes van code, documentatie
- publicatie en archief 
- change log, dependency graph, central issue en bug tracker 
- communicatie van release dates, breaking changes, critical issue

### Reviewen

- quality assurance
- audit (security, tests, documents, Q&A)
- works with feature development party 

### Development

- new features
- works with review party 

### Implementeren

- local implementations
- repots bugs, issues, needs
- optionally with local changes

### Leveren

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

## Repo structure

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

## Dual vendorship

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

## Marktpartijen 


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
