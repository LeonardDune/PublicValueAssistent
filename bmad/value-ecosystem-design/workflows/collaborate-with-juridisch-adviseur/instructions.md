<critical>The workflow execution engine is governed by: {project_root}/bmad/core/tasks/workflow.xml</critical>
<critical>You MUST have already loaded and processed: {installed_path}/workflow.yaml</critical>

<workflow>

<step n="1" goal="Collaboration setup">
<action>Establish collaboration parameters with juridisch adviseur</action>
<ask>Define collaboration scope:
1. Type advies request (juridisch, ethisch, technisch)
2. Public service proposition details
3. Urgentie niveau (hoog, medium, laag)
4. Gewenste expertise gebieden
5. Communicatie voorkeuren</ask>
<template-output>collaboration_setup</template-output>
</step>

<step n="2" goal="Context preparation">
<action>Prepare comprehensive context for legal advisor</action>
<action>Assemble relevant information:
- Public service proposition beschrijving
- Stakeholders en belangen
- Juridische kaders en beperkingen
- Risico analyse en ethische overwegingen</action>
<template-output>advisor_context</template-output>
</step>

<step n="3" goal="Advice request formulation">
<action>Formulate structured advice request</action>
<action>Include specific questions and scenarios:
- Juridische haalbaarheid
- Compliance vereisten
- Risico mitigatie strategieën
- Implementation richtlijnen</action>
<template-output>advice_request</template-output>
</step>

<step n="4" goal="Advisor consultation facilitation">
<action>Facilitate consultation with juridisch adviseur</action>
<ask>Schedule consultation details:
1. Adviseur contact informatie
2. Voorkeurs communicatiemethode
3. Tijdschema en duur
4. Specifieke aandachtspunten</ask>
<critical>Initiate consultation process</critical>
<template-output>consultation_summary</template-output>
</step>

<step n="5" goal="Expert analysis and feedback">
<action>Capture and analyze received advice</action>
<action>Document expert insights:
- Juridische beoordelingen
- Risico identificatie
- Compliance aanbevelingen
- Implementation constraints</action>
<template-output>expert_analysis</template-output>
</step>

<step n="6" goal="Integration synthesis">
<action>Synthesize advice with project context</action>
<action>Correlate expert input with:
- Ontwerp beslissingen
- Implementation strategieën
- Risico management
- Stakeholder communication</action>
<template-output>integration_synthesis</template-output>
</step>

<step n="7" goal="Recommendation development">
<action>Develop actionable recommendations</action>
<action>Formulate specific guidance:
- Juridisch compliant oplossingen
- Risk mitigation measures
- Compliance monitoring
- Documentation requirements</action>
<template-output>recommendations</template-output>
</step>

<step n="8" goal="Knowledge Graph advice integration">
<action>CRITICAL: Always LOAD existing Knowledge Graph from knowledge/legal-analysis-graph.ttl FIRST</action>
<action>Integrate juridisch advies as gUFO-compliant triples</action>
<action>Create advice instances linked to propositions:
- rdf:type :LegalAdvice
- gufo:typeOf gufo:Situation
- Links naar betreffende legal concepts en propositions
- Compliance recommendations als triples</action>
<action>DOCUMENT every advice addition with:
- Precise definition specifying the ontological type (e.g., "X is a LegalRelator that...", "Y is a Right that...")
- 3 examples (instances that comply)
- 3 counter-examples (edge cases that fall outside definition)</action>
<action>SAVE updated graph back to knowledge/legal-analysis-graph.ttl with nieuwe adviesdata</action>
<template-output>knowledge_graph_integration</template-output>
</step>

</workflow>
