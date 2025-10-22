# Maintain Legal Glossary Workflow

## Doel

Deze workflow onderhoudt en update systematisch een juridische termen woordenlijst gebaseerd op de LegalOntology. Het zorgt voor continue synchronisatie tussen ontologische ontwikkelingen en praktische terminologie documentatie.

## Gebruik

Activeer deze workflow door in de LegalAnalyst agent te typen: `*update-glossary`

## Invoer

De workflow vraagt om onderhoudsparameters:
1. **Update frequentie** - Dagelijks, wekelijks, maandelijks, on-demand
2. **Onderhoudstype** - Volledige update, incrementeel, specifiek domein
3. **Bron wetgevingsdomeinen** - Civiel recht, strafrecht, etc.
4. **Doelgroep** - Algemeen publiek, professionals, academici
5. **Output format** - Alfabetisch, categorisch, ontologisch

## Uitvoer

Genereert een bijgewerkte juridische woordenlijst met:
- Geïndexeerde termen uit LegalOntology
- Ontologisch gefundeerde definities
- Categorisatie en cross-referenties
- Kwaliteitsborging en versiebeheer
- Onderhoudsrichtlijnen

## Onderhoudsstrategieën

### Update Types
- **Volledig**: Complete herbouw gebaseerd op nieuwste LegalOntology
- **Incrementeel**: Alleen nieuw toegevoegde/bijgewerkte termen
- **Targeted**: Specifiek domein of categorie focus

### Term Categorieën
- **Concept termen**: Rechten, verplichtingen, procedures
- **Relatie termen**: Mediation, characterization, componentOf
- **Actor termen**: Partijen, autoriteiten, vertegenwoordigers
- **Eigenschap termen**: Attributen en constraints

## Bestanden

- `workflow.yaml` - Configuratie met onderhoudsstrategieën
- `instructions.md` - 8-staps woordenlijst onderhoud proces
- `template.md` - Woordenlijst structuur en categorieën
- `checklist.md` - Ontologische en juridische validatie criteria

## Methodologie

Deze workflow gebruikt:
- **Systematische extractie** van alle LegalOntology termen
- **Ontologische categorization** gebaseerd op UFO principes
- **Audience-adaptive definitions** voor verschillende gebruikers
- **Kwaliteits assurance** met checklist validatie
- **Version management** voor traceability

## Toepassingsgebieden

### Juridische Praktijk
- Uniforme terminologie in documenten
- Conceptuele helderheid bij juridische analyse
- Basis voor geautomatiseerde juridische systemen

### Onderwijs en Training
- Gestandaardiseerde juridische onderwijs
- Conceptuele fundering voor rechtenstudie
- Praktijkvoorbeelden met ontologische diepgang

### Systeemontwikkeling
- Basis voor juridische ontologies in AI systemen
- Concept mapping voor juridische databases
- Validatie framework voor juridische modellen

## Technische Specificaties

### Input Integratie
- Automatische LegalOntology parsing
- Incrementiele updates detectie
- Bestaande woordenlijst compatibiliteit

### Output Formaten
- Markdown voor web publicatie
- JSON voor systeem integratie
- PDF voor professionele distributie

## Kwaliteitsborging

De workflow waarborgt:
- **Ontologische accuraatheid** door directe LegalOntology synchronisatie
- **Juridische correctheid** met professionele review aanbevelingen
- **Gebruikerstoegankelijkheid** door audience-adaptive taalgebruik
- **Maintainability** door systematische update procedures

## Vereisten

- Toegang tot LegalOntology voor term extractie
- BMAD core workflow engine met for-each ondersteuning
- Optioneel: Bestaande woordenlijst voor incrementeel onderhoud

## Implementatie Protocol

Na workflow uitvoering:
1. Review definities voor juridische accuraatheid door experts
2. Implementeer woordenlijst in doeltoepassingen
3. Stel automatische updates in volgens gekozen frequentie
4. Monitor gebruik en verzamel feedback voor verbeteringen
