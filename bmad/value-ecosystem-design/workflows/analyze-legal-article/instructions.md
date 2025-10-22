<critical>Workflow execution governed by: {project_root}/bmad/core/tasks/workflow.xml</critical>
<critical>Tonto-modellen voor analyse, OWL output met ob: verwijzingen naar OntologyBasis.ttl</critical>

<workflow>

<step n="1" goal="Laad alle OntologyBasis Tonto-modellen voor juridische expertise">
<action>CRITICAL: Load alle 13 OntologyBasis .tonto bestanden voor volledige ontologische context</action>
<action>Laad deze Tonto-modellen als expert kennisbasis:</action>
<subaction>AgentOntology.tonto - Agent concepten, NaturalPerson, LegalPerson, GovernmentBody rollen</subaction>
<subaction>LegalOntology.tonto - LegalRelator, Right, Duty, Claimant, Committor concepten</subaction>
<subaction>ObjectOntology.tonto - NormativeDescription, LegalDocument, Permission/Prohibition/Obligation</subaction>
<subaction>LawOntology.tonto - Law, Article, LegalSection hiërarchie</subaction>
<subaction>EventOntology.tonto - InstitutionalAct, CommunicativeAct concepten</subaction>
<subaction>ModeOntology.tonto - SocialCommitment, SocialClaim, Intention concepten</subaction>
<subaction>ValueOntology.tonto - PublicValue, BusinessValue, ValueBearer concepten</subaction>
<subaction>DEMOOntology.tonto - Transaction, CoordinationAct, ProductionFact concepten</subaction>
<subaction>IndividualOntology.tonto - Quality concepten</subaction>
<subaction>Andere ontologieën - voor cross-ontology verbanden</subaction>
<action>Maak complete ontologische context beschikbaar voor analyse</action>
<critical>LegalAnalyst mag NIET beginnen zonder volledige Tonto expertise geladen</critical>
<template-output>ontology_tonto_loaded</template-output>
</step>

<step n="1.5" goal="Legal article input collection">
<action>Gather legal article information from user</action>
<ask>Provide the legal article details:
1. Full article text or reference
2. Legal jurisdiction (e.g., Dutch, EU, international)
3. Article reference/ID (e.g., Article 12, §34)
4. Context (law name, purpose, domain)</ask>
<critical>Store article content and metadata for analysis</critical>
<template-output>article_details</template-output>
</step>

<step n="1.5" goal="Tonto Knowledge Acquisition - VERPLICHT">
<action>CRITICAL: LegalAnalyst MOET alle Tonto guidance bestanden laden en bestuderen</action>
<action>Laad de volgende Tonto guidance bestanden:</action>
<subaction>tonto_llm_documentation_guide.instructions.md</subaction>
<subaction>tonto_llm_guidance.instructions.md</subaction>
<subaction>tonto_llm_terminology_analysis_guide.instructions.md</subaction>
<subaction>tonto_llm_understanding_and_summarization_guide.instructions.md</subaction>
<subaction>tonto-cardinality-guidance.instructions.md</subaction>
<subaction>tonto-guidance.instructions.md</subaction>
<subaction>tonto-llm-create-new-elements.instructions.md</subaction>
<action>Integreer Tonto kennis voor:</action>
<subaction>Correct Tonto syntax in alle outputs</subaction>
<subaction>Proper ontologische concepten en stereotypen</subaction>
<subaction>Terminology analysis volgens Tonto standards</subaction>
<subaction>Documentatie in professionele Tonto format</subaction>
<subaction>Cardinality rules voor relaties</subaction>
<subaction>Guidance voor nieuwe elementen creatie</subaction>
<critical>LegalAnalyst mag NIET verdergaan zonder volledige Tonto expertise</critical>
</step>

<step n="2" goal="Complete OntologyBasis Loading and Cross-Ontology Analysis">
<action>Load ALL OntologyBasis ontologieën (13 bestanden) als complete context</action>
<action>Voer cross-ontology analyse uit:</action>
<subaction>AgentOntology.tonto - Agent, Role, SocialAgent concepten</subaction>
<subaction>EventOntology.tonto - Event, Action, Participation concepten</subaction>
<subaction>ModeOntology.tonto - Intention, Belief, SocialMoment concepten</subaction>
<subaction>ObjectOntology.tonto - Object, NormativeDescription, LegalDocument</subaction>
<subaction>LegalOntology.tonto - LegalRelator, Right, Duty, Power concepten</subaction>
<subaction>LawOntology.tonto - Law, Article, LegalSection hiërarchie</subaction>
<subaction>Value ontologies - Value, ValueBearer, ValueAscription concepten</subaction>
<subaction>DEMOOntology.tonto - Transaction, ActorRole patronen</subaction>
<action>Identificeer cross-ontology relaties en afhankelijkheden</action>
<action>Maak geïntegreerde ontologische context voor juridische analyse</action>
<template-output>ontology_familiarization</template-output>
</step>

<step n="2.1" goal="Load Existing OWL Knowledge Graph - VERPLICHT VOOR ELKE ANALYSE">
<critical>CRITICAL: LOAD bestaande OWL Knowledge Graph FIRST - dit is de iteratieve juridische kennisbasis</critical>
<action>Bepaal Knowledge Graph locatie: {project-root}/docs/legal-owl-knowledge-graph.ttl</action>
<check if="file does not exist">
<action>Creëer lege basisstructuur voor nieuwe Knowledge Graph</action>
<action>Documenteer: "Nieuwe Knowledge Graph aangemaakt - eerste analyse in serie"</action>
</check>
<check if="file exists">
<action>LOAD complete bestaande OWL Knowledge Graph</action>
<action>Parse alle bestaande instanties, relaties en cross-referenties</action>
<action>Maak geïntegreerde kennisbasis beschikbaar voor cross-validatie</action>
<action>Documenteer: "Bestaande Knowledge Graph geladen met X instanties"</action>
</check>
<action>Stel Knowledge Graph beschikbaar als referentie voor alle volgende stappen</action>
<critical>LegalAnalyst: Elke nieuwe analyse breidt deze Knowledge Graph uit, voegt nieuwe instanties toe EN aanvullingen aan bestaande instanties</critical>
<template-output>knowledge_graph_status</template-output>
</step>

<step n="3" goal="Article surface analysis">
<action>Analyze article text for legal concepts</action>
<action>Identify potential mappings to existing LegalOntology concepts</action>
<template-output>initial_analysis</template-output>
</step>

<step n="4" goal="Primaire ontologische concept mapping naar juridische kernontologieën">
<critical>VERPLICHT: Start ALTIJD met mapping naar de 3 JURIDISCHE KERNONTOLOGIEËN</critical>
<action>Map artikel concepten naar BESTAANDE concepten in PRIMAIR:</action>
<subaction>LegalOntology.tonto: Rechtsbetrekkingen, rechtssubjecten, rechtsobjecten, rechten, plichten</subaction>
<subaction>ObjectOntology.tonto: NormativeDescription, Norm (Permission, Prohibition, Obligation)</subaction>
<subaction>LawOntology.tonto: Wet structuur (Law, Article, Chapter, Paragraph)</subaction>
<action>Juridische Kern Mapping Patronen:</action>
<subaction>Artikel tekst = Article (LawOntology) bevat Norm (ObjectOntology)</subaction>
<subaction>Rechtssubjecten = LegalSubject/Claimant/Committor (LegalOntology)</subaction>
<subaction>Rechtsbetrekkingen = LegalRelator/RightDutyRelator (LegalOntology)</subaction>
<subaction>Rechten/Plichten = Right/Duty (LegalOntology)</subaction>
<action>Tonto expertise toepassen voor primary mapping:</action>
<subaction>Prompt user: "Concept X - Primary mapping naar juridische kern: Y (stereotype Z). Correct? [j/n/bewerken]"</subaction>
<subaction>If 'bewerk': Tonto guidance voor alternatieven binnen kernontologieën</subaction>
<subaction>VALIDATIE: Alle artikel concepten MOETEN eerst gemapped worden naar juridische kern</subaction>
<template-output>primary_concept_mapping</template-output>
<elicit-required>
<action>Present primary concept mappings for user validation</action>
<action>Show: mandaat → Power, bestuursorgaan → GovernmentBody, besluiten nemen → InstitutionalAct</action>
<ask>Are these primary mappings correct? [ja/nee/bewerken]</ask>
</elicit-required>
</step>

<step n="4A" goal="Secundaire context mapping naar aanvullende OntologyBasis ontologieën">
<critical>Secundair: Gebruik andere ontologieën voor context en cross-ontology relaties - ALLE relevante verbanden leggen</critical>
<action>Map secundaire context naar BESTAANDE concepten in:</action>
<subaction>AgentOntology.tonto: Actoren (NaturalPerson, LegalPerson, SocialAgent, alle roltypes)</subaction>
<subaction>EventOntology.tonto: Gebeurtenissen (InstitutionalAct, CommunicativeAct)</subaction>
<subaction>ModeOntology.tonto: Intenties, verplichtingen (SocialCommitment, SocialClaim)</subaction>
<subaction>ValueOntology.tonto: Waarden, waardebepalingen (ValueBearer, Value)</subaction>
<subaction>Alle andere OntologyBasis ontologieën: Voor specifieke cross-ontology verbanden</subaction>
<action>Cross-Ontology Integration Patronen - BREED SPEKTRUM:</action>
<subaction>LegalSubject rol gespeeld door ENIGE Agent (NaturalPerson, LegalPerson, GovernmentBody, etc.)</subaction>
<subaction>Rechtsfeit manifested via ENIGE Event (InstitutionalAct, maar ook andere gebeurtenissen)</subaction>
<subaction>Contract participant via LegalPerson of NaturalPerson (AgentOntology → alle juridische contexten)</subaction>
<subaction>Value bearer als LegalObject in rechtsbetrekkingen (ValueOntology → LegalOntology)</subaction>
<subaction>Social commitments als juridische basis voor rights/duties (ModeOntology → LegalOntology)</subaction>
<subaction>Actions en transactions in juridische context (EventOntology → LegalOntology)</subaction>
<action>Tonto expertise voor cross-ontology validatie:</action>
<subaction>Prompt user: "Cross-ontology verband gevonden: Concept X uit Y-ontology kan gekoppeld worden aan juridische context Z. Uitbreiden? [ja/nee/selectief]"</subaction>
<subaction>Voorbeelden van patronen (niet limitatief):</subaction>
<subaction>- "Burger = NaturalPerson = Claimant in Recht-op-Onderwijs relatie"</subaction>
<subaction>- "Bedrijf = PrivateLegalPerson = Committor in Belastingplicht relatie"</subaction>
<subaction>- "Contractondertekening = InstitutionalAct manifests juridische verplichting"</subaction>
<subaction>- "Geldsom = ValueBearer = LegalObject in betalingsverplichting"</subaction>
<subaction>CROSS-VALIDATIE: Secundaire mappings mogen juridische kern NIET conflicteren</subaction>
<template-output>secondary_context_mapping</template-output>
</step>

<step n="4.5" goal="CROSS-VALIDATION tegen Existing Tonto Knowledge Graph - VERPLICHT">
<critical>CRITICAL: Voer cross-validaties uit tegen GELADEN Tonto Knowledge Graph</critical>
<action>SCAN bestaande Tonto Knowledge Graph concepten voor cross-validatie:</action>

Cross-Validation Algoritme:
Voor elk nieuw gevalideerd concept:
- **Direct Match Check**: Exact dezelfde naam/concept reeds aanwezig?
- **Proximity Analysis**: Semantisch vergelijkbare concepten (zelfde domein, gerelateerde betekenis)
- **Extension Opportunities**: Bestaande concepten die aangevuld kunnen worden met nieuwe informatie
- **Conflict Detection**: Concepten die conflicteren met bestaande definities

<action>Voor elke match/proximity detectie:</action>
<subaction>Analyseer: Is dit hetzelfde concept dat uitgebreid kan worden?</subaction>
<subaction>Of: Is dit een nieuw concept dat niet conflicteert?</subaction>
<subaction>Of: Is er een semantisch conflict dat opgelost moet worden?</subaction>

<action>Extension Detection:</action>
<subaction>Bestaande concepten identificeren die GEEN juridische context hebben maar WEL relevant zijn</subaction>
<subaction>Cross-ontology verbanden leggen tussen nieuwe concepten en bestaande</subaction>
<subaction>Gebruiker vragen: "Bestaand concept X kan aangevuld worden met nieuwe juridische context. Uitbreiden? [ja/nee/nieuw-concept]"</subaction>

<action>User Decisions voor Cross-Validation:</action>
<subaction>Voor direct matches: "Bestaand concept gevonden - uitbreiden of nieuw apart concept? [uitbreiden/apart/bewerken]"</subaction>
<subaction>Voor proximity matches: "Gerelateerd concept gevonden - combineren of apart houden? [combineren/apart/analyse]"</subaction>
<subaction>Voor extension kansen: "Concept kan bestaande kennis uitbreiden - toepassen? [ja/nee/selectief]"</subaction>

<critical>LegalAnalyst: Dit is waar je de Knowledge Graph ITERATIEF UITBREIDT - niet alleen toevoegt, maar ook VERBETERT bestaande concepten</critical>
<template-output>cross_validation_results</template-output>
</step>

<step n="5" goal="Legal relation analysis">
<action>Analyze relations using existing LegalOntology relation types</action>
<template-output>relation_analysis</template-output>
</step>

<step n="6" goal="Knowledge Graph Maintenance en Versioning">
<critical>CRITICAL: Zorg voor Knowledge Graph integriteit na elke update</critical>
<action>Voer maintenance checks uit:</action>
<subaction>Alle cross-referenties nog geldig?</subaction>
<subaction>Geen orphaned concepten ontstaan?</subaction>
<subaction>Ontology consistentie behouden?</subaction>
<subaction>Geen circulaire referenties geïntroduceerd?</subaction>
<action>Version control en backup:</action>
<subaction>Creeer backup van vorige Knowledge Graph versie</subaction>
<subaction>Documenteer alle veranderingen (toevoegingen, uitbreidingen, conflicts opgelost)</subaction>
<subaction>Update versie metadata</subaction>
<action>Laatste validatie: Knowledge Graph klaar voor volgende analyse iteratie</action>
<template-output>knowledge_graph_maintenance</template-output>
</step>

<step n="6.5" goal="Cross-Ontology Integration Validation">
<action>Valideer model tegen alle OntologyBasis ontologieën</action>
<action>Controleer cross-ontology consistentie en referenties</action>
<action>Zorg voor juiste Tonto syntax volgens alle guidance bestanden</action>
<template-output>ontology_integration_validation</template-output>
</step>

<step n="7" goal="Tonto Model Validation and Error Correction">
<action>CRITICAL: Implement automatic Tonto validation en error correction</action>
<action>Validate generated Tonto code:</action>
<subaction>CHECK syntax against Tonto grammar and guidance files</subaction>
<subaction>VALIDATE stereotypes juiste ontology principes volgen</subaction>
<subaction>VERIFY cardinalities volgens cardinality guidance</subaction>
<subaction>TEST terminology consistency volgens analysis guide</subaction>
<subaction>CONFIRM documentation standards volgens documentation guide</subaction>
<action>Error correction algorithm:</action>
<subaction>Upon syntax error: Auto-fix met Tonto guidance correcties</subaction>
<subaction>Upon stereotype error: Advise correct stereotype uit guidance</subaction>
<subaction>Upon cardinality error: Fix volgens cardinality rules</subaction>
<subaction>Upon terminology error: Correct volgens terminology guide</subaction>
<subaction>Upon documentation error: Improve volgens documentation standards</subaction>
<action>Generate validation report:</action>
<subaction>Number of errors found and corrected</subaction>
<subaction>Confidence score voor corrected model</subaction>
<subaction>Suggestions voor manual review indien needed</subaction>
<critical>Tonto model MOET 100% compliant zijn voordat naar Knowledge Graph wordt geschreven</critical>
<template-output>tonto_validation_and_correction</template-output>
</step>

<step n="8" goal="Multilingual OWL Instance Graph Integration with ob: prefix">
<action>Voor elke geïdentificeerde entiteit:</action>
<subaction>Genereer unieke URI: ex:article{section}-{number}-{entity}</subaction>
<subaction>Voeg rdf:type relatie naar ob:OntologyBasis.ttl</subaction>
<subaction>Voeg rdfs:label in @en en @nl toe</subaction>
<subaction>Voeg ob:definition in @en en @nl toe</subaction>
<subaction>Voeg rdfs:comment met juridische context toe</subaction>
<subaction>Maak ontologische relaties (:inheresIn, :composedOf, ob:inheresIn)</subaction>
<action>Output naar {owl_knowledge_graph_output} als Turtle format (.ttl)</action>
<action>Gebruik deze namespace prefixen:</action>
<subaction>@prefix ob: <https://example.com#> .</subaction>
<subaction>@prefix ex: <https://example.com/instances#> .</subaction>
<action>Write complete OWL graph to: {project-root}/docs/legal-owl-knowledge-graph.ttl</action>
<action>Append new instances to existing graph (don't overwrite)</action>
<action>Update metadata with analysis timestamp and article reference</action>
<action>Voorbeeld per instantie:</action>
<subaction>ex:article10-1-government-body rdf:type ob:GovernmentBody ;</subaction>
<subaction>    rdfs:label "Government Body"@en , "Bestuursorgaan"@nl ;</subaction>
<subaction>    ob:definition "A governmental body that exercises..."@en , "Een bestuursorgaan dat..."@nl ;</subaction>
<subaction>    rdfs:comment "Instantie uit artikel 10:1 Awb"@nl .</subaction>
<critical>Elke instantie MOET multilingual metadata hebben voor internationale querybaarheid</critical>
<action>Integrate validated Tonto concepts into Knowledge Graph:</action>
<subaction>READ current Knowledge Graph file</subaction>
<subaction>MERGE new concepts met bestaande structuur</subaction>
<subaction>UPDATE cross-references en relaties</subaction>
<subaction>MAINTAIN package integriteit (LegalKnowledgeGraph)</subaction>
<action>Extended legal structure analysis:</action>
<subaction>EXPAND LawOntology mappings: Law → Chapter → Article → Paragraph hiërarchie</subaction>
<subaction>ADD Norm concepts: Permission, Prohibition, Obligation uit ObjectOntology</subaction>
<subaction>MAP legal subjects en objects naar complete juridische structuur</subaction>
<subaction>CONNECT rights/duties naar concrete norm types</subaction>
<action>Update Knowledge Graph metadata:</action>
<subaction>Add analyzed article to accumulated articles list</subaction>
<subaction>Update version information</subaction>
<subaction>Document integration quality metrics</subaction>
<action>Final validation:</action>
<subaction>Knowledge Graph parseert zonder fouten</subaction>
<subaction>All cross-references resolved</subaction>
<subaction>Concept map volledig geïntegreerd</subaction>
<critical>SUCCESS: Article analysis volledig geïntegreerd in Knowledge Graph - klaar voor volgende analyse</critical>
<template-output>knowledge_graph_only_output</template-output>
</step>



</workflow>
