# Product Requirements Document (PRD)
## AI Public Value Ecosystem Design Agent

---

### 1. Product Overview

The **AI Public Value Ecosystem Design Agent (PVE Agent)** supports policymakers, designers, and enterprise architects in **value-driven design of public service ecosystems**.

The system enables modeling, reasoning, and evaluation of ecosystems in terms of:

- **Public values** (e.g., justice, safety, trust);
- **Value propositions** at multiple levels (ecosystem, organization, role);
- **Transactions** that express value creation or exchange between actors;
- **Value objects** that embody what is valued or exchanged.

The agent is both **knowledge-based** (driven by an ontology and vectorstore) and **AI-supported** (generative reasoning through LLM and semantic querying).

---

### 2. Problem Statement

Public service delivery chains consist of multiple autonomous organizations with partially overlapping mandates.  
There is no shared conceptual language to:

- Describe the **public value proposition** of the whole ecosystem;
- Understand the **contributions of individual actors** to that proposition;
- Analyze **inter-actor dependencies and transactions** in value terms;
- Identify and explain **loss of public value** at points of failure or fragmentation.

This leads to siloed optimization, fragmented accountability, and diminished societal impact.

---

### 3. Product Goals

The PVE Agent should enable users to:

1. **Model ecosystems** in terms of actors, roles, values, services, and transactions.  
2. **Formulate value propositions**:
   - For the ecosystem as a whole;
   - For individual actors/roles;
   - For specific services.
3. **Identify and describe transactions**:
   - Who delivers what to whom?
   - What is exchanged (value object)?
   - What public values are affected?
4. **Analyze value creation and loss**:
   - Which values are strengthened or weakened?
   - How does each actor contribute to public value?
5. **Support design and governance decisions** driven by public values.

---

### 4. Core Concepts (Ontology Overview)

| Concept | Definition | Key Relationships |
|----------|-------------|-------------------|
| **Public Value Ecosystem (PVE)** | A coherent system of actors, roles, services, and transactions that collectively create public value. | Has one or more *Public Value Propositions*; consists of *Actors*, *Roles*, *Services*, and *Transactions*. |
| **Public Value Proposition** | The promise of value creation for society by the ecosystem (or a role within it). | Targets one or more *Public Values* and focuses on one or more *Value Objects*. |
| **Public Value** | A normatively desired societal condition (e.g., justice, safety, trust). | Is realized or threatened through *Transactions* and *Services*. |
| **Value Object** | That which carries or embodies value (e.g., safety, information integrity, legal certainty, care). | Is the focus of a *Service* or *Transaction*. |
| **Actor** | An organization or individual participating in the ecosystem. | Fulfills one or more *Roles*; participates in *Transactions*. |
| **Role** | The functional position of an actor in the ecosystem (e.g., prosecutor, victim, police officer). | Can deliver or consume *Services*; participates in *Transactions*. |
| **Transaction** | An exchange between roles involving the delivery or receipt of a *Value Object*. | Connects *Supplier Role* and *Consumer Role*; contributes to *Public Value*. |
| **Service** | An organized, repeatable pattern of transactions that delivers value to others. | Delivered by *Supplier Role*, consumed by *Consumer Role*, focused on a *Value Object*. |

---

### 5. Relationship Diagram (Semantic Structure)

PublicValueEcosystem
├── hasValueProposition → PublicValueProposition
│ ├── targets → PublicValue
│ └── focusesOn → ValueObject
├── hasActor → Actor
│ └── fulfills → Role
├── includesService → Service
│ ├── delivers → ValueObject
│ ├── providedBy → Role (Supplier)
│ └── consumedBy → Role (Consumer)
└── includesTransaction → Transaction
├── hasSupplier → Role
├── hasConsumer → Role
├── exchanges → ValueObject
└── contributesTo → PublicValue

---

### 6. Functional Requirements

| ID | Requirement | Description |
|----|--------------|-------------|
| F1 | Ecosystem Definition | User can create and save an ecosystem model with actors, roles, values, and services. |
| F2 | Ontology Navigation | User can browse the semantic structure and visualize entity relationships. |
| F3 | Value Mapping | The agent assists in linking transactions and services to public values. |
| F4 | Value Proposition Editor | The agent supports the formulation of public value propositions at ecosystem and actor level. |
| F5 | Transaction Reasoning | The agent can reason about the consistency of transactions (supplier, consumer, value). |
| F6 | Value Conflict Detection | The agent detects conflicts between public values or actor interests. |
| F7 | Scenario Simulation | The agent can simulate how changes in services or transactions affect public values. |
| F8 | Export Ontology | The user can export the ontology in JSON-LD or Tonto format. |

---

### 7. Example Use Case: Victim Support in the Criminal Justice Chain

**Ecosystem:** Criminal Justice System  
**Public Value Proposition:** Justice and recovery for victims  
**Public Values:** Justice, safety, trust  
**Actors:** Police, Victim Support, Public Prosecution, Judiciary  
**Roles:**  
- *Police* → Incident Handler (supplier)  
- *Victim Support* → Care Provider (supplier)  
- *Victim* → Recipient of Care (consumer)

**Service:** Victim Information Provision  
**Value Object:** “Information about criminal proceedings”  
**Transaction:** Police → Victim (information exchange)  
**Contribution to Public Value:** Strengthens *trust* and *justice*.

---

### 8. Non-Functional Requirements

| ID | Requirement | Description |
|----|--------------|-------------|
| N1 | Explainability | All reasoning steps and conclusions must be traceable to underlying knowledge sources. |
| N2 | Interoperability | Ontology must be exportable in RDF/OWL, JSON-LD, and Tonto formats. |
| N3 | Extensibility | Ontology must support domain-specific extensions. |
| N4 | Usability | Conversational interface with natural language prompts. |
| N5 | Traceability | All model changes must be version-controlled and auditable. |

---

### 9. Future Extensions

- Integration with legal ontologies (e.g., Hohfeld schema, Wetsanalyse).  
- Linking with DEMO transaction theory for coordination act modeling.  
- Automated public value impact assessment using real-world data.

---

### 10. Deliverables

- `public_value_ontology.jsonld`  
- `public_value_ontology.tonto`  
- Conversational UI prototype  
- Reasoning engine (Python + vectorstore)  
- Knowledge import/export module

---

*Last updated: October 2025*
