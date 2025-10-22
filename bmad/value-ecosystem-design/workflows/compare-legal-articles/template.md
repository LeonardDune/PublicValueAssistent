# Vergelijkende Analyse van Wetsartikelen

**Datum:** {{date}}
**Gebruiker:** {{user_name}}
**Workflow:** compare-legal-articles

---

## 1. Vergelijking Opzet

{{comparison_setup}}

---

## 2. LegalOntology Vergelijking Kader

{{ontology_framework}}

---

## 3. Individuele Artikel Analyses

{{individual_analyses}}

---

## 4. Concept Overlappingen

{{concept_overlaps}}

---

## 5. Conflicten en Inconsistenties

{{conflicts_analysis}}

---

## 6. Knowledge Graph Instantiëring

**CRITICAL: Always LOAD existing Knowledge Graph from knowledge/legal-analysis-graph.ttl FIRST**
**Nieuwe cross-artikel instanties toegevoegd in gUFO format**
**SAVE updated graph back to knowledge/legal-analysis-graph.ttl after vergelijkingsanalyse**

{{graph_instantiation}}

---

## 7. gUFO Compliance Validatie

**Validatie tegen https://nemo-ufes.github.io/gufo/gufo.ttl**
**Alle triples gebruiken OntologyBasis.ttl concept referenties**

{{compliance_validation}}

---

## 8. Knowledge Graph Update Rapport

{{comparison_report}}

---

*Deze vergelijkende analyse gebruikt LegalOntology als vaste lens voor inter-artikel relatie discovery en Knowledge Graph populatie in strikte gUFO compliance.*
