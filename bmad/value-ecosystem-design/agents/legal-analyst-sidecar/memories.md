# Lex Onto's Memory Bank

## User Preferences
- Communication language: Nederlands
- Analysis depth: Detailed with practical examples for non-experts
- Legal focus: Public service propositions and value ecosystem design
- Framework: Always use LegalOntology.tonto as foundation

## Session History
<!-- Important moments from our interactions -->
- Created: 20 oktober 2025 - Initial agent definition with LegalOntology integration
- Focus: Building ontologie-based knowledge graph for legal analysis
- Lesson Learned: Strict UFO-L compliance - user corrected invented concepts to official ontology only
- Lesson Learned: gUFO format requirement - explicit rdf:type and gufo:typeOf relations for all instances
- Updated Memory & Instructions: Incorporated ontological compliance protocol for future analyses

## Personal Notes
<!-- My observations and insights about legal analysis patterns -->
- LegalOntology provides rich framework for rights/duties/powers analysis
- Integration with JuridischAdviseur essential for policy recommendations
- Need to maintain clear examples for stakeholders without legal background

## Learned Lessons - Ontological Compliance

### Strict UFO-L Compliance
- ALWAYS use only concepts defined in OntologyBasis/LegalOntology.tonto
- NO invented relations or concepts - stick to existing UFO-L framework
- Validate every analysis against official LegalOntology types
- Different types: Power/Subjection/Disability/Immunity (modes), LegalRelator (relations), InstitutionalAct (events)

### gUFO Knowledge Graph Format
- Use OntologyBasis.ttl as reference for all gUFO compliant output
- Every instance MUST have: rdf:type (specific) + gufo:typeOf (general UFO category)
- Explicit type relations: :instance rdf:type :Type ; gufo:typeOf :Type
- Relations like gufo:inheresIn, :composedOf, :defines from LegalOntology properties
