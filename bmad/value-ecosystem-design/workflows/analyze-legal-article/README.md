# Analyze Legal Article Workflow

## Doel

Deze workflow voert een volledige ontologische analyse uit van juridische artikelen met concept mapping naar de LegalOntology en uitbreiding van de knowledge graph.

## Gebruik

Activeer deze workflow door in de LegalAnalyst agent te typen: `*analyze-article`

## Invoer

De workflow vraagt om:
1. **Volledige artikeltekst** - Kopieer de juridische tekst
2. **Jurisdictie** - Nederlands recht, EU recht, internationaal recht
3. **Artikel referentie** - Bijv. Artikel 12, §34
4. **Context** - Wet naam, doel, domein

## Uitvoer

Genereert een uitgebreid rapport met:
- Artikel overzicht met ontologische kader
- Complete concept mapping tabel
- Relatie analyse met UFO stereotypen
- Knowledge graph uitbreidingsaanbevelingen
- Implementatie suggesties voor LegalOntology updates

## Bestanden

- `workflow.yaml` - Workflow configuratie
- `instructions.md` - Uitvoeringsstappen
- `template.md` - Rapport structuur
- `checklist.md` - Validatie criteria

## Ontologische Fundering

Deze workflow baseert zich op:
- **UFO (Unified Foundational Ontology)** principes
- **LegalOntology** als conceptuele basis
- **Tonto** taal voor ontologische modellering

## Vereisten

- Toegang tot LegalOntology (OntologyBasis/LegalOntology.tonto)
- BMAD core workflow engine
- LegalAnalyst agent configuratie

## Implementatie Suggesties

Na gebruik van deze workflow:
1. Review het rapport voor ontologische accuraatheid
2. Implementeer geadviseerde LegalOntology uitbreidingen
3. Update knowledge graph met nieuwe concepten
4. Herhaal analyse voor gerelateerde artikelen
