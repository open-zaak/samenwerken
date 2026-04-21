---
layout: default
title: Test scenarios 
parent: Vervolgstappen
nav_order: 2
---

# Test scenarios

Prioriteit:  

1) Ontiwkkelen van een nieuwe feature  
2) Security report via de github repo  
3) Patch release met bug fixes  
4) Pull request van buitenaf  
   
Later uit te werken:  

1) Feature release (major and minor)  
2) Nieuwe versie van de VNG standaard  
3) Dependabot issue gemaakt van common vulnerability exploit (automatic)  
4) Wens vanuit andere overheidsorgaan (bvb Logius)  
5) Wens vanuit andere gemeente voor locaal versnellen  
6) Wens vanuit de regie organisatie  
7)  Bug/issue reported op de github  
8)  Security release  
9)  Issue vanuit test suite voor dependencies tussen componenten

## Ontiwkkelen van een nieuwe feature

| Stap | Regie | Uitgever | Onderhoud |
|------|-------|----------|-----------|
| 1 | stelt financiering en opdracht beschikbaar; keurt feature goed voor roadmap en bewaakt scope en architectuurprincipes | — | — |
| 2 | valideert architecturale conformiteit van de feature tijdens het ontwikkelproces | — | — |
| 3 | — | — | beoordeelt impact op bestaande stable releases en backwards compatibiliteit |
| 4 | — | accepteert en reviewt pull request op kwaliteit, veiligheid, herbruikbaarheid en architecturale fit | — |
| 5 | — | verwerkt goedgekeurde feature in een nieuwe versietak; past versiebeheer toe | — |
| 6 | — | publiceert release-notes en communiceert release naar mailinglijst | — |
| 7 | — | werkt documentatie en compatibiliteitsmatrix bij | — |
| 8 | — | — | beoordeelt de nieuwe feature expliciet op beheerbaarheid, onderhoudbaarheid en overdraagbaarheid voordat structureel beheer wordt aanvaard |
| 9 | — | — | rolt CI pipeline en geautomatiseerde testen uit op nieuwe release; lost eventuele regressions op |

## Security report via de github repo

| Stap | Regie | Uitgever | Onderhoud |
|------|-------|----------|-----------|
| 1 | — | ontvangt melding via responsible disclosure e-mailadres of issue tracker | — |
| 2 | wordt geïnformeerd over ernst en scope; is eindverantwoordelijk voor naleving van het disclosure beleid | — | voert dagelijkse beveiligingsscan uit; identificeert of bevestigt het probleem |
| 3 | beslist over prioriteit en urgentie in overleg met uitgever en onderhoud; escaleert indien nodig conform security- en compliancekaders | — | — |
| 4 | — | — | valideert en reproduceert het beveiligingsprobleem; beoordeelt prioriteit |
| 5 | — | — | ontwikkelt en test de security patch |
| 6 | — | — | levert patch aan als pull request aan de uitgever |
| 7 | — | reviewt en accepteert de patch; verwerkt in een patch release | — |
| 8 | wordt geïnformeerd over CVE publicatie; keurt communicatie goed conform disclosure beleid | publiceert CVE; communiceert security release naar mailinglijst en relevante stakeholders | — |
| 9 | — | archiveert de gepatchte release in de centrale repository | — |
| 10 | — | — | monitort stable releases na de patch op eventuele verdere issues |

## Patch release met bug fixes

| Stap | Regie | Uitgever | Onderhoud |
|------|-------|----------|-----------|
| 1 | — | — | monitort stable releases op bugs, security en performance issues |
| 2 | — | — | valideert gerapporteerde bugs en beoordeelt prioriteit |
| 3 | wordt geïnformeerd over prioriteit en scope van de patch | — | — |
| 4 | — | — | ontwikkelt en test bug fixes binnen de stable release branch |
| 5 | — | — | levert patch aan als pull request aan de uitgever |
| 6 | — | reviewt en accepteert de patch op kwaliteit, veiligheid en backwards compatibiliteit | — |
| 7 | — | verwerkt goedgekeurde patch in een nieuwe patch release; past versiebeheer toe | — |
| 8 | — | publiceert release-notes en communiceert patch release naar mailinglijst | — |
| 9 | — | archiveert de gepatchte release in de centrale repository | — |

## Pull request van buitenaf

| Stap | Regie | Uitgever | Onderhoud |
|------|-------|----------|-----------|
| 1 | — | ontvangt pull request via de openbare issue tracker of repository | — |
| 2 | — | toetst of de bijdrage voldoet aan de contributierichtlijnen en EUPL licentievoorwaarden | — |
| 3 | — | monitort pull request op kwaliteit, veiligheid, herbruikbaarheid en architecturale fit | — |
| 4 | — | — | beoordeelt impact op bestaande stable releases en backwards compatibiliteit |
| 5 | wordt geconsulteerd indien de bijdrage raakt aan roadmap, scope of architectuurprincipes | — | — |
| 6 | — | geeft feedback aan de externe bijdrager en begeleidt het iteratieproces | — |
| 7 | — | accepteert en verwerkt goedgekeurde bijdrage in de relevante versietak | — |
| 8 | — | werkt documentatie en release-notes bij | — |
| 9 | — | — | beoordeelt de bijdrage op beheerbaarheid en onderhoudbaarheid voordat structureel beheer wordt aanvaard |
| 10 | — | — | rolt CI pipeline en geautomatiseerde testen uit op de bijgewerkte codebase |
