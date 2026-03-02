---
layout: default
title: Intellectueel eigendom en licenties
parent: Resultaten
nav_order: 4
---

# Intellectueel eigendom en licenties

Dit document bevat input over de EUPL-licentie, verkregen via expertinterviews.

## Inhoudsopgave
* TOC
{:toc}

## Inleiding

Omdat er onduidelijkheid bestaat over Intellectueel Eigendom bij het laten ontwikkelen van Open Source Software en de rol van de licentie daarbij, maken we hier een kort overzicht van de belangrijkste punten. Let op dat dit geen juridisch advies is, maar een samenvatting van de huidige stand van zaken, die in beweging zijn.

Hoog over adviseren wij om deze vraag bij de Open Source Program Officer van Common Ground neer te leggen voor een formele juridische check, en de ontwikkeling van de GIBIT 25/26 nauwlettend te volgen.

## Achtergrond

*“Wanneer publieke organisaties aanbesteden, dan doen ze dat vrijwel altijd met behulp van standaard inkoopvoorwaarden. [...] Bij gemeenten is dat de GIBIT. In het geval van maatwerk, stellen deze inkoopvoorwaarden, moet het intellectueel eigendom worden overgedragen aan de opdrachtgever. De opdrachtgever wordt daarmee juridisch eigenaar van het ontwikkelde product. De achterliggende reden om juridisch eigenaar te willen zijn van een product, is dat je niet beperkt wordt in de doorontwikkeling ervan. Leveranciers hebben door de overdracht van intellectueel eigendom geen mogelijkheden om doorontwikkeling te belemmeren. Wanneer broncode zonder opensourcelicentie beschikbaar wordt gesteld [door een overheid, red.], dan zijn er volgens artikel 15b [van de auteurswet, red.] geen enkele belemmeringen in het gebruik ervan. Waarmee ook niet afgedwongen kan worden dat de doorontwikkeling van de broncode open source moet blijven. Vanuit open source licenties bekeken zou dit vergelijkbaar zijn met de BSD0*.”* - [https://opensourcewerken.nl/page/view/b28e707b-2731-49bf-bcc6-ac693f1f250a/overzicht-wet-en-regelgeving](https://opensourcewerken.nl/page/view/b28e707b-2731-49bf-bcc6-ac693f1f250a/overzicht-wet-en-regelgeving)]

\* Zie ook [https://en.wikipedia.org/wiki/Public-domain-equivalent_license](https://en.wikipedia.org/wiki/Public-domain-equivalent_license)

## GIBIT 2025 en Open Source

Op 2 maart 2026 publiceerde de VNG de nieuwe [GIBIT 2025](https://vng.nl/sites/default/files/2026-03/gibit-2025-artikelen.pdf) [[2](https://vng.nl/nieuws/vng-publiceert-gibit-2025-inkoopvoorwaarden)]. Hierin is Open Source als een los hoofdstuk opgenomen:

- Leverancier ontwikkelt in lijn met het Common Ground gedachtegoed.
- Broncode en rechten gaan naar Opdrachtgever.
- Overdracht vindt plaats bij publicatie in de repository.
- Broncode staat op een publiek Git-platform. Leverancier vertelt waar. Vóór acceptatie: privé. Daarna: publiek.
- De repository is de bron van waarheid.
- Opdrachtgever publiceert de broncode onder EUPL 1.2 of hoger.
- Bij incompatibele licenties: overleg over alternatief.
- Leverancier onderhoudt de software tijdens de looptijd.
- Opdrachtgever heeft doorslaggevende stem bij prioritering.
- Publicatie zit in de basisvergoeding.
- Extra werk wordt apart in rekening gebracht.
- Bij beëindiging worden openstaande verplichtingen (zoals publicatie) alsnog nagekomen.
- Geen bijzondere exit-regeling nodig als alles correct is nageleefd.

## Citaten

*"Wat zijn redenen om te kiezen voor intellectueel eigendom in plaats van voor een open source licentie? De aanwezigen waren eensgezind dat de bepaling over intellectueel eigendom eigenlijk voortkomt uit oud denken, en niet het beste juridische middel is om de gewenste doelen te bereiken. Een open source licentie verplicht stellen op maatwerk is effectiever."* - [https://opensourcewerken.nl/blog/view/db717354-150b-45f8-abf0-74a53f85c83b/open-source-aanbesteden-belemmeringen-kansen-en-intellectueel-eigendom](https://opensourcewerken.nl/blog/view/db717354-150b-45f8-abf0-74a53f85c83b/open-source-aanbesteden-belemmeringen-kansen-en-intellectueel-eigendom)

*"Tijdens de aanbesteding viel op dat we met elkaar een opgave hebben in hoe we vanuit aanbestedingsrecht kijken naar intellectueel eigendom in relatie tot open source. Volgens de meeste standaard inkoopvoorwaarden in de publieke sector komt bij maatwerkaanbestedingen het intellectueel eigendom standaard bij de opdrachtgever te liggen. Zo wordt de opdrachtgever niet belemmert bij de doorontwikkeling van dat maatwerk. Nadeel is alleen dat verder niemand iets met die broncode kan zonder toestemming van die opdrachtgever. Het biedt allerlei voordelen om die intellectueel eigendomsbepaling te vervangen of aanvullen door een opensource-licentie. Je wordt als opdrachtgever niet belemmerd in de doorontwikkeling van het maatwerk en derden – inclusief de opdrachtnemer – krijgen de mogelijkheid om de broncode ook (commercieel) te hergebruiken naar eigen inzicht. De broncode die met publiek geld is ontwikkeld kan daarmee aanvullend renderen én de leverancier heeft een prikkel om de broncode zo goed mogelijk voor hergebruik te ontwikkelen. Makkelijk te hergebruiken broncode is ook makkelijker te doorontwikkelen, wat weer een voordeel is voor de opdrachtgever."* - [https://opensourcewerken.nl/blog/view/d4728802-1556-44e7-b251-602ab0d03fcf/hoe-vws-open-source-aanbesteedt-naar-een-open-zorg-ict-ecosysteem](https://opensourcewerken.nl/blog/view/d4728802-1556-44e7-b251-602ab0d03fcf/hoe-vws-open-source-aanbesteedt-naar-een-open-zorg-ict-ecosysteem)

*"Denk dat ik al in 2008 heb geschreven dat de overheid als opdrachtgever kan kiezen tussen overdracht van auteursrechten, of in plaats daarvan levering onder de EUPL. Daaruit volgt dat overdracht inderdaad niet perse nodig is."* - Matthieu Paapst, expert Open Source en Intellectueel Eigendom.

*"Terzijde: die beoogde wetswijziging van de Auteurswet gaat volgens mij vooral over het werkgeversauteursrecht, en niet over de overdracht waar wij het nu over hebben. Daarvoor blijft namelijk, net zoals nu het geval is, een schriftelijke en specifieke overdracht noodzakelijk. ***De enkele vermelding ervan in algemene voorwaarden wordt is en was onvoldoende om de overdracht ook daadwerkelijk te effectueren.**"* - Matthieu Paapst, expert Open Source en Intellectueel Eigendom.

*"Voor de delen van de code waar je zelf de IE-rechten van bezit, kun je altijd nog van licentie wisselen. Zodra de code echter is vermengd met bijdragen van derden, zit je vast aan de voorwaarden waaronder zij hun bijdrage hebben geleverd. Een licentiewijziging kan dan alleen met hun toestemming. Let er ook op dat een licentiewijziging van een module gevolgen kan hebben voor de licentie van het project als geheel. Zo kan een project als geheel niet langer onder de EUPL blijven, wanneer een losse module van MIT naar GPL wijzigt – althans niet meer in combinatie met die specifieke versie van de module."* - [https://minvws.opensourcewerken.nl/open-source-ambitieladder-voor-opensourcewerken-in-projecten/](https://minvws.opensourcewerken.nl/open-source-ambitieladder-voor-opensourcewerken-in-projecten/)

### Voorlopige analyse voor OpenZaak (niet juridisch)

- Indien de software is ontstaan onder de vorige GIBIT, dan is volgens de GIBIT het IE bij de (toenmalige) opdrachtgever (wie is dat?), met de kanttekening van Matthieu Paapst dat algemene voorwaarden niet voldoende zijn voor overdracht; dat moet expliciet gebeuren in de overeenkomst.
- Indien EUPL licentie vanaf het begin is afgesproken, dan zijn alle bijdragen onder die licentie gedaan.
- De EUPL licentie geeft iedereen (waaronder de opdrachtgever) het recht om de software te gebruiken, te wijzigen, te verspreiden, en afgeleide werken te maken (en dus door te (laten) ontwikkelen), mits de voorwaarden van de licentie worden nageleefd.
- Intellectueel eigendom noch licentie zegt iets over de beschikbaarheid van de broncode. Zorg voor een kopie op een plaats onder eigen beheer.
- Zaken als merkregistratie en domeinnaam staan los van IE en licentie op de software, maar zijn wel belangrijk om ook goed te regelen.

**Laat dit formeel checken door een jurist (wij zijn dat niet)**
