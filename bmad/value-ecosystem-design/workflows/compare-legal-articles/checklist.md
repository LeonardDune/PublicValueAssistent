# Validatie Checklist: Vergelijkende Artikel Analyse

## Structuur en Compleetheid

- [ ] Minimaal 2 artikelen succesvol ingeladen en geanalyseerd
- [ ] Vergelijking focus correct bepaald (overlaps/conflicts/relations)
- [ ] Alle analyse secties aanwezig (1-8)
- [ ] LegalOntology correct als kader gebruikt

## Ontologische Kwaliteit van Individuele Analyses

- [ ] Elk artikel correct gemapped naar LegalOntology concepten
- [ ] Relatie stereotypen correct toegepast per artikel
- [ ] Unique elementen per artikel correct gecatalogiseerd
- [ ] Ontologische principes consistent toegepast

## Vergelijkingsanalyse

- [ ] Concept overlappingen accuraat geïdentificeerd en geclassificeerd
- [ ] Overlap typen correct bepaald (exact/taxonomisch/part-whole)
- [ ] Equivalent concepten met verschillende terminologie herkend
- [ ] Gedeelde LegalOntology instantiations correct gemapped

## Conflict Detectie

- [ ] Contradictorische verplichtingen/rechten geïdentificeerd
- [ ] Wederzijds uitsluiten procedures gevonden
- [ ] Ontologische constraint schendingen gedetecteerd
- [ ] Directe en indirecte conflicten onderscheiden

## Knowledge Graph Instantiation

- [ ] CRITICAL: Bestaande legal-analysis-graph.ttl succesvol GELADEN
- [ ] Nieuwe cross-artikel instanties toegevoegd in gUFO format
- [ ] SAVE uitgevoerd naar knowledge/legal-analysis-graph.ttl
- [ ] Incrementele uitbreiding op bestaande graph

## gUFO Compliance

- [ ] Alle triples voldoen aan gUFO specificatie (https://nemo-ufes.github.io/gufo/gufo.ttl)
- [ ] rdf:type verwijzingen naar specifieke concepten (bijv. :LegalRelator)
- [ ] gufo:typeOf verwijzingen naar UFO categorieën (bijv. gufo:Role)
- [ ] Prefixes correct (gufo:, :, rdf:, rdfs:)

## Inter-Artikel Knowledge Graph

- [ ] Cross-artikel relaties geïntroduceerd als gUFO triples
- [ ] Gedeelde concepten gelinkt tussen artikelen
- [ ] Conflicten geformaliseerd in Knowledge Graph
- [ ] Inter-artikel afhankelijkheden gemodelleerd

## Rapport Kwaliteit

- [ ] Vergelijking duidelijk en systematisch gepresenteerd
- [ ] Overlap/conflict matrices overzichtelijk
- [ ] Inter-artikel relatie diagrammen begrijpelijk
- [ ] Aanbevelingen concreet en actiegericht
- [ ] Terminologie consistent door rapport heen

## Technische Accuraatheid

- [ ] Template variabelen volledig vervangen (geen placeholders)
- [ ] Vergelijking logica ontologisch sound
- [ ] Cross-referenties correct en verifieerbaar
- [ ] Bronnen en referenties compleet

---

## Uitbreidingspunten (Optioneel)

**Als validatie volledig slaagt:**
- [ ] Rapport gereed voor juridisch advies toepassingen
- [ ] LegalOntology updates geïmplementeerd
- [ ] Nieuwe artikelen kunnen aan vergelijkingset toegevoegd

**Validatie Status:** ☐ Uitstekend ☐ Goed ☐ Voldoende ☐ Verbeteren ☐ Herschrijven
