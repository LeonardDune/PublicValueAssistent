# Compare Legal Articles Workflow

## Doel

Deze workflow vergelijkt juridische artikelen op overlappingen, conflicten en onderlinge relaties met behulp van het LegalOntology framework. Het identificeert systematisch juridische connecties tussen verschillende wetsteksten.

## Gebruik

Activeer deze workflow door in de LegalAnalyst agent te typen: `*compare-articles`

## Invoer

De workflow vraagt om:
1. **Aantal artikelen** - Minimum 2 voor vergelijking
2. **Artikel teksten** - Volledige juridische teksten of referenties
3. **Jurisdictie context** - Gedeelde rechtsgebied voor artikelen
4. **Vergelijking focus** - Overlaps, conflicten, relaties, of alles

## Uitvoer

Genereert een uitgebreid vergelijkingsrapport met:
- Individuele artikel analyses
- Overlap matrices en conflict detectie
- Inter-artikel relatie diagrammen
- LegalOntology uitbreiding aanbevelingen
- Implementatiesuggesties voor juridische harmonisatie

## Analyse Componenten

### Individuele Analyse
- Concept mapping naar LegalOntology per artikel
- Relatie analyse met UFO stereotypen
- Unique elementen catalogus

### Vergelijkende Analyse
- **Overlappingen identificatie**: Gedeelde concepten en equivalenties
- **Conflict detectie**: Contradicties en incompatibiliteiten
- **Relatie analyse**: Cross-artikel afhankelijkheden en connecties

### Ontologische Uitbreiding
- Nieuwe relaties tussen bestaande klassen
- Ontbrekende intermediaire concepten
- Framework verbeteringen gebaseerd op bevindingen

## Bestanden

- `workflow.yaml` - Workflow configuratie met LegalOntology integratie
- `instructions.md` - 8-staps vergelijkingsmethodologie
- `template.md` - Rapport structuur voor uitvoer
- `checklist.md` - Validatie criteria voor vergelijkingskwaliteit

## Ontologische Methodologie

Deze workflow gebruikt:
- **Systeem vergelijking** van ontologische mappings
- **Conflict analyse** gebaseerd op UFO constraints
- **Relatie synthese** tussen verschillende juridische contexten
- **Knowledge graph integratie** voor bredere inzichten

## Toepassingsgebieden

- Wetgevingsharmonisatie tussen jurisdicties
- Conflictoplossing in juridische kaders
- Duidelijkheid verbetering in complexe reglementen
- Ontwikkeling van geïntegreerde juridische systemen

## Vereisten

- Toegang tot LegalOntology voor framework mapping
- BMAD core workflow engine
- Minimaal 2 juridische artikelen voor vergelijking

## Vervolgacties

Na workflow uitvoering:
1. Review vergelijkingsrapport voor juridische implicaties
2. Implementeer ontologische verbeteringen
3. Gebruik bevindingen voor wetgevingsverbetering
4. Herhaal analyse bij nieuwe juridische ontwikkelingen
