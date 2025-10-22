<critical>The workflow execution engine is governed by: {project_root}/bmad/core/tasks/workflow.xml</critical>
<critical>You MUST have already loaded and processed: {installed_path}/workflow.yaml</critical>

<workflow>

<step n="1" goal="Example generation setup">
<action>Collect parameters for example generation</action>
<ask>Specify example generation parameters:
1. Legal concepts to generate examples for (names or from LegalOntology)
2. Target audience (juristen, burgers, experts, studenten)
3. Complexity level (basic, intermediate, advanced)
4. Number of examples per concept (1-5)
5. Context domain (privacy, contracten, administratief recht, etc.)</ask>
<critical>Validate input parameters</critical>
<template-output>example_generation_setup</template-output>
</step>

<step n="2" goal="LegalOntology concept selection">
<action>Load relevant concepts from LegalOntology</action>
<action>Filter concepts based on user parameters:
- Rights (LegalRight instances)
- Obligations (LegalObligation classes)
- Procedures (LegalProcedure relations)
- Actors and stakeholders</action>
<action>Categorize concepts by type and complexity</action>
<template-output>selected_concepts</template-output>
</step>

<step n="3" goal="Concept familiarization">
<action>Deep understanding of selected legal concepts</action>
<action>For each concept analyze:
- Ontological definition and characteristics
- UFO stereotypes and relations
- Practical implications
- Real-world occurrences</action>
<template-output>concept_familiarization</template-output>
</step>

<step n="4" goal="Example categorization framework">
<action>Create framework for example types</action>
<action>Define example categories:
- Simple hypothetical scenarios
- Real-world case adaptations (anonymized)
- Progressive complexity levels
- Cross-domain applications</action>
<template-output>example_framework</template-output>
</step>

<step n="5" goal="Individual concept examples">
<action>Generate examples for each selected concept</action>
<for-each concept="selected_legal_concepts">
<action>Create 1-5 examples per concept based on parameters</action>
<action>Ensure examples are:
- Realistic and grounded in legal practice
- Appropriate for target audience complexity
- Clear demonstrations of the legal concept
- Include stakeholder perspectives</action>
</for-each>
<elicit-required/>
<template-output>concept_examples</template-output>
</step>

<step n="6" goal="Example validation and refinement">
<action>Validate generated examples for accuracy and clarity</action>
<action>Check each example:
- Legal-concept correspondence (maps correctly to ontology)
- Practical applicability (useful in real situations)
- Clarity and comprehension (target audience appropriate)
- Ethical considerations (proper anonymization, no misleading)</action>
<template-output>example_validation</template-output>
</step>

<step n="7" goal="Educational enhancement">
<action>Add educational value to examples</action>
<action>For each example include:
- Concept explanation in simple terms
- Legal implications and consequences
- Related concepts cross-references
- Practical advice or considerations</action>
<template-output>educational_enhancements</template-output>
</step>

<step n="8" goal="Knowledge Graph integration">
<action>CRITICAL: Always LOAD existing Knowledge Graph from knowledge/legal-analysis-graph.ttl FIRST</action>
<action>Add generated examples as gUFO-compliant Turtle triples</action>
<action>Create example instances linked to LegalOntology concepts:
- rdf:type :LegalExample
- gufo:typeOf gufo:Situation
- Links to relevant LegalOntology concepts
- Educational metadata triples</action>
<action>DOCUMENT every example addition with:
- Precise definition specifying the ontological type (e.g., "X is a LegalRelator that...", "Y is a Right that...")
- 3 examples (instances that comply)
- 3 counter-examples (edge cases that fall outside definition)</action>
<action>SAVE updated graph back to knowledge/legal-analysis-graph.ttl with new examples</action>
<template-output>knowledge_graph_integration</template-output>
</step>

</workflow>
