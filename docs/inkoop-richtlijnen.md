---
layout: default
title: Richtlijnen voor inkoop
nav_order: 6
---

# Richtlijnen voor inkoop

Dit document bevat input voor inkooprichtlijnen voor OpenZaak.

## Inhoudsopgave
* TOC
{:toc}

## Inleiding

Bij de inkoop rond OpenZaak spelen meerdere beslissingslagen een rol, namelijk:

1) de GIBIT  
2) generieke Common Ground-principes  
3) ecosysteemkeuze per codebase  
4) afspraken met de marktpartij  

(Toelichting hieronder)

Een logische werkwijze lijkt om te verwijzen naar de GIBIT, daarnaast een Common Ground-document te hebben met principes en generieke ecosysteembeschrijvingen, en vervolgens een beknopt contract met de leverancier dat naar deze voorgaande lagen verwijst.

## De GIBIT 

De GIBIT is bewust breed opgezet om toepasbaar te zijn op alle IT-inkopen. Open source wordt wel genoemd, maar beperkt uitgewerkt. Dit is begrijpelijk, omdat zo flexibiliteit behouden blijft, afhankelijk van het type open source en de context van toepassing.

Hiervoor bestaat al een tool die contractteksten kan genereren en jaarlijks wordt geactualiseerd.

## Generieke Common Ground-principes

Het lijkt nuttig aanvullende documentatie op te stellen voor open source zoals uitgevoerd onder landelijke regie / Common Ground. Dit kan onderdeel zijn van het Standaard Governance Model (SGM) (zie "Samenwerkingsprincipes Platform Dienstverlening").

Deze aanvullende documentatie kan onder meer bevatten:  
- algemene richtlijnen voor governance binnen communities  
- specificaties over de repository waar code moet worden aangeleverd  
- een eenduidige definitie van “done”  
- engineering- en ontwerprichtlijnen zoals gehanteerd door de landelijke regie  
- welke standaardterminologie wordt gebruikt  
  
Dit zijn afspraken die richtinggevend zijn, maar niet vaak zouden moeten veranderen. Te verwijzen als organiserende principes in een centraal beheerd document.

## Ecosysteembeschrijvingen

Daarbovenop komt het ecosysteem rond een specifieke codebase (bijvoorbeeld één leverancier, meerdere leveranciers, aparte reviewpartijen, etc.). Dit is het niveau dat onregelmatig verandert, namelijk wanneer de communitystructuur of het belang van de codebase daarom vraagt.

De definitie van een beperkt aantal gestandaardiseerde ‘staten’ voor codebases en hun governance helpt met: 
- overzicht te houden  
- governance eenduidig toe te passen  
- standaardprocedures uit te voeren  
- het ecosysteem te ontwikkelen zonder bestaande contracten te veranderen

Zo wordt voorkomen dat iedere codebase of ieder contract een eigen afwijkende governance ontwikkelt.

Deze staten kunnen centraal worden beschreven, vastgesteld en beheerd door de codebase steward vanuit landelijke regie.

> Voorbeeldsituatie:
> Er is een overeenkomst met één leverancier voor vier jaar om als enige partij aan een codebase te werken. Na twee jaar groeit de codebase zodanig dat een tweede reviewpartij gewenst is. Dat moet mogelijk zijn zonder het oorspronkelijke contract te wijzigen.
>In het contract staat dan bijvoorbeeld:
> “De leverancier vervult deze rol, die zich momenteel in staat A bevindt en kan doorgroeien naar staat B.”

## Afspraken met de marktpartij  

Het contract met een individuele leverancier blijft vervolgens:

- kort  
- rolgericht  
- verwijzend naar de geldende kaders en de huidige “staat” van de codebase  

## Voorgestelde documentstructuur

Deze aanpak leidt tot een heldere scheiding van lagen:

- GIBIT-tool → genereert het juridische contractsjabloon  
- Landelijke regie → centraal online document met  
  - algemene werkafspraken  
  - werkafspraken per ‘staat’  
- Contract → één beknopt document per marktpartij  
- ‘Staat’ van de codebase → vastgelegd als bestand in de repository  

Zo ontstaat een modulair systeem waarin juridische stabiliteit en organisatorische flexibiliteit goed samengaan.
