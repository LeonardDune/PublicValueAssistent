# Lex Onto Knowledge Base

## Legal Analysis Knowledge Graph

**Bestand**: `legal-analysis-graph.ttl`
**Formaat**: gUFO-compliant Turtle (TTL)
**Ontology**: Based on `OntologyBasis/LegalOntology.tonto` + `OntologyBasis.ttl`

### Huidige Content

#### Artikelen Geanalyseerd (20 oktober 2025)
- **Artikel 10:1 Awb**: Mandaat definitie - Machtsafstand concepten
- **Artikel 10:2 Awb**: Mandaat grenzen - Disability-Immunity patterns

#### UFO-L Concept Coverage
- **Legal Positions**: Power, Subjection, Disability, Immunity
- **Legal Relators**: PowerSubjectionRelator, DisabilityImmunityRelator
- **Institutional Elements**: InstitutionalAct (besluitvorming)
- **Normative Elements**: NormativeDescription (wetteksten)
- **Conditional Logic**: LegalCondition, DerivationRule

#### Graph Metrics
- Totaal triples: ~85
- Instances: 18 (alle UFO-L compliant)
- Cross-artikel relaties: 3
- Compliance level: 100% gUFO/UFO-L

### Usage Instructions

#### Nieuwe Analyse Starten
1. **Load** bestaande graph: `legal-analysis-graph.ttl`
2. **Extend** met nieuwe concepten en relaties
3. **Validate** tegen LegalOntology.ttl
4. **Save** terug naar dit bestand

#### Queries Uitvoeren
Graph is SPARQL-ready voor complexe queries:
- Cross-artikel verbanden vinden
- Disability patterns analyseren
- Legal position inheritance traceren

### Maintenance Notes

- **Incremental Building**: Elke analyse breidt de graph uit
- **Version Control**: TTL format is Git-compatible
- **Backup**: Automated updates bij elke analyse
- **Future Extensions**: Gereed voor meer Awb artikelen, Europese wetgeving, verdragen

### Integration Points

- **BMAD Workflow**: Gebruikt in value ecosystem design pipelines
- **JuridischAdviseur**: Voorziet gestructureerde juridische kennis
- **Other VED Agents**: Levert ontologische foundation voor stakeholder analyses

---

**Last Updated**: 20 oktober 2025
**Articles Count**: 2
**Compliance**: 100% UFO-L Strict
