---
layout: default
title: Bedrijfszekerheidsfactor
nav_order: 2
parent: Tools
---

# Templates voor stewardship report

## Strategisch belang?

Wat is het strategisch belang van de codebase?

## Bedrijfszekerheidsfactor

### Continuiteit 

Hoe belangrijk is het de continuiteit voor de overheid?

> bvb - bepaalde uptime? kan het makkelijk worden vervangen door een andere codebase of marktpartij? hoe veel zou dit kosten/welke risicos brengt het mee?

Hoe belangrijk is de continuiteit van de marktpartij?

> bvb - is het belangrijk dat die zelvde marktij altijd het zelvde team heeft klaar staan? verwachten we regelmatig werk dat snel gedaan moet worden? zouden vertragingen bij nieuwe features een probleem zijn? hoeveel specialisatie kennis is er, en is het makkelijk om nieuwe developers met warme kennis te vinden?

```mermaid
quadrantChart
    title Continuiteit ven contracten en werken
    x-axis Onzekerheid Overheid --> Zekerheid Overheid
    y-axis Onzekerheid Marktpartij --> Zekerheid Marktpartij
    quadrant-1 1
    quadrant-2 2
    quadrant-3 3
    quadrant-4 4
    Ambitie landelijkevoorziening: [0.8, 0.8]
    Codebase nu: [0.3, 0.3]
```

### Financiering 

Hoe strak is de financiering rondom de codebase?

```mermaid
quadrantChart
    title Financiering
    x-axis Strak --> Flexible
    y-axis Ongestructureerd --> Gestructureerd
    quadrant-1 1
    quadrant-2 2
    quadrant-3 3
    quadrant-4 4
    Ambitie landelijkevoorziening: [0.8, 0.8]
    Codebase nu: [0.4, 0.3]
```

### Verantwoordelijkheid 

Op welke wijze wordt verantwoordelijkheid voor de codebase geborgd?

```mermaid
quadrantChart
    title Verantwoordelijkheid
    x-axis Onverbonden --> Persoonlijke betrokkenheid
    y-axis Ongestructureerd --> Structureerd gewaarborgd
    quadrant-1 1
    quadrant-2 2
    quadrant-3 3
    quadrant-4 4
    Ambitie landelijkevoorziening: [0.8, 0.8]
    Codebase nu: [0.8, 0.3]
```

### Samenwerking tussen community 

Hoe werkt de community samen?

```mermaid
quadrantChart
    title Samenwerking
    x-axis Opportunistisch --> Waarde gedreven
    y-axis Ad hoc --> Gestructureerd
    quadrant-1 1
    quadrant-2 2
    quadrant-3 3
    quadrant-4 4
    Ambitie landelijkevoorziening: [0.8, 0.8]
    Codebase nu: [0.5, 0.4]
```
