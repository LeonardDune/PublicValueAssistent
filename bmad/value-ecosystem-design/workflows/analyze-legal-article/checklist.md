# Validatie Checklist: Tonto-Gebaseerde Artikel Analyse

## Structuur en Compleetheid

- [ ] Alle analyse secties zijn aanwezig (1-10)
- [ ] Artikel details volledig vastgelegd (tekst, jurisdictie, referentie)
- [ ] ALLE 13 OntologyBasis ontologieën geladen als complete context
- [ ] Tonto guidance bestanden geladen en geïntegreerd (7 guidance files)

## Tonto Expertise Integration

- [ ] Stap 1.5 uitgevoerd: Alle Tonto guidance bestanden bestudeerd
- [ ] LegalAnalyst heeft volledige Tonto expertise voorgelegd
- [ ] Correct Tonto syntax gebruikt in alle outputs
- [ ] Proper stereotyping volgens Tonto guidance (kind, role, relator, etc.)

## Ontologische Integriteit

- [ ] Concepten gemapped naar BESTAANDE concepten in ALLE OntologyBasis ontologieën
- [ ] Cross-ontology context geïntegreerd (Agent, Event, Mode, Object, Legal, Value)
- [ ] UFO-concepten gebruikt via OntologyBasis ontologieën (geen directe gUFO)
- [ ] Geen nieuwe concepten toegevoegd - alleen bestaande uitgebreid

## Tonto Model Instantiation

- [ ] Tonto model gegenereerd met correcte syntax
- [ ] Proper cardinalities volgens cardinality guidance
- [ ] Labels en descriptions in @en en @nl volgens documentation guide
- [ ] Relaties met correcte connectors (-- voor association, <>-- voor aggregation)

## Cross-Ontology Integration

- [ ] Model gevalideerd tegen alle 13 OntologyBasis ontologieën
- [ ] Cross-ontology consistentie en referenties gecontroleerd
- [ ] Geen conflicten tussen ontologieën geïdentificeerd
- [ ] Geïntegreerde ontologische context behouden

## Tonto Compliance Validatie

- [ ] Tonto syntax volledig compliant
- [ ] Stereotyping correct volgens Tonto guidance
- [ ] Cardinalities gevalideerd volgens cardinality guidance
- [ ] Terminology gecontroleerd volgens terminology analysis guide
- [ ] Documentatie volledig volgens documentation guide

## Knowledge Graph Maintenance

- [ ] Bestaande Tonto Knowledge Graph geladen bij workflow start (stap 2.1)
- [ ] Cross-validaties uitgevoerd tegen alle bestaande concepten (stap 4.5)
- [ ] Concepten aangevuld waar nieuwe analyse relevantie toevoegt
- [ ] Knowledge Graph incrementeel uitgebreid (niet vervangen)
- [ ] Geen conflicten geïntroduceerd tussen nieuwe en bestaande concepten
- [ ] Cross-referenties behouden en bijgewerkt waar nodig
- [ ] Knowledge Graph maintenance checks uitgevoerd (stap 6.6)
- [ ] Backup gemaakt van vorige versie
- [ ] Versie metadata bijgewerkt

## Primaire Concept Mapping - Juridische Kern

- [ ] Stap 4: Primaire mapping naar juridische kern ontologieën uitgevoerd
- [ ] Alle artikel concepten eerst gemapped naar LegalOntology.tonto (rechtsbetrekkingen, rechtssubjecten, rechtsobjecten)
- [ ] Artikel tekst gemapped naar Article (LawOntology.tonto) bevattende Norm (ObjectOntology.tonto)
- [ ] Rechtssubjecten geïdentificeerd als LegalSubject/Claimant/Committor (LegalOntology.tonto)
- [ ] Rechtsbetrekkingen gemapped naar LegalRelator/RightDutyRelator (LegalOntology.tonto)
- [ ] Rechten/Plichten correct toegepast als Right/Duty uit LegalOntology.tonto
- [ ] InstitutionalAct gebruikt voor institutionele acties waar relevant

## Secundaire Context Mapping - Cross-Ontology

- [ ] Stap 4A: Secundaire context mapping naar aanvullende ontologieën uitgevoerd
- [ ] AgentOntology cross-links: NaturalPerson/Claimant, LegalPerson/Committor, GovernmentBody/LegalSubject
- [ ] EventOntology cross-links: InstitutionalAct manifestations, CommunicativeAct juridische contexten
- [ ] ModeOntology cross-links: SocialCommitment juridische basis, SocialClaim rechten
- [ ] ValueOntology cross-links: ValueBearer als LegalObject, ValueAscription waardebepalingen
- [ ] ALLE relevante cross-ontology verbanden geïdentificeerd en gelegd
- [ ] Cross-ontology patronen toegepast (bijv. burger→NaturalPerson→Claimant, bedrijf→PrivateLegalPerson→Committor)

## Cross-Ontology Integration

- [ ] Secundaire mappings conflicteren NIET met primaire juridische kern
- [ ] Alle cross-ontology relaties ontologisch consistent
- [ ] Voorbeeld patronen correct toegepast (burger/onderwijs-recht, bedrijf/belastingplicht, geldsom/betalingsverplichting)
- [ ] Alle OntologyBasis perspectieven geïntegreerd (Agent, Event, Mode, Object, Legal, Value)
- [ ] Geen relevante cross-ontology kansen overgeslagen

## Tonto Knowledge Graph Output

- [ ] Knowledge Graph opgeslagen naar {project-root}/docs/legal-knowledge-graph.tonto
- [ ] Geïntegreerde model klaar voor Tonto tooling (syntax highlighting, validation, etc.)
- [ ] Incrementeel uitgebreid op bestaande juridische kennisbasis
- [ ] Model review mogelijk voor gebruiker
- [ ] Klaar voor volgende analyse iteratie als input

## Rapport en Output Kwaliteit

- [ ] Rapport documenteert Tonto model toevoegingen
- [ ] Tonto compliance status gerapporteerd
- [ ] Cross-article relatie kansen geïdentificeerd
- [ ] Rapport klaar voor juridisch en ontologisch gebruik

---

## Compliance Check

**Ontologische Compliance:** ☐ Strikt OntologyBasis ☐ Goed ☐ Verbetering Nodig ☐ Herschrijven

**Tonto Compliance:** ☐ Volledig Compliant ☐ Deels Compliant ☐ Niet Compliant ☐ Herschrijven

**Cross-Ontology Integration:** ☐ Perfect ☐ Goed ☐ Verbetering Nodig ☐ Conflicten Oplosbaar ☐ Herschrijven

**Tonto Model Output:** ☐ Succesvol ☐ Mislukt ☐ Handmatig Nagekeken ☐ Status Onbekend

**LegalAnalyst Tonto Expertise:** ☐ Volledig Geverifieerd ☐ Deels Geverifieerd ☐ Niet Voldoende ☐ Herscholing Nodig
