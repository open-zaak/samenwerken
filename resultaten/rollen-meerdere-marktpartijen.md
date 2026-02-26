---
layout: default
title: Rollen voor meerdere marktpartijen
parent: Resultaten
nav_order: 3
---

# Rollen voor meerdere marktpartijen

Op basis van de interviews, workshops en bedrijfszekerheidsdoelen, schetst dit document een visie voor de community, de repository-structuur en de relaties tussen marktpartijen.

Het doel is om voor te bereiden dat meerdere marktpartijen kunnen bijdragen, indien en wanneer dit gewenst of vereist is door de G4 en/of landelijke regie.

Daarbij is het belangrijk om op te merken dat OpenZaak niet op zichzelf staat, maar onderdeel is van het Common Ground landschap van componenten én partijen. De regiepartij heeft een belangrijke rol in het bewaken van de planning van en samenhang tussen deze componenten en het over en weer inzetten van partijen die aan meerdere componenten bijdragen.

```mermaid
graph LR
    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management in samenhang"]
    Impl["Implementatiepartij implementeert oplossing bij gemeente"]
    subgraph CommonGround["Common Ground"]
        %% Nodes
        Comp1["Component 1 codebase en ecosysteem"]
        Comp2["Component 2 codebase en ecosysteem"]
        Comp3["Component 3 codebase en ecosysteem"]
        More["..."]

        classDef ellipsis fill:#ffffff,stroke-dasharray: 5 5,color:#666;
        class More ellipsis
    end

    %% Connections
    Regie --> Comp1
    Regie --> Comp2
    Regie --> Comp3
    Regie --> More
    Comp1 --> Impl
    Comp2 --> Impl
    Comp3 --> Impl
    More --> Impl
```

## Inhoudsopgave
* TOC
{:toc}

## Inleiding: huidige governance- en werkafspraken

De huidige OpenZaak community werkt goed voor snel en informeel werken.

Er is veel informele samenwerking binnen de community, inclusief documentatie met een informeel karakter.
Rollen en verantwoordelijkheden zijn niet altijd duidelijk belegd en meerdere rollen worden door dezelfde partij vervuld, waardoor het niet altijd duidelijk is welke activiteiten en beslissingen onder welke rol vallen.
De G4 vervult een aansturende rol.
Er is veel goodwill en de meeste betrokken partijen zijn tevreden.

Naarmate OpenZaak groeit en breder wordt ingezet, kan de community veranderen.

Gezien de ambitie om van OpenZaak een kerncomponent te maken die op landelijk niveau onder centrale regie wordt geëxploiteerd, kunnen stappen worden gezet om de bedrijfszekerheid van de community te versterken.

## Voorstel: rollen & verantwoordelijkheden

Uit de gesprekken komen een aantal rollen naar voren die we van elkaar kunnen scheiden, om deze in een later stadium aan verschillende marktpartijen te kunnen toewijzen, indien gewenst of vereist, te weten:
- Regiepartij (voorheen Ecosysteem/codebase steward),
- Ontwikkelpartij (voorheen Development),
- Reviewpartij (voorheen Reviewen),
- Uitgever,
- Onderhoudspartij (voorheen Maintenance/onderhoud),
- SaaS aanbieder (voorheen Leveren (SaaS)),
- Implementatiepartij (voorheen Implementeren).

```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl
```

Hieronder lichten we per rol toe wat de rol inhoudt, welke taken daarbij horen, en waarom we deze rol gescheiden hebben van andere rollen.

---

### Regiepartij

Nu: G4 overleg

Toekomst: Intern vanuit landelijke regie, of gedelegeerd

```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Dev,Rev,Up,Maint,SaaS,Impl,OpenZaak grey;
```

#### Rolbeschrijving

Het ophalen van problemen en wensen met betrekking tot de doorontwikkeling van de component en het coördineren van de doorontwikkeling op basis van de afgesproken governance, om de verschillende belangen in balans te houden: tussen aanbieders en afnemers, en tussen bijv. grote en kleine gemeenten, etc.

#### Taken

- Collectief product ownerschap met duidelijke roadmap, doel & scope, architectuurprincipes, standaarden, lifecycle and compatibility etc.
- Portfolio management over alle componenten heen, inclusief samenhang en configuratie tussen versies daarvan.
- Regie over marktpartijen en samenwerking tussen marktpartijen.
- Community management, inclusief open-source governance, bijdrageprocessen, besluitvorming, rolzuiverheid, kenniscontinuïteit en bedrijfszekerheid.
- Ecosysteem management, inclusief afweging tussen stabiliteit, innovatie, onafhankelijkheid en beheerkosten.
- Financiering en opdrachtgeverschap.

#### Overwegingen

*  Dit is een landschap met meerdere componenten, dus er moet vanuit landelijke regie toezicht zijn op de onderlinge afhankelijkheden tussen de verschillende componenten.

---

### Uitgever

Nu: Maykin

Toekomst: Intern vanuit landelijke regie, of gedelegeerd


```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Dev,Regie,Rev,Maint,SaaS,Impl,OpenZaak grey;
```

#### Rolbeschrijving

Langetermijn beschikbaar stellen van component(versies).
Op orde en compliant houden van de opensourcecode van de component(versies).

#### Taken

- Upstream repository met publicatie en archief van alle (stable) releases van code
- Central issue en bug tracker, acceptatie van feature pull request   
- Product release management met documentatie
  - communicatie van release dates, breaking changes, critical issues
  - change log, dependency graph
  - installatie-, beheers, en gebruiks-handleiding

#### Overwegingen

*  Een centrale repository, in eigendom en beheer van de landelijke regie, met alle (stabiele) versies van alle componenten, maakt beter toezicht en betere regie mogelijk.
*  Dit vereist dat de landelijke regie hiervoor verantwoordelijkheid neemt en over de relevante expertise beschikt of deze inhuurt.

---

### Ontwikkelpartij

Nu: Maykin

Toekomst: Mogelijk tweede marktpartij met een feature development contract, indien nodig/gewenst

```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Regie,Rev,Up,Maint,SaaS,Impl,OpenZaak grey;
```

#### Rolbeschrijving

Projectmatig ontwikkelen van een component of een feature van een component.

#### Taken

- Code contributies (new features of patches) met alle bijhorende documentatie en tests 
- Aanbieden aan beheerder als pull request
- Werkt mogelijk samen met een review party

#### Overwegingen

*  Levering aan de centrale repository, onder toezicht van de steward, maakt een duidelijke definitie van “done” en het beheer van features/versies mogelijk.
*  Dit kan enige complexiteit in het ontwikkelproces introduceren, waardoor enkele iteraties in de workflow nodig zijn.

---

### Reviewpartij

Nu: Maykin

Toekomst: Mogelijk tweede marktpartij met een review contract


```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Dev,Regie,Up,Maint,SaaS,Impl,OpenZaak grey;
```

#### Rolbeschrijving

Samenwerken met de development partij door contributies naar de publicatie repo te reviewen. 
Dit in het kader van vier ogen principe én warme kennis bij meer dan één partij.

#### Taken

- Onafhankelijke review (code, security, documentatie, herbruikbaarheid, etc)

#### Overwegingen

*  De introductie van een tweede reviewpartij zorgt voor meer veerkracht in het ecosysteem, waarbij een tweede partij over warme kennis van de codebase beschikt.
*  Dit zal extra kosten en vertraging in de workflow introduceren, in verhouding tot de ambitie, diepgang en kwaliteit van de review. Dit moet een bewuste keuze zijn.

---

### Onderhoudspartij

Nu: Maykin, als onderdeel van een featurecontract

Toekomst: Maykin met een specifiek onderhoudscontract, mogelijk tweede marktpartij met een specifiek onderhoudscontract


```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Dev,Regie,Rev,Up,SaaS,Impl,OpenZaak grey;
```

#### Rolbeschrijving

Onderhoud van een of meerdere stable release versies van de code, inclusief bug fixes, updates en security patches. 

#### Taken

- Monitoren van stable releases op bugs, security en performance issues.
- Uitvoeren van bug fixes, updates en security patches.
- Communiceren van onderhoudsactiviteiten naar relevante stakeholders.

#### Overwegingen

*  Indien gewenst, zou de tweede onderhoudspartij op termijn ook het beheer van de codebase kunnen doen (bijvoorbeeld bij elke andere stabiele release) om zo nog meer kennis van de codebase op te bouwen. Dit ambitieniveau is op dit moment nog niet aan de orde.

---

### SaaS aanbieder

Nu: Verschillende SaaS aanbieders

Toekomst: centrale SaaS aanbieder onder landelijke regie


```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Dev,Regie,Rev,Up,Maint,Impl,OpenZaak grey;
```

#### Rolbeschrijving

Het leveren van stable versie(s) uit de publicatie repositorie als een draaiende instantie van de component.

#### Taken

- Levert eindproducten als SaaS-dienst.
- Verantwoordelijkheid voor performance, schaalbaarheid, capaciteit van de diensten.
- Monitoring, incidentmanagement, back-ups, herstel en dagelijkse operationele beveiliging.
- Inbrengen bugs, issues, requirements terug naar de centrale issue tracker.

#### Overwegingen

* Een aparte SaaS-aanbieder om de kwaliteit van de codebase, de uitvoerbaarheid door andere partijen, en daarmee de veerkracht van het ecosysteem te waarborgen.

---

### Implementatiepartij

```mermaid
graph LR
    subgraph OpenZaak
    %% Nodes
        Dev["Ontwikkelpartij ontwikkelt feature in eigen repo"]
        Rev["Review partij reviewt feature branch in upstream repo"]
        Up["Uitgever beheert versie branches in upstream repo"]
        Maint["Onderhoudspartij onderhoudt stable release branches in upstream repo"]
        SaaS["SaaS aanbieder levert draaiende instantie (vanuit eigen repo)"]

        %% Connections
        Dev --"push naar feature branch"--> Rev
        Rev --> Up
        Maint --> Up
        Up --> SaaS
    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]

    %% Connections
    Regie --> OpenZaak
    OpenZaak --> Impl

    %% Styling
    classDef grey fill:#eeeeee,stroke:#bbbbbb,color:#777777;
    class Dev,Regie,Rev,Up,Maint,SaaS,OpenZaak grey;
```

#### Rolbeschrijving

Het inrichten van de instantie van de component voor specifiek gebruik bij een gemeente, het trainen van medewerkers en het beantwoorden van vragen.

#### Taken
 
- Aanpassen van werkprocessen, configuraties en werkwijzen zodat de SaaS-diensten aansluiten op de dagelijkse praktijk.
- Brengen ervaringen, knelpunten en behoeften van gebruikers terug naar het ecosysteem ter verbetering van productdefinitie, adoptie en dienstverlening.

## Voorstelvisie ecosysteem van componenten

```mermaid
graph LR
    subgraph Component1
    %% Nodes
        Dev1["Ontwikkelpartij A ontwikkelt feature in eigen repo"]
        Rev1["Ontwikkelpartij C reviewt feature branch in upstream repo"]
        Maint1["Onderhoudspartij onderhoudt stable release branches in upstream repo"]

        %% Connections
        Dev1 --"push naar feature branch"--> Rev1
    end

    subgraph Component2
    %% Nodes
        Dev2["Ontwikkelpartij B ontwikkelt feature in eigen repo"]
        Rev2["Ontwikkelpartij A reviewt feature branch in upstream repo"]
        Maint2["Onderhoudspartij onderhoudt stable release branches in upstream repo"]

        %% Connections
        Dev2 --"push naar feature branch"--> Rev2
    end

    subgraph Component3
    %% Nodes
        Dev3["Ontwikkelpartij C ontwikkelt feature in eigen repo"]
        Rev3["Ontwikkelpartij B reviewt feature branch in upstream repo"]
        Maint3["Onderhoudspartij onderhoudt stable release branches in upstream repo"]

        %% Connections
        Dev3 --"push naar feature branch"--> Rev3
    end

    subgraph Landelijke-regie
    %% Nodes
    Up["Uitgever beheert versie branches in upstream repo"]

    end

    %% Nodes
    Regie["Regiepartij stuurt ontwikkeling en release management, faciliteert samenwerking tussen marktpartijen, en houdt toezicht op de kwaliteit van de codebase en het ecosysteem"]
    Impl["Implementatiepartij implementeert OpenZaak bij gemeente"]
    Up["Uitgever beheert versie en stable release branches in upstream repo"]
    SaaS["SaaS aanbieder levert draaiende instantie van stable release branches vanuit eigen repo"]

    %% Connections
    Regie --> Component1
    Regie --> Component2
    Regie --> Component3
    Rev1 --"merge into versie branch"--> Up
    Rev2 --"merge into versie branch"--> Up
    Rev3 --"merge into versie branch"--> Up
    Maint1 --> Up
    Maint2 --> Up
    Maint3 --> Up
    Up --> SaaS
    Up --> Impl

    %% Styling
    classDef softBlue fill:#e3f2fd,stroke:#90caf9,color:#0d47a1;
    class Dev1,Rev2 softBlue;

    classDef softGreen fill:#e8f5e9,stroke:#a5d6a7,color:#1b5e20;
    class Dev2,Rev3 softGreen;

    classDef softRed fill:#fdecea,stroke:#f5b7b1,color:#7f1d1d;
    class Dev3,Rev1 softRed;

```