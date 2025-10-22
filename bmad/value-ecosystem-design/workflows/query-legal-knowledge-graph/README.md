# Query Legal Knowledge Graph Workflow

## Doel

Deze workflow stelt gebruikers in staat om diepgaande queries uit te voeren op de LegalOntology-gebaseerde knowledge graph voor het ontdekken van complexe juridische relaties, patronen en inzichten.

## Gebruik

Activeer deze workflow door in de LegalAnalyst agent te typen: `*query-knowledge-graph`

## Invoer

De workflow vraagt om query specificaties:
1. **Query type** - SPARQL, concept search, relatie exploratie, patroon matching
2. **Focus gebied** - Rechten, verplichtingen, procedures, actoren, alles
3. **Query scope** - Enkel concept, relatie chains, subgraph, volledige graph
4. **Output format** - Tekst samenvatting, graph visualisatie, data export

## Uitvoer

Genereert uitgebreide query resultaten met:
- Directe en inferred relatie resultaten
- Ontologische betekenis analyse
- Knowledge graph enrichment suggesties
- Visualisaties van gevonden patronen
- Uitvoerbare aanbevelingen voor verdere exploratie

## Query Types

### SPARQL Queries
- **Complex queries** voor specifieke relatie patronen
- **Path finding** voor multi-hop connecties
- **Aggregation queries** voor statistische inzichten
- **Validation queries** voor data kwaliteit checks

### Concept Searches
- **Semantische zoekopdrachten** in ontologische hiërarchieën
- **Similarity matching** voor equivalente concepten
- **Context-aware retrieval** voor relevante relaties
- **Cross-domain linking** voor interdisciplinaire connecties

### Relation Exploration
- **Chain discovery** voor afhankelijkheid paden
- **Network analysis** voor stakeholder connecties
- **Pattern mining** voor structurele regelmatigheden
- **Constraint validation** voor ontologische consistentie

## Toepassingen

### Juridische Research
- Complexe relatie patronen ontdekken
- Ontbrekende connecties identificeren
- Compliance paden doorzoeken
- Risico afhankelijkheden analyseren

### Ontologische Ontwikkeling
- Knowledge graph kwaliteit valideren
- Nieuwe relatie patronen ontdekken
- Ontologische assumptions testen
- Enhancement opportunities identificeren

### Stakeholder Analyse
- Interconnecties tussen actoren mappen
- Beïnvloedingsnetwerken analyseren
- Juridische afhankelijkheden visualiseren
- Governance structuren doorzoeken

## Technische Specificaties

### Graph Processing
- LegalOntology als ontologische backbone
- SPARQL query execution voor complexe searches
- Graph traversal voor relatie chains
- Confidence scoring voor inferred results

### Output Formaten
- **JSON export** voor systeem integratie
- **GraphML export** voor visualisatie tools
- **CSV export** voor spreadsheet analyse
- **TTL/RDF export** voor semantic web toepassingen

## Kwaliteitsborging

De workflow verzekert:
- **Query accurateit** door ontologische grounding
- **Resultaat compleetheid** via comprehensieve traversal
- **Interpretatie juistheid** met expert context
- **Performance optimization** voor grote graph queries

## Vereisten

- LegalOntology beschikbaar voor ontologische fundament
- Knowledge graph data beschikbaar (gegenereerd door andere workflows)
- BMAD core workflow engine met query ondersteuning
- Query expertise voor complexe vraagstellingen

## Implementatie Protocol

Na query uitvoering:
1. Review query resultaten voor ontologische correctheid
2. Integreer inzichten in juridische besluitvorming
3. Implementeer geadviseerde graph enhancements
4. Gebruik bevindingen voor LegalOntology verbetering
