---
layout: default
title: Ecosysteemconfiguratie
nav_order: 1
parent: Tools
---

# Ecosysteemconfiguratie

Status: Draft

# Rollen en verantwoordelijkheden in het open-source component-ecosysteem

Dit document beschrijft de rollen en hun onderlinge verhoudingen in een componentgebaseerd softwareontwikkellandschap met open source software.
Het uitgangspunt is dat niet alleen componenten, maar het **hele ecosysteem** actief wordt gestuurd en bewaakt.
De regiepartij vervult hierin een expliciete **ecosysteem-stewardship** rol met het oog op samenhang en bedrijfszekerheid.

Het ecosysteem bestaat uit **meerdere componenten**, waarbij **per component één primaire ontwikkelpartij** verantwoordelijk is voor de realisatie.
Gezamenlijk vormen deze ontwikkelpartijen een pool die elkaar over en weer ondersteunt via review en kennisdeling.

---

## Regiepartij

De regiepartij is systeemverantwoordelijk voor het functioneren, de samenhang en de duurzaamheid van het gehele ecosysteem.
Zij is steward van zowel de componenten als de instituties, processen en relaties daaromheen.

- **Architectuur / integratie**  
  Stelt architectuurprincipes vast, bewaakt samenhang tussen componenten en definieert API-contracten, standaarden en integratiepatronen.
  Stuurt actief op ontkoppeling, vervangbaarheid en beheersbare afhankelijkheden.

- **Product-/component ownership**  
  Bepaalt doel, scope, roadmap en prioriteiten van componenten vanuit publieke waarde en herbruikbaarheid.
  Neemt besluiten over starten, doorontwikkelen, samenvoegen en uitfaseren van componenten.

- **Productdefinitie & versiebeleid**  
  Bepaalt wat als eindproduct geldt, welke functionaliteit en configuraties daarbij horen, en wanneer nieuwe versies worden vrijgegeven of uitgefaseerd.
  Is eigenaar van productcommunicatie, roadmap en lifecycle-informatie.

- **Lifecycle- en compatibiliteitsbeleid**  
  Stelt beleid vast voor versieondersteuning, backward compatibility en end-of-life, inclusief afweging tussen stabiliteit, innovatie en beheerkosten.

- **Financiering & opdrachtgeverschap**  
  Regelt structurele bekostiging, mandaat en contractuele afspraken.
  Borgt continuïteit, onafhankelijkheid en lange termijn duurzaamheid van het ecosysteem.

- **Community / stewardship (ecosysteemniveau)**  
  Organiseert, documenteert en bewaakt open-source governance van het hele ecosysteem: bijdrageprocessen, besluitvorming, rolzuiverheid, kenniscontinuïteit en bedrijfszekerheid.
  Voorkomt machtsconcentratie en lock-in, en organiseert escalatie en conflictbeslechting.

- **Audit & toezicht**  
  Organiseert onafhankelijke toetsing op kwaliteit, werking, governance en publieke waarden, zowel op component- als ecosysteemniveau.
  Zorgt dat bevindingen worden opgevolgd.

- **Security & compliance**  
  Definieert en handhaaft security-eisen, privacy-kaders en wettelijke compliance.
  Borgt dat deze consistent worden toegepast door alle partijen.

- **Release & distributie**  
  Beslist over releases, versies en distributiekanalen.
  Borgt reproduceerbare builds, transparantie over wijzigingen en heldere communicatie richting beheer, hosting en implementatie.

- **Codebeschikbaarheid & centrale codevoorziening**  
  Zorgt voor structurele beschikbaarheid en toegankelijkheid van alle componentcode via een centrale codevoorziening (bijv. een gezamenlijke Git-hostingomgeving).
  Borgt uniforme inrichting van repositories, toegangsrechten, bijdrageprocessen en archivering, zodat code vindbaar, overdraagbaar en onafhankelijk van individuele partijen blijft.

---

## Ontwikkelpartij

Per component is één ontwikkelpartij aangewezen als **primaire ontwikkelverantwoordelijke**.
Deze partij is verantwoordelijk voor realisatie en doorontwikkeling van het component binnen de kaders van het ecosysteem en in opdracht van de regiepartij.
Over het hele ecosysteem bestaan meerdere ontwikkelpartijen, ieder primair verantwoordelijk voor een of meer componenten.

- **Ontwikkeling**  
  Ontwerpt, bouwt en test de eigen component(en) conform vastgestelde architectuur, standaarden en kwaliteitscriteria.

- **Kennis & documentatie (Definition of Done)**  
  Levert bij elke wijziging volledige en actuele documentatie: code-documentatie, technische uitleg, gebruiksinformatie en relevante ontwerpkeuzes.

- **Vervullen van reviewrollen in andere componenten**  
  Treedt, naast het ontwikkelen van eigen componenten, op als aangewezen reviewpartij voor andere componenten binnen het ecosysteem, conform toewijzing en kaders van de regiepartij.

---

## Reviewpartij

Per component wordt **één onafhankelijke reviewpartij aangewezen**.
Deze partij is niet de primaire ontwikkelpartij van het betreffende component.
In de praktijk worden reviewrollen vervuld door andere ontwikkelpartijen uit het ecosysteem, waardoor kennis wordt gespreid en afhankelijkheid van één partij wordt voorkomen.

- **Onafhankelijke code-, architectuur- en kwaliteitsreview**  
  Toetst het component op onderhoudbaarheid, veiligheid, architectuurconformiteit en kwaliteit, los van het ontwikkelbelang van het component zelf.

- **Warme kennis als ecosysteemvoorziening**  
  Door structurele review ontstaat inhoudelijke kennis bij meerdere partijen, waardoor continuïteit en overdraagbaarheid van componenten worden vergroot.

---

## Beheerpartij

De beheerpartij is verantwoordelijk voor de stabiliteit en betrouwbaarheid van componenten over de lange termijn, los van wie ze oorspronkelijk heeft ontwikkeld.

- **Overname en acceptatie van de codebase**  
  Ontvangt de codebase vanuit de ontwikkelpartij en beoordeelt deze expliciet op beheerbaarheid, onderhoudbaarheid en overdraagbaarheid.
  Verifieert dat documentatie, versie-inrichting en technische keuzes voldoen aan de eisen voor langetermijnbeheer voordat structureel beheer wordt aanvaard.

- **Langetermijnonderhoud**  
  Zorgt voor duurzame werking van componenten na oplevering.

- **Versiebeheer en compatibiliteitsbeleid**  
  Beheert ondersteunde versies, patches en updates binnen het door de regiepartij vastgestelde compatibiliteitsbeleid.
  Backward compatibility wordt alleen geborgd waar dit expliciet is besloten, gezien de kosten en impact op beheer en doorontwikkeling.

- **Kennis & documentatie m.b.t. lifecycle en onderhoud**  
  Onderhoudt documentatie over beheerprocedures, lifecycle-keuzes, migraties en end-of-life trajecten.

---

## Hostingpartij (productleverancier / SaaS)

De hostingpartij levert de **eindproducten** aan afnemers in de vorm van operationele SaaS-diensten.
Zij is verantwoordelijk voor het daadwerkelijk beschikbaar stellen van werkende functionaliteit aan gebruikers, binnen de kaders van het ecosysteem.

- **Dienstverlening op basis van vastgestelde eindproducten**  
  Levert door de regiepartij gedefinieerde eindproducten als SaaS-dienst.
  Wijzigt geen functionaliteit, versies of lifecycle zonder expliciete afstemming en besluitvorming door de regiepartij.

- **Exploitatie**  
  Draagt verantwoordelijkheid voor performance, schaalbaarheid, capaciteit en kostenbeheersing van de diensten.

- **Operations**  
  Verzorgt monitoring, incidentmanagement, back-ups, herstel en dagelijkse operationele beveiliging.

- **Conformiteit aan ecosysteemkaders**  
  Levert de eindproducten binnen vastgestelde architectuur-, security-, compliance- en lifecyclekaders, en stemt wijzigingen af met regie- en beheerpartij.

---

## Implementatiepartners

Implementatiepartners ondersteunen organisaties bij het **in gebruik nemen van de SaaS-eindproducten**.
Zij begeleiden de organisatorische, procesmatige en gebruikerskant van adoptie, zonder zelf eigenaar te zijn van de software of de dienstverlening.

- **Adoptie van SaaS-eindproducten**  
  Helpen organisaties bij het starten met en effectief gebruiken van de geleverde SaaS-diensten.

- **Inbedding in de uitvoering**  
  Ondersteunen bij het aanpassen van werkprocessen, configuraties en werkwijzen zodat de SaaS-diensten aansluiten op de dagelijkse praktijk.

- **Gebruikersvertegenwoordiging**  
  Brengen ervaringen, knelpunten en behoeften van gebruikers terug naar het ecosysteem ter verbetering van productdefinitie, adoptie en dienstverlening.
