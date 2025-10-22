<critical>The workflow execution engine is governed by: {project_root}/bmad/core/tasks/workflow.xml</critical>
<critical>You MUST have already loaded and processed: {installed_path}/workflow.yaml</critical>
<critical>LegalAnalyst MUST study all Tonto guidance files before proceeding with comparison</critical>

<workflow>

<step n="1" goal="Comparison input collection - Multi-article setup">
<action>Collect multiple legal articles for comprehensive Tonto-based comparison analysis</action>
<ask>Provide comparison details with OntologyBasis context awareness:
1. Number of articles to compare (minimum 2, recommended 3-5 for meaningful comparisons)
2. Full text or references for each article
3. Legal jurisdiction context and comparison scope
4. Comparison focus areas:
   - overlaps (gedeelde concepten)
   - conflicts (tegenstrijdigheden)
   - relations (cross-article verbanden)
   - evolution (hoe concepten zich ontwikkelen)
   - all (comprehensive analysis)</ask>
<critical>Validate minimum 2 articles and informed comparison scope</critical>
<critical>Prepare for cross-ontology pattern recognition across all articles</critical>
<template-output>comparison_setup</template-output>
</step>

<step n="1.5" goal="Tonto Knowledge Acquisition - VERPLICHT voor vergelijkende analyses">
<action>CRITICAL: LegalAnalyst MOET alle Tonto guidance bestanden laden en bestuderen</action>
<action>Laad de volgende Tonto guidance bestanden voor comparative analysis expertise:</action>
<subaction>tonto_llm_documentation_guide.instructions.md</subaction>
<subaction>tonto_llm_guidance.instructions.md</subaction>
<subaction>tonto_llm_terminology_analysis_guide.instructions.md</subaction>
<subaction>tonto_llm_understanding_and_summarization_guide.instructions.md</subaction>
<subaction>tonto-cardinality-guidance.instructions.md</subaction>
<subaction>tonto-guidance.instructions.md</subaction>
<subaction>tonto-llm-create-new-elements.instructions.md</subaction>
<action>Integreer Tonto kennis voor comparative analysis:</action>
<subaction>Consistent mapping across multiple articles</subaction>
<subaction>Cross-article terminology harmonization</subaction>
<subaction>Ontological pattern recognition tussen artikelen</subaction>
<subaction>Comprehensive Tonto documentation standards</subaction>
<critical>LegalAnalyst mag NIET verdergaan zonder volledige Tonto expertise voor comparative analysis</critical>
</step>

<step n="2" goal="Complete OntologyBasis Loading - Comprehensive comparison framework">
<action>Load ALL OntologyBasis ontologieën (13 bestanden) als complete comparative framework</action>
<action>Voer cross-ontology analysis uit voor comparative capabilities:</action>
<subaction>LegalOntology.tonto - Rechtsbetrekkingen voor conflict/overlap analyse</subaction>
<subaction>ObjectOntology.tonto - NormativeDescription voor regelvergelijking</subaction>
<subaction>LawOntology.tonto - Wet structuur voor hiërarchische vergelijking</subaction>
<subaction>AgentOntology.tonto - Actoren voor rechtssubject vergelijking</subaction>
<subaction>EventOntology.tonto - Gebeurtenissen voor procedurele verschillen</subaction>
<subaction>ModeOntology.tonto - Intenties voor motivationele analyse</subaction>
<subaction>ValueOntology.tonto - Waarden voor impact assessment</subaction>
<subaction>Alle andere ontologieën voor complete context</subaction>
<action>Identificeer comparative analysis patterns en cross-ontology linkages</action>
<action>Maak geïntegreerde comparative ontologische context voor multi-article analyse</action>
<template-output>ontology_familiarization</template-output>
</step>

<step n="2.1" goal="Load Existing Tonto Knowledge Graph - VERPLICHT voor vergelijkende analyses">
<critical>CRITICAL: LOAD bestaande Tonto Knowledge Graph FIRST - dit is de foundation voor comparative analysis</critical>
<action>Bepaal Knowledge Graph locatie: {project-root}/docs/legal-knowledge-graph.tonto</action>
<check if="file does not exist">
<action>Creëer lege basisstructuur voor nieuwe comparative Knowledge Graph</action>
<action>Documenteer: "Nieuwe comparative Knowledge Graph aangemaakt voor multi-article analyse"</action>
</check>
<check if="file exists">
<action>LOAD complete bestaande Tonto Knowledge Graph</action>
<action>Parse alle bestaande concepten, relaties en cross-referenties</action>
<action>Maak comparative analysis capabilities beschikbaar voor cross-article validatie</action>
<action>Documenteer: "Bestaande Knowledge Graph geladen met X concepten voor comparative enhancement"</action>
</check>
<action>Stel Knowledge Graph beschikbaar als foundation voor inter-article comparisons</action>
<critical>LegalAnalyst: Elke comparative analyse bouwt voort op bestaande juridische kennis voor diepere inzichten</critical>
<template-output>knowledge_graph_status</template-output>
</step>

<step n="3" goal="Primaire juridische kern mapping per artikel - Hiërarchische aanpak">
<critical>VERPLICHT: Start comparative analysis ALTIJD met individuele juridische kern mappings</critical>
<action>Voer primaire juridische kern mapping uit voor ELK artikel apart:</action>
<subaction>LegalOntology.tonto: Rechtsbetrekkingen, rechtssubjecten, rechtsobjecten</subaction>
<subaction>ObjectOntology.tonto: NormativeDescription, Norm types</subaction>
<subaction>LawOntology.tonto: Article, Chapter, Law structuren</subaction>
<for-each article="comparison_articles">
<action>Primaire mapping per artikel:</action>
<subaction>Map naar juridische kern concepten (LegalOntology eerst)</subaction>
<subaction>Valideer tegen LawOntology structuren</subaction>
<subaction>Toepas ObjectOntology voor normatieve elementen</subaction>
<subaction>Gebruik Tonto expertise voor consistente stereotyping</subaction>
</for-each>
<template-output>primary_article_mappings</template-output>
</step>

<step n="3A" goal="Secundaire context mapping per artikel - Cross-ontology enrichment">
<critical>Secundair: Voeg cross-ontology context toe aan elke individuele artikel mapping</critical>
<action>Voer secundaire cross-ontology mapping uit voor ELK artikel:</action>
<subaction>AgentOntology: Actoren identificeren (NaturalPerson, LegalPerson, GovernmentBody)</subaction>
<subaction>EventOntology: Gebeurtenissen en temporaliteit (InstitutionalAct, time sequences)</subaction>
<subaction>ModeOntology: Intenties en verplichtingen (SocialCommitment, motivations)</subaction>
<subaction>ValueOntology: Waardebepalingen (ValueBearer, impact assessments)</subaction>
<action>Cross-ontology Integration per artikel:</action>
<subaction>LegalSubject rol linking: Citizens → NaturalPerson → Claimant/LegalSubject</subaction>
<subaction>Organizational actors: GovernmentBody → LegalSubject in governance context</subaction>
<subaction>Economic aspects: ValueBearer → LegalObject in financial contexts</subaction>
<subaction>Temporal sequences: InstitutionalAct → Event chains in procedures</subaction>
<template-output>secondary_article_mappings</template-output>
</step>

<step n="4" goal="Inter-article comparative analysis - Kern juridische concepten">
<critical>Nu pas inter-article vergelijking uitvoeren met volledige ontologische context</critical>
<action>Voer hiërarchische comparative analysis uit tussen artikelen:</action>
<subaction>Niveau 1 - Primaire kern: Rechtsbetrekkingen overlaps/conflicten</subaction>
<subaction>Niveau 2 - Structuur: Wet hiërarchieën en artikel relaties</subaction>
<subaction>Niveau 3 - Cross-ontology: Actoren, waarden, gebeurtenissen</subaction>
<action>Identificeer comparative patterns:</action>
<subaction>Exact concept matches tussen artikelen</subaction>
<subaction>Semantische equivalences met verschillende terminologie</subaction>
<subaction>Taxonomic relationships (specialisatie/generalizatie)</subaction>
<subaction>Complementaire concepten (elkaar versterkend)</subaction>
<template-output>comparative_concept_analysis</template-output>
</step>

<step n="4A" goal="Conflict en consistentie analyse - Multi-perspective validatie">
<critical>Multi-perspective conflict detectie met complete OntologyBasis</critical>
<action>Analyseer conflicts en consistenties tussen artikelen:</action>
<subaction>Juridische kern conflicts: Tegenstrijdige rechten/verplichtingen</subaction>
<subaction>Procedurele incompatibiliteiten: Conflicterende InstitutionalAct sequences</subaction>
<subaction>Actor conflicts: Tegenstrijdige GovernmentBody rollen</subaction>
<subaction>Waarde conflicts: Inconsistente ValueBearer toepassingen</subaction>
<action>Systeem consistentie validatie:</action>
<subaction>Ontologische constraints: UFO-L constraint violations</subaction>
<subaction>Cross-ontology referenties: Broken linkages tussen concepten</subaction>
<subaction>Temporaliteit conflicts: Onverenigbare InstitutionalAct sequenties</subaction>
<template-output>comprehensive_conflict_analysis</template-output>
</step>

<step n="4.5" goal="CROSS-VALIDATION tegen Existing Tonto Knowledge Graph - Inter-article enrichment">
<critical>CRITICAL: Voer cross-validaties uit tegen GELADEN Tonto Knowledge Graph voor comparative insights</critical>
<action>Integreer comparative findings met bestaande juridische kennis:</action>
<subaction>Direct Match Validation: Nieuwe comparative insights tegen bestaande concepten</subaction>
<subaction>Extension Opportunities: Comparative analysis reveal nieuwe aspecten van bestaande concepten</subaction>
<subaction>Gap Analysis: Ontbrekende cross-article verbanden in bestaande Knowledge Graph</subaction>
<action>User Decisions voor Knowledge Graph Enhancement:</action>
<subaction>"Comparative analysis toont nieuwe aspect van bestaand concept X. Uitbreiden? [ja/nee/selectief]"</subaction>
<subaction>"Nieuw cross-article verband geïdentificeerd tussen bestaande concepten Y en Z. Toevoegen?"</subaction>
<subaction>"Comparative analysis conflicteert met bestaande definitie. Harmoniseren?"</subaction>
<critical>LegalAnalyst: Comparative analysis ENRICHT de bestaande Knowledge Graph met multi-article insights</critical>
<template-output>comprehensive_cross_validation</template-output>
</step>

<step n="5" goal="Inter-article relatie analyse - Comprehensive mapping">
<action>Analyze relations tussen artikelen met complete ontologische context</action>
<action>Identificeer inter-article relation types:</action>
<subaction>Complementaire relaties: Concepten die elkaar ondersteunen</subaction>
<subaction>Conflicterende relaties: Tegenstrijdige juridische posities</subaction>
<subaction>Evolutionaire relaties: Hoe concepten evolueren tussen artikelen</subaction>
<subaction>Preconditionele relaties: Voorwaarden tussen verschillende artikelen</subaction>
<template-output>inter_article_relations</template-output>
</step>

<step n="6" goal="Tonto Model Instantiation met Knowledge Graph Integration - Comparative synthesis">
<action>CRITICAL: Load bestaande Tonto Knowledge Graph FIRST - integreer comparative insights</action>
<action>Syntheseer comparative findings in geïntegreerde Tonto model updates:</action>
<subaction>Nieuwe cross-article concepten: Comparative analysis reveals</subaction>
<subaction>Concept expansions: Existing concepts krijgen nieuwe comparative dimensies</subaction>
<subaction>Relation enhancements: Cross-article linkages geïdentificeerd</subaction>
<action>Interactive comparative model building:</action>
<subaction>"Comparative analysis toont concept cluster tussen artikelen A, B, C. Nieuwe cluster aanmaken?"</subaction>
<subaction>"Evolution pattern geïdentificeerd: Concept X ontwikkelt van artikel 1 naar artikel 2. Uitbreiden?"</subaction>
<action>MERGE comprehensive comparative model met bestaande Knowledge Graph</action>
<template-output>comprehensive_model_synthesis</template-output>
</step>

<step n="6.6" goal="Knowledge Graph Maintenance en Comparative Documentation">
<critical>CRITICAL: Zorg voor Knowledge Graph integriteit na comparative enhancements</critical>
<action>Documenteer alle comparative additions:</action>
<subaction>Cross-article verbanden toegevoegd</subaction>
<subaction>Bestaande concepten uitgebreid met comparative insights</subaction>
<subaction>Conflict resoluties vastgelegd</subaction>
<subaction>Evolution patterns gedocumenteerd</subaction>
<action>Version control en archiving:</action>
<subaction>Creeer backup van pre-comparative state</subaction>
<subaction>Documenteer comparative methodology gebruikt</subaction>
<subaction>Update metadata met multi-article scope</subaction>
<template-output>comparative_maintenance_report</template-output>
</step>

<step n="7" goal="Cross-Ontology Integration Validatie - Post-comparative">
<action>Valideer comparative model tegen alle OntologyBasis ontologieën</action>
<action>Controleer cross-ontology consistentie en referenties</action>
<action>Zorg voor juiste Tonto syntax volgens alle guidance bestanden</action>
<action>Valideer comparative logic: Is de synthesis ontologisch sound?</action>
<template-output>integration_validation_comprehensive</template-output>
</step>

<step n="8" goal="Tonto Model Validatie - Comparative compliance">
<action>Valideer comparative Tonto model syntax en ontologische consistentie</action>
<action>Controleer stereotyping volgens Tonto guidance</action>
<action>Valideer comparative cardinalities en cross-article relations</action>
<action>Controleer terminology volgens terminology analysis guide</action>
<template-output>comprehensive_validation</template-output>
</step>

<step n="9" goal="Tonto Knowledge Graph Update and Comparative Report">
<action>Genereer comprehensive comparative rapport met alle Knowledge Graph enhancements</action>
<action>Documenteer cross-ontology synthesis en comparative insights</action>
<action>Beoordeel kwaliteit van multi-article analysis en comparative model</action>
<action>Toon final integrated comparative model voor review</action>
<template-output>comprehensive_comparative_report</template-output>
</step>

</workflow>
