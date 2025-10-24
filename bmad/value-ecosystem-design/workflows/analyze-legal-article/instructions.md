# Legal Article Analysis Workflow v2.0 - Complete Rewrite

## Overview
Deze workflow analyseert juridische artikelen en converteert ze direct naar OWL instanties in een juridische Knowledge Graph, gebruikmakend van volledige OntologyBasis expertise uit alle 13 Tonto ontologieën.

## Prerequisites - Belangrijke Vereisten

**Vooraf te laden bestanden:**
- Hierarchy van alle 13 OntologyBasis .tonto bestanden
- OntologyBasis.ttl voor OWL URI mapping
- Alle 7 Tonto guidance files voor juiste interpretatie
- Bestaande Knowledge Graph docs/legal-knowledge-graph.ttl

**Tonto Expertise Vereist:**
Workflow moet volledige kennis hebben van:
- UFO-L ontologische patronen
- @mediation, @componentOf, @formal relatie semantic
- LegalOntology, LawOntology, ObjectOntology als primaire ontologieën
- Juridische domein termen en verbanden

---

# RONDE 1: Ontology Loading & Tonto Expertise

## STAP 1: Ontology Loading
**Doel:** Laad alle OntologyBasis bestanden voor volledige juridische kennis

**Te Laden:**
1. **Alle 13 Tonto OntologyBasis files**
   - AgentOntology.tonto
   - DEMOOntology.tonto
   - EventOntology.tonto
   - IndividualOntology.tonto
   - LawOntology.tonto ✓ **PRIMAIRE**
   - LegalOntology.tonto ✓ **PRIMAIRE**
   - ModeOntology.tonto
   - ObjectOntology.tonto ✓ **PRIMAIRE**
   - OfferingOntology.tonto
   - ValueAscriptionOntology.tonto
   - ValueBearerOntology.tonto
   - ValueOntology.tonto
   - ValuePropositionOntology.tonto

2. **OntologyBasis.ttl voor OWL URI mapping**
3. **Alle 7 Tonto guidance files** voor interpretatie instructies

**Input:** Artikel tekst van gebruiker
**Output:** Geladen ontologieën klaar voor analyse

## STAP 2: Knowledge Graph Loading
**Doel:** Laad bestaande juridische Knowledge Graph voor cross-reference

**Te Laden:** docs/legal-knowledge-graph.ttl
**Initialisatie:** Proximity scoring subsystem met legal structure awareness
**Validatie:** KG moet parseable OWL zijn

---

# RONDE 2: Eerste Juridische Mapping (Primaire Ontologieën)

## STAP 3: Primaire Juridische Ontologie Mapping
**Doel:** Map alle artikel elementen naar exact 3 primaire ontologieën

**Primaire Ontologieën Te Gebruiken:**
1. **LegalOntology**: Rechtssubjecten, relators, claims/commitments, posities
2. **LawOntology**: Artikel structuur, wettelijke elementen, hiërarchieën
3. **ObjectOntology**: Normen, verplichtingen, bevoegdheden, uitzonderingen

**Mapping Proces:**
- Lees volledig artikel door
- Identificeer alle juridische concepten in de tekst
- Map ELK concept naar relevante primaire ontologie klasse

**Classificatie Aantal Check:** Minimaal 3 verschillende primaire ontologieën per artikel moeten geraakt worden

**USER APPROVAL VERPLICHT:**
Voor elke identificatie: Zodat gebruiker bevestigt dat mapping correct is

## STAP 4: Primaire Mapping Cross-Reference
**Doel:** Cross-reference alle nieuwe concepten tegen bestaande KG

**Dual Proximity Analyse:**
1. **Semantic Proximity** (zoals huidige workflow)
2. **NIEUW: Legal Structure Proximity**
   - Extra punten voor zelfde wet (+50)
   - Extra punten voor zelfde hoofdstuk (+30)
   - Extra punten voor aangrenzende artikelen (+15)
   - Extra punten voor zelfde juridische domein (+20)

**Combined Scoring Thresholds:**
- **≥150 punten:** Automated merge recommendation
- **80-149 punten:** Gebruiker beslissing required
- **30-79 punten:** Verder onderzoek nodig
- **<30 punten:** Hoogstwaarschijnlijk nieuw concept

**USER APPROVAL VERPLICHT:**
Gebruiker krijgt lijst van matches met proximity scores en moet kiezen:
- Extend existing concept
- Create new concept
- Merge concepts
- Investigate further

## STAP 5: Primaire Relatie Analyse
**Doel:** Analyse juridische relaties volgens UFO-L ontologische patronen

**Exclusief toegestaan relatie stereotypen:**
- `@mediation` (LegalOntology relator pattern)
- `@componentOf` (LawOntology hiërarchie)
- `@formal` (ObjectOntology norm definities)

**ANDERE rapporten stereotypen NIET TOEGESTAAN**
Dit voorkomt ontologische inconsistenties.

**USER APPROVAL VERPLICHT:**
Elke geïdentificeerde relatie moet door gebruiker goedgekeurd worden

---

# RONDE 3: Secundaire Ontologie Cross-Analysis

## STAP 6: Secundaire Ontologie Mapping
**Doel:** Breid concepten uit naar alle 10 resterende ontologieën

**Proces:**
1. Neem primaire mappings als startpunt
2. Laad één voor één elk van de overige ontologieën
   - AgentOntology.tonto
   - DEMOOntology.tonto
   - EventOntology.tonto
   - IndividualOntology.tonto
   - ModeOntology.tonto
   - OfferingOntology.tonto
   - ValueAscriptionOntology.tonto
   - ValueBearerOntology.tonto
   - ValueOntology.tonto
   - ValuePropositionOntology.tonto
3. Analyseer de geladen ontologie
   * Voor elk geïdentificeerd concept: vind aanvullende relaties in de andere ontologieën
   * Gebruik cross-ontology patronen voor consistente semantiek
4. Als nog niet alle ontologieën bekeken zijn:
   * Laad de volgende ontologie en herhaal de analyse voor die ontologie.

**Cross-Analysis Doel:**
Elke collectie concepten moet in samenhang gebracht worden met de overige ontologieën.

**USER APPROVAL VERPLICHT:**
Gebruiker ziet alle cross-ontology relaties en kan Nederlandse termen bijstellen

## STAP 7: Secundaire Ontologie Validatie
**Doel:** Cross-ontology integratie en conflict detectie

**Te Controleren:**
- Semantic conflicts tussen ontologische interpretaties
- Missing logical connections tussen concepten
- Coherence checks tussen alle 13 ontologieën

**Validatie Output:**
Lijst van geïdentificeerde conflicts/issues met oplossingsvoorstellen

**USER APPROVAL VERPLICHT:**
Gebruiker moet conflicten oplossen voordat naar volgende ronde

---

# RONDE 4: Advanced Cross-Reference & Proximity

## STAP 8: Advanced Proximity Cross-Reference
**Doel:** Nieuwe ronde cross-reference met full proximity awareness

**Advanced Analyses:**
1. **Semantic Matching** tegen alle bestaande KG concepten
2. **Legal Structure Proximity** (wet, hoofdstuk, artikel hiërarchie)
3. **Combined Proximity Scoring** met drempelwaarden
4. **Cross-Reference met Nederlandse termen** voor taal-consistentie

**Decision Matrix:**
Gebruiker krijgt tabel met:
- Nieuwe concept
- Beste match(es) uit KG
- Proximity score breakdown
- Recommended action (merge/extend/new)

**USER APPROVAL VERPLICHT:**
Elke final decision over concept relationship moet goedgekeurd worden

---

# RONDE 5: OWL Knowledge Graph Documentatie

## STAP 9: OWL Instantie Creatie

**Doel:** Creëer formele OWL instanties voor alle geaccepteerde concepten

**Taak:**
Jouw taak is het creëren van een formele, conceptuele representatie van juridische concepten. Je volgt hierbij de good practice om het begrippenkader en de ontologie te scheiden. Voor elk juridisch concept creëer je twee verbonden entiteiten:
* Een Klasse (owl:Class) in de ontologie, die het 'zijn' van het concept modelleert.
* Een Begrip (skos:Concept) in het begrippenkader, die de 'gedachte' over het concept beschrijft.

Dit zorgt voor een duurzame, machineleesbare en nationaal uitwisselbare knowledge graph. Elk concept wordt toegevoegd aan de centrale, cumulatieve knowledge base, opgeslagen in het bestand docs\legal-knowledge-graph.ttl

**Kernprincipes**
* NL-SBB Conformiteit: Voor een Begrip volg je de structuur zoals gedefinieerd in https://github.com/geonovum/NL-SBB. Dit is de leidende standaard.
* Eén Bron van Waarheid: Alle kennis wordt in één enkel bestand (docs\legal-knowledge-graph.ttl) beheerd. Je creëert geen nieuwe bestanden per concept.
* Idempotentie: Het toevoegen van een Begrip of Klasse die al bestaat, mag geen wijziging in het bestand veroorzaken. Je controleert altijd op het bestaan van een URI voordat je toevoegt.
* Lidmaatschap van een Begrippenkader (NL-SBB): Elk Begrip MOET lid zijn van een centraal gedefinieerd skos:ConceptScheme.
* Strikte Scheiding: Strikte Scheiding: Modelleer de owl:Class en het skos:Concept als aparte resources met hun eigen URI's.
* Correcte Eigenschappen:
  * Formele, logische relaties (rdfs:subClassOf) horen bij de Klasse.
  * Beschrijvende, lexicale en contextuele metadata (skos:prefLabel, skos:definition, dcterms:source) horen bij het Begrip.
* Gespecialiseerde Relaties: Modelleer relaties tussen domein-specifieke klassen als owl:ObjectProperty. Deze moeten rdfs:subPropertyOf zijn van een generieke relatie uit de upper-ontology, en moeten een specifieke rdfs:domain en rdfs:range hebben.
* Verplichte Metadata (NL-SBB): Elk Begrip MOET een unieke dcterms:identifier en een rov:status hebben
* Gestructureerde Data (SKOS): Gebruik de specifieke SKOS-properties voor definities, labels en noten. Vermijd het generieke rdfs:comment.
* Volledige Meertaligheid: Alle tekstuele metadata (literals) MOETEN worden voorzien van een taaltag (@nl en @en).
* Externe Bronnen: De bronverwijzing (dcterms:source) linkt naar de officiële, externe URI's. Zorg ervoor dat je de door de gebruiker opgegeven link hiervoor gebruikt.
* Verbinden met BasisOntology: Elke Klasse moet verbonden worden met de gerelateerde concepten uit de BasisOntology die in de eerdere stappen zijn gevonden. Gebruik daarvoor rdfs:SubClassOf, of een meer passende rdfs of owl eigenschap.

**Stappenplan voor het Creëren van een Concept**
Volg deze stappen rigoureus voor elk te modelleren juridisch concept.

**Stap 9a: Definieer de Prefixen**
Elk Turtle-bestand moet beginnen met deze gestandaardiseerde prefixen. Controleer in de bestaande Knowdlegde Graph (docs\legal-knowledge-graph.ttl) of onderstaande prefixen al aanwezig zijn. Indien er prefixen ontbreken, voeg deze dan toe.

@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix rov: <http://www.w3.org/ns/reg-en-ovid#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

# Namespace voor de formele ontologie (de Klassen)
@prefix ont: <http://data.recht.nl/ont/> .

# Eigen namespaces voor het begrippenkader
@prefix vocab: <http://data.recht.nl/begrippenkader/> .

# Namespace voor de concepten (definities)
@prefix begrip: <http://data.recht.nl/begrip/> .

# Placeholder voor de Upper-Ontology
@prefix ob: <http://example.com/upper-ontology#> .

**Stap 9b: Creeer de Klasse**
Dit is de formele, logische entiteit.
1. Bepaal de URI: ont:{ConceptNaamInCamelCase} (bv. ont:OnrechtmatigeDaad)
2. Wijs het Type toe: a owl:Class ;
3. Voor elke gevonden relatie van de Klasse met een concept uit de BasisOntology:
   * Verbind de Klassse met de BasisOntology: Gebruik rdfs:subClassOf of andere passende eigenschappen om de Klasse in de bredere hiërarchie te plaatsen. 
4. Verbind met het Begrip: Voeg de cruciale link toe die stelt "de betekenis van deze klasse wordt uitgelegd door het volgende begrip".
  * Code: rdfs:isDefinedBy begrip:{ConceptNaamInCamelCase} .

**Stap 9c: Modelleer Formele Relaties (owl:ObjectProperty)**
Dit is de nieuwe, cruciale stap. Wanneer twee van de Klassen in de Knowledge Graph een relatie hebben die een specialisatie is van een relatie in de BasisOntology:
1. Identificeer de Generieke Relatie: Vind de owl:ObjectProperty in de BasisOntology (bv. upper:inheresIn_2).
2. Definieer de Specifieke Relatie:
   * Creëer een URI: ont:{relatienaam} (bv. ont:heeftAlsDrager).
   * Wijs Type toe: a owl:ObjectProperty ;
   * Maak het een Sub-Property: rdfs:subPropertyOf ob:inheresIn_2 ;
3. Definieer het Domein en Bereik (Domain & Range): Koppel de relatie aan de specifieke klassen die u in 9b heeft gemaakt.
   * rdfs:domain klas:{DomeinKlasse} ; (bv. klas:Aanbiedingsverplichting)
   * rdfs:range klas:{BereikKlasse} . (bv. klas:Aanbieder)
4. Geef een Label: rdfs:label

**Stap 9d: Creeer de Begrippen**
Dit is de rijke, mens-leesbare beschrijving. Voor elke Klasse en elke Specifieke Relatie die beschreven moet worden, creëer een bijbehorend skos:Concept.
1. Bepaal de URI: begrip:{ConceptNaamInCamelCase} (bv. begrip:OnrechtmatigeDaad)
2. Wijs het Type toe: a skos:Concept ;
3. Voeg NL-SBB Metadata toe:
   * skos:inScheme vocab:JuridischBegrippenkader ;
   * dcterms:identifier "JBK-{ConceptNaam}"^^xsd:string ;
   * rov:status rov:stabiel ;
4. Voeg Beschrijvende Metadata toe (SKOS):
   * skos:prefLabel, skos:altLabel, elk met @en en @nl
   * skos:definition (de tekstuele definitie), @en en @nl
   * skos:scopeNote, skos:example, @en en @nl
5. Verwijs naar de Juridische Bron: dcterms:source <officiële-uri> ;
6. Leg Semantische Relaties met Andere Begrippen:
   * skos:broader, skos:related etc. naar andere begrip: URI's.

**VOORBEELD**
# === PREFIX DEFINITIES ===
# ...

# === Stap 9b: DEFINITIE VAN DE KLASSEN ===

ont:Aanbieder
  a owl:Class ;
  rdfs:subClassOf ob:Offeror ;
  rdfs:isDefinedBy begrip:Aanbieder .

ont:Aanbiedingsverplichting
  a owl:Class ;
  rdfs:subClassOf ob:OfferingCommitment ;
  rdfs:isDefinedBy begrip:Aanbiedingsverplichting .

# === Stap 9c: DEFINITIE VAN DE GESPECIALISEERDE RELATIE ===
# Deze relatie is een specifieke vorm van de 'inheresIn' relatie uit de upper-ontology,
# maar dan toegespitst op de juridische context van aanbieders en hun verplichtingen.

ont:heeftAlsDrager
  # Typering
  a owl:ObjectProperty ;

  # Specialisatie: dit is een sub-eigenschap van de generieke relatie
  rdfs:subPropertyOf ob:inheresIn_2 ;

  # Specificatie: het domein en bereik zijn nu veel specifieker
  rdfs:domain ont:Aanbiedingsverplichting ;
  rdfs:range ont:Aanbieder ;

  # Beschrijving
  rdfs:label "heeft als drager"@nl ;
  rdfs:isDefinedBy begrip:heeftAlsDrager .

# === Stap 9c: DEFINITIE VAN DE BEGRIPPEN ===

begrip:Aanbieder
  a skos:Concept ;
  skos:inScheme vocab:JuridischBegrippenkader ;
  rov:status rov:stabiel ;
  dcterms:identifier "JBK-Aanbieder"^^xsd:string ;
  skos:prefLabel "Aanbieder"@nl ;
  skos:definition "De (rechts)persoon die gehouden is een aanbiedingsverplichting na te komen."@nl .
  dcterms:source <http://wetten.overheid.nl/eli/nl/wet/1992/01/01/BWBR0005289/boek/6> ;
  # Hiërarchie: Een Aanbieder is een specifiek soort Rechtssubject.
  skos:broader begrip:Rechtssubject ;
  # Associatie: Een Aanbieder is gerelateerd aan het Aanbod dat hij doet.
  skos:related begrip:Aanbod .

begrip:Aanbiedingsverplichting
  a skos:Concept ;
  skos:inScheme vocab:JuridischBegrippenkader ;
  rov:status rov:stabiel ;
  dcterms:identifier "JBK-Aanbiedingsverplichting"^^xsd:string ;
  skos:prefLabel "Aanbiedingsverplichting"@nl ;
  skos:definition "Een verplichting die inherent is aan een aanbieder om een aanbod te doen onder bepaalde voorwaarden."@nl .
  # Bronverwijzing: Dit soort verplichtingen komt vaak voort uit jurisprudentie over aandeelhoudersovereenkomsten.
  dcterms:source <https://deeplink.rechtspraak.nl/uitspraak?id=ECLI:NL:HR:2015:1234> ; # Let op: fictieve ECLI

  # Hiërarchie: Een Aanbiedingsverplichting is een specifiek soort Verbintenis.
  skos:broader begrip:Verbintenis ;

  # Associatie: Gerelateerd aan de overeenkomst waaruit het voortkomt.
  skos:related begrip:Overeenkomst .

begrip:heeftAlsDrager
  a skos:Concept ;
  skos:inScheme vocab:JuridischBegrippenkader ;
  rov:status rov:stabiel ;
  dcterms:identifier "JBK-heeftAlsDrager"^^xsd:string ;
  skos:prefLabel "heeft als drager"@nl ;
  skos:definition "Een relatie die aangeeft welke (rechts)persoon de drager is van een verplichting."@nl .

  # Hiërarchie: Dit is een specifiek soort algemene relatie.
  skos:broader begrip:HeeftRelatieMet ;

  # Associatie: Deze relatie verbindt de concepten die het domein en bereik vormen.
  skos:related begrip:Aanbieder, begrip:Aanbiedingsverplichting .

**USER APPROVAL VERPLICHT:**
Gebruiker keurt elke OWL instance goed voordat toevoeging aan de Knowledge Graph plaatsvindt.

## STAP 10: Knowledge Graph Update & Finalisatie

**MANDATORY EXECUTION SEQUENCE:**
GEEN STAP VOLTOOid TOT ALLE SUBSTAPPEN AFGEROND
- 10a: User Oversight Presentatie (eerst overzicht tonen)
- 10b: User Toestemming Verkrijgen (dan toestemming vragen)
- 10c: KG Update Executie (ALLEEN dan uitvoeren)

**STAP 10a: User Oversight Presentatie**
**Doel:** Complete onderwerp presentatie van verwachte KG updates (NIET UITVOEREN)

**Vereisten:**
- Complete overzicht presenteren van nieuwe elementen
- Aantal nieuwe instanties, relaties, impact tonen
- Validatie resultaten communiceren
- NIET de update uitvoeren

**OUTPUT:** Gebruikersinformatie GEGEVEN

**STAP 10b: User Toestemming Verkrijgen**
**Doel:** Expliciete toestemming verkrijgen voor KG modificaties

**Vereisten:**
- Velde gebruikerskeuze vragen
- Wacht op "ja/nee" reactie
- Log user voor audit trail
- VERBOD: Ga NIET verder naar update zonder toestemming

**CONTROLE:** User response QUOTA ontvangen

**STAP 10c: KG Update Executie**
**Doel:** Update de Knowledge Graph NA toestemming (MANDATORY) en sla de wijzigingen op in het bestand (docs\legal-knowledge-graph.ttl).

**Proces:** (ALLEEN UITVOEREN NA STAP 10a + 10b VOLTOOID)
1. **Backup maken** van huidige KG (zelfde bestandsnaam blijft actief)
2. **Nieuwe triples toevoegen** aan bestaande graph
3. **Consistency validatie** uitvoeren
4. **Merge operatie** uitvoeren
5. **Success/failure rapporteren** aan gebruiker

**PRECONDITIES:** Stap 10a beeindigend en stap 10b toestemming verkregen

---

# SUCCESS METRICS

**Minimale Vereisten:**
- Alle 5 rondes succesvol doorlopen
- Minimaal 3 verschillende primaire ontologie mappings
- Hoog proximity scores (≥150) voor concept merges
- KG blijft OWL consistent na update
- User approval voor alle critical stappen

**Quality Assurance:**
- Rich semantic documentation in rdfs:comment
- Complete Nederlandse EN Engelse metadata
- Cross-reference traces voor audit trail
- Backup recovery capability

---

# ERROR HANDLING

**Recovery Points:**
- Step 4: Na primaire mapping validatie
- Step 7: Na secundaire ontologie validatie
- Step 10: Na KG update

**Rollback Strategy:**
Incremental rollback mogelijk naar recovery points

**Critical Failures:**
Stop uitvoeren en rapporteer aan gebruiker voor manual intervention

---

# Gebruiker Interaction Patterns

**USER APPROVAL NOTIFICATIES:**
- `[ALERT]Nieuwe juridische concept geïdentificeerd - keur goed?`
- `[DECISION]Concept merge aangeboden - extend/merge/new?`
- `[VALIDATION]Ontologische conflict gedetecteerd - oplossen?`
- `[CONFIRMATION]KG update voorgesteld - proceed?`

**Gebruiker Kan Altijd:**
- Stop workflow op elk punt
- Keer terug naar vorige stap
- Pas Nederlandse termen aan
- Override automatische beslissingen
- Vraag extra uitleg over ontologische interpretaties
