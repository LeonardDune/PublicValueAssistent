<critical>The workflow execution engine is governed by: {project_root}/bmad/core/tasks/workflow.xml</critical>
<critical>You MUST have already loaded and processed: {installed_path}/workflow.yaml</critical>
<critical>LegalAnalyst MUST study all Tonto guidance files before proceeding with terminology work</critical>

<workflow>

<step n="1" goal="Complete OntologyBasis Glossary Setup - Comprehensive scope">
<action>Initialize comprehensive glossary maintenance met complete OntologyBasisontologieën context</action>
<ask>Specify comprehensive glossary maintenance scope met cross-ontology awareness:
1. Update frequency (real-time, daily, weekly, monthly, on-demand)
2. Maintenance type (full OntologyBasis update, incremental, targeted ontology domain, cross-ontology relations)
3. Source legislation domains EN cross-ontology concepten
4. Target audience (general public, legal professionals, ontologists, academics, system developers)
5. Output format (ontological hierarchy, alphabetical, categorical, cross-ontology matrix, Tonto-integrated)
6. Integration type (standalone glossary, Knowledge Graph integrated, Tonto model embedded)</ask>
<critical>Valideer scope tegen beschikbare OntologyBasis ontologieën en Tonto capabilities</critical>
<critical>Prepare voor cross-ontology terminology harmonization across all 13 ontologieën</critical>
<template-output>comprehensive_glossary_setup</template-output>
</step>

<step n="1.5" goal="Tonto Knowledge Acquisition - VERPLICHT voor terminology expertise">
<action>CRITICAL: LegalAnalyst MOET alle Tonto guidance bestanden laden en bestuderen</action>
<action>Laad de volgende Tonto guidance bestanden voor comprehensive terminology work:</action>
<subaction>tonto_llm_documentation_guide.instructions.md - Voor professionele glossary documentatie</subaction>
<subaction>tonto_llm_guidance.instructions.md - Voor ontologische terminology correctness</subaction>
<subaction>tonto_llm_terminology_analysis_guide.instructions.md - Voor terminology analysis en harmonization</subaction>
<subaction>tonto_llm_understanding_and_summarization_guide.instructions.md - Voor concept comprehension</subaction>
<subaction>tonto-cardinality-guidance.instructions.md - Voor relation terminology</subaction>
<subaction>tonto-guidance.instructions.md - Voor stereotyping en naming conventions</subaction>
<subaction>tonto-llm-create-new-elements.instructions.md - Voor terminology extensions</subaction>
<action>Integreer Tonto kennis voor comprehensive terminology management:</action>
<subaction>Cross-ontology terminology harmonization</subaction>
<subaction>Ontological concept clarity volgens UFO principles</subaction>
<subaction>Tonto documentation standards voor definitions</subaction>
<subaction>Terminology analysis voor semantic consistency</subaction>
<critical>LegalAnalyst mag NIET verdergaan zonder volledige Tonto expertise voor terminology work</critical>
</step>

<step n="2" goal="Complete OntologyBasis Term Extraction - Comprehensive harvest">
<action>Extract ALL termen uit alle 13 OntologyBasis ontologieën systematisch</action>
<action>Voer cross-ontology term extraction uit:</action>
<subaction>LegalOntology.tonto: 60+ juridische concepten (Rights, Duties, LegalRelator, etc.)</subaction>
<subaction>ObjectOntology.tonto: Normatieve concepten (NormativeDescription, Permission, Obligation, etc.)</subaction>
<subaction>LawOntology.tonto: Wet structuur termen (Law, Article, Chapter, etc.)</subaction>
<subaction>AgentOntology.tonto: Actor termen (NaturalPerson, GovernmentBody, SocialAgent, etc.)</subaction>
<subaction>EventOntology.tonto: Gebeurtenis termen (InstitutionalAct, CommunicativeAct, etc.)</subaction>
<subaction>ModeOntology.tonto: Intentionele termen (SocialCommitment, SocialClaim, etc.)</subaction>
<subaction>ValueOntology.tonto: Waarde termen (ValueBearer, ValueAscription, etc.)</subaction>
<subaction>All other ontologies: Complete terminology coverage</subaction>
<action>Cross-ontology categorization by ontological type:</action>
<subaction>Sortal terms (kinds, subkinds, phases, roles)</subaction>
<subaction>Non-sortal terms (categories, mixins, roleMixins, modes)</subaction>
<subaction>Relation terms (associations, aggregations, compositions)</subaction>
<subaction>Attribute terms (properties, meta-properties, derived values)</subaction>
<subaction>Cross-ontology linkage terms (mediation, characterization, participation)</subaction>
<template-output>comprehensive_term_extraction</template-output>
</step>

<step n="2.1" goal="Load Existing Tonto Knowledge Graph - VERPLICHT voor terminology context">
<critical>CRITICAL: LOAD bestaande Tonto Knowledge Graph FIRST - voor terminology enrichment</critical>
<action>Bepaal Knowledge Graph locatie: {project-root}/docs/legal-knowledge-graph.tonto</action>
<check if="file does not exist">
<action>Creëer lege basisstructuur voor nieuwe terminology Knowledge Graph</action>
<action>Documenteer: "Nieuwe comprehensive glossary Knowledge Graph aangemaakt"</action>
</check>
<check if="file exists">
<action>LOAD complete bestaande Tonto Knowledge Graph</action>
<action>Parse alle bestaande concepten voor terminology validation</action>
<action>Maak existing terminology beschikbaar voor harmonization</action>
<action>Documenteer: "Bestaande Knowledge Graph geladen voor terminology enhancement"</action>
</check>
<action>Stel terminology Knowledge Graph beschikbaar als foundation voor comprehensive glossary</action>
<critical>LegalAnalyst: Comprehensive glossary building ENRICHT de bestaande juridische kennisbasis</critical>
<template-output>terminology_knowledge_graph_status</template-output>
</step>

<step n="3" goal="Existing Glossary Analysis - Knowledge Graph integration">
<action>Load en analyseer huidige glossary indien aanwezig (Tonto geïntegreerd of standalone)</action>
<check if="existing_glossary exists and is Tonto-integrated">
<action>Parse Tonto model structure and cross-references</action>
<action>Compare met recente OntologyBasis terminology updates</action>
<action>Identify semantic gaps, outdated definitions en nieuwe cross-ontology termen</action>
<action>Valideer tegen loaded Knowledge Graph voor consistency</action>
</check>
<check if="existing_glossary exists but not Tonto-integrated">
<action>Assess migratiemogelijkheden naar Tonto format</action>
<action>Cross-reference met OntologyBasis voor ontologische validatie</action>
<action>Identify modernization opportunities</action>
</check>
<check if="no existing_glossary">
<action>Initialize comprehensive Tonto-based glossary structure</action>
<action>Create ontological categorization framework (volgens UFO principles)</action>
<action>Setup cross-ontology reference system</action>
</check>
<template-output>comprehensive_glossary_analysis</template-output>
</step>

<step n="4" goal="Primaire juridische kern term definitions - UFO foundation">
<critical>VERPLICHT: Start ALTIJD met juridische kern terminology definitions</critical>
<action>Genereer definitions voor primaire juridische kern termen:</action>
<subaction>LegalOntology termen: Complete UFO-L definitions (Rights, Duties, LegalRelator, etc.)</subaction>
<subaction>ObjectOntology normen: Precise rule definitions (Permission, Prohibition, Obligation)</subaction>
<subaction>LawOntology structuren: Wet hierarchy definitions (Law, Article, LegalSection)</subaction>
<action>Tonto documentation standards toepassen per definitie:</action>
<subaction>@en en @nl labels volgens documentation guide</subaction>
<subaction>Ontologische foundations (UFO stereotypes) expliciet</subaction>
<subaction>Cross-ontology context waar relevant</subaction>
<subaction>Voorbeelden en counter-voorbeelden volgens guidance</subaction>
<subaction>Semantische clarity volgens terminology analysis guide</subaction>
<template-output>primary_terminology_definitions</template-output>
</step>

<step n="4A" goal="Secundaire cross-ontology term definitions - Complete context">
<critical>Secundair: Breid uit met alle cross-ontology terminology voor complete coverage</critical>
<action>Genereer definitions voor alle secundaire ontologie termen:</action>
<subaction>AgentOntology actoren: NaturalPerson, GovernmentBody, LegalPerson definitions</subaction>
<subaction>EventOntology gebeurtenissen: InstitutionalAct, CommunicativeAct definitions</subaction>
<subaction>ModeOntology intenties: SocialCommitment, SocialClaim definitions</subaction>
<subaction>ValueOntology waarden: ValueBearer, ValueAscription definitions</subaction>
<subaction>Alle andere ontologies: Complete terminology coverage</subaction>
<action>Cross-ontology integration in definitions:</action>
<subaction>Agent rollen in juridische context beschrijven</subaction>
<subaction>Event participation in legal relations verklaren</subaction>
<subaction>Mode inherence in legal positions beschrijven</subaction>
<subaction>Value aspects in legal objects verklaren</subaction>
<template-output>secondary_terminology_definitions</template-output>
</step>

<step n="5" goal="Comprehensive Term Organization - Ontological + Cross-ontology categorization">
<action>Organiseer alle termen in coherente comprehensive categorieën met cross-ontology awareness</action>
<action>Tonto-gebaseerde classificatie systemen:</action>
<subaction>By ontological type: Sortals (kinds, roles, phases), Non-sortals (categories, mixins), Perdurants (events, situations)</subaction>
<subaction>By cross-ontology relations: Mediation terms, Characterization terms, Participation terms, etc.</subaction>
<subaction>By legal domain: Civil, criminal, administrative, constitutional (extended with cross-ontology)</subaction>
<subaction>By functional role: Rights, duties, powers, subjections, obligations, permissions (all ontologies)</subaction>
<subaction>By complexity: Basic (single ontology), Intermediate (dual ontology), Advanced (multi-ontology relations)</subaction>
<action>Generate comprehensive cross-references:</action>
<subaction>Intra-ontology relations (binnenzelfde ontologie)</subaction>
<subaction>Inter-ontology relations (tussen verschillende ontologieën)</subaction>
<subaction>Legal integration linkages (hoe termen juridisch functioneren)</subaction>
<template-output>comprehensive_term_organization</template-output>
</step>

<step n="6" goal="Cross-Validation tegen Tonto Knowledge Graph - Terminology harmonization">
<critical>CRITICAL: Voer terminology cross-validaties uit tegen GELADEN Tonto Knowledge Graph</critical>
<action>Harmonizeer terminology tegen bestaande juridische kennis:</action>
<subaction>Term consistency: Nieuwe definitions vs bestaande Knowledge Graph</subaction>
<subaction>Semantic gaps: Identificeer ontbrekende cross-references</subaction>
<subaction>Definition conflicts: Los terminology disagreements op</subaction>
<subaction>Integration opportunities: Nieuwe termen die bestaande kennis uitbreiden</subaction>
<action>User Decisions voor terminology harmonization:</action>
<subaction>"Nieuwe definitie conflicteert met bestaande KG definitie. Harmoniseren? [nieuwe-definitie/behoud/OntologyBasis-reference]"</subaction>
<subaction>"Ontbrekende cross-ontology relatie geïdentificeerd tussen termen A en B. Toevoegen?"</subaction>
<subaction>"Terminology uitbreiding geïdentificeerd voor bestaand concept. Uitbreiden?"</subaction>
<critical>LegalAnalyst: Comprehensive glossary building HARMONISEERT terminology across complete OntologyBasis</critical>
<template-output>comprehensive_terminology_validation</template-output>
</step>

<step n="7" goal="Quality Assurance en Cross-Ontology Validation - Complete coverage">
<action>Valideer comprehensive glossary compleetheid, accuracy en cross-ontology integration</action>
<action>Multi-perspective quality assessment:</action>
<subaction>Ontological completeness: Alle 13 OntologyBasis ontologieën covered</subaction>
<subaction>Definition clarity: Tonto documentation standards toegepast</subaction>
<subaction>Terminology consistency: Harmonized across ontologies volgens Tonto guidance</subaction>
<subaction>Cross-ontology references: Complete linkage system</subaction>
<subaction>Audience appropriateness: Professional legal + ontologische expertise</subaction>
<subaction>Tonto compliance: Syntax, stereotyping, cardinality rules</subaction>
<template-output>comprehensive_quality_assurance</template-output>
</step>

<step n="8" goal="Comprehensive Glossary Formatting met Tonto Integration">
<action>Apply comprehensive formatting and Tonto-enhanced features</action>
<action>Advanced glossary features met cross-ontology integratie:</action>
<subaction>Ontological hierarchy presentation (UFO-compliant categorization)</subaction>
<subaction>Cross-ontology relation visualization</subaction>
<subaction>Interactive Tonto model linkages</subaction>
<subaction>Search index met ontologische filters</subaction>
<subaction>Usage examples met ontologische context</subaction>
<subaction>Legal source references + OntologyBasis mappings</subaction>
<subaction>Tonto Knowledge Graph integration metadata</subaction>
<subaction>Version history met ontologische changes</subaction>
<template-output>comprehensive_glossary_formatting</template-output>
</step>

<step n="9" goal="Tonto Model Integration met Knowledge Graph Expansion - Comprehensive synthesis">
<action>CRITICAL: Load bestaande Tonto Knowledge Graph FIRST - integreer comprehensive terminology</action>
<action>Syntheseer comprehensive glossary in Tonto model met Knowledge Graph expansion:</action>
<subaction>Nieuwe terminology concepten: Comprehensive glossary reveals</subaction>
<subaction>Definition expansions: Existing concepten krijgen enhanced terminology</subaction>
<subaction>Relation enhancements: Cross-ontology terminology linkages</subaction>
<action>Interactive terminology Tonto model building:</action>
<subaction>"Comprehensive glossary toont nieuwe terminology cluster tussen ontologieën A, B, C. Nieuwe cluster aanmaken?"</subaction>
<subaction>"Enhanced definition geïdentificeerd voor bestaand concept X. Bijwerken?"</subaction>
<action>MERGE comprehensive terminology model met bestaande Knowledge Graph</action>
<template-output>comprehensive_terminology_synthesis</template-output>
</step>

<step n="9.6" goal="Knowledge Graph Maintenance en Terminology Documentation">
<critical>CRITICAL: Zorg voor Knowledge Graph integriteit na comprehensive terminology additions</critical>
<action>Documenteer alle terminology additions:</action>
<subaction>Cross-ontology termen toegevoegd</subaction>
<subaction>Bestaande concepten uitgebreid met enhanced definitions</subaction>
<subaction>Terminology harmonizations vastgelegd</subaction>
<subaction>Ontological categorization verbeterd</subaction>
<action>Version control en archiving:</action>
<subaction>Creeer backup van pre-terminology state</subaction>
<subaction>Documenteer comprehensive terminology methodology gebruikt</subaction>
<subaction>Update metadata met complete OntologyBasis scope</subaction>
<template-output>comprehensive_terminology_maintenance</template-output>
</step>

<step n="10" goal="Final Validation en Comprehensive Glossary Report">
<action>Genereer final comprehensive glossary rapport met alle enhancements</action>
<action>Documenteer cross-ontology terminology synthesis en ontologische verbeteringen</action>
<action>Beoordeel kwaliteit van complete OntologyBasis terminology coverage</action>
<action>Toon final integrated comprehensive glossary voor review</action>
<template-output>comprehensive_glossary_final_report</template-output>
</step>

</workflow>
