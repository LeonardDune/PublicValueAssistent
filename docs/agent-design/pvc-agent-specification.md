# PVC Agent Specification

## Overzicht

De PVC Agent is een gespecialiseerde BMAD agent die teams begeleidt bij het ontwerpen van ecosystemen voor publieke dienstverlening. De agent combineert Value Sensitive Design (VSD), Public Value Theory (PVT), en Public Value Canvas (PVC) om ethisch verantwoorde, waarde-gedreven publieke diensten te ontwikkelen.

## Kernexpertise

### 1. Value Sensitive Design (VSD)
- **Conceptual Research**: Identificatie van relevante publieke waarden voor het vraagstuk
- **Empirical Research**: Stakeholder participatie en belangenanalyse met multi-disciplinaire methoden
- **Technical Research**: Vertaling van waarden en belangen naar concrete ontwerpeisen
- **Value Hierarchy**: Systematische ordening van waarden → normen → ontwerpeisen

### 2. Public Value Theory (PVT)
- **Strategic Triangle**: Purpose (publieke waarde) ↔ Support (legitimiteit) ↔ Capacity (middelen)
- **Public Value Creation Process**: Denken en handelen, compleetheid en coherentie, politieke en operationele risico's
- **Public vs Private Value**: Onderscheid tussen uitkomsten, outputs en publieke baten

### 3. Public Value Canvas (PVC)
- **Problem**: Huidige situatie en uitdagingen
- **Envisioned Future**: Gewenste eindtoestand
- **Purpose**: Strategische doelstellingen
- **Team**: Betrokken stakeholders en partners
- **Environment**: Institutioneel en sociaal kader
- **Support**: Politieke en maatschappelijke legitimiteit
- **Capacity**: Beschikbare middelen en competenties
- **Plan**: Uitvoeringsstrategie
- **Public Value Proposition**: Kernaanbod aan samenleving
- **Public Value Account**: Verwachte maatschappelijke baten

### Critical PVC Canvas Relationship Monitoring Requirements

**PVC Agent MOET actief monitoren en beheren:**
- **Inter-element dependencies tracken:** Continue monitoring hoe keuzes in één PVC element invloed hebben op andere elementen, bijvoorbeeld hoe Purpose keuzes Team samenstelling beïnvloeden
- **Cross-impact analysis uitvoeren:** Bij elke keuze analyseren welke effecten dit heeft op bestaande elementen en consequenties voor elementen die nog niet volledig zijn ingevuld
- **Gap identification triggeren:** Automatisch opvallende gaten in inter-element relaties signaleren aan gebruiker, bijvoorbeeld wanneer Environment factoren conflicteren met Support strategie
- **Consequence modeling:** Vooraf analyseren hoe keuzes in één element (bijv. Purpose prioritering) impact hebben op reeds gemaakte keuzes in andere elementen (bijv. bestaande Team commitment)
- **User challenging protocol:** Agent CHALLENGE gebruikers expliciet wanneer inconsistenties tussen PVC elementen worden gedetecteerd, met concrete voorbeelden en suggesties voor herziening

### 6. Public Values Inventory (Jørgensen & Bozeman)
- **72 Publieke Waarden**: Gegroepeerd in constellaties
- **Value Clustering**: Hiërarchie, proximiteit en causaliteit tussen waarden
- **Prime vs Instrumental Values**: Fundamentele vs afgeleide waarden

### 7. Universal Declaration of Human Rights (UDHR)
- **30 Artikelen**: Universele mensenrechten als ethische basis
- **Public Service Context**: Respect voor mensenrechten in dienstverlening

## Workflow Structuur

### Problem Exploratie Workflow
**Doel**: Eerste idee over maatschappelijk vraagstuk concretiseren en uitdagen
**Input**: Initiële probleemhypothese
**Output**: Solide PVC foundation (Problem + Envisioned Future)
**Totale duur**: 4-6 uur (inclusief pauzes)

#### Divergentie Fase - Problem Exploratie

##### 1. 5 Whys & Root Cause Analysis (30-45 min)
**Doel**: Diepgravend naar fundamentele oorzaken
**Input**: Initiële probleem statement
**Output**: Gelaagde oorzaak-analyse

**Gedetailleerde stappen:**
1. Start met initiële probleem statement ("Burgers hebben moeite met toegang tot zorg")
2. Stel eerste "Waarom?" vraag → Antwoord wordt nieuw probleem statement
3. Herhaal 4-5 keer tot fundamentele oorzaak bereikt
4. Valideer keten: Controleer logische verbanden tussen lagen
5. Identificeer systeemfactoren vs individuele factoren
6. Documenteer assumpties en alternatieve interpretaties

##### 2. Problem Reframing Matrix (45-60 min)
**Doel**: Verschillende perspectieven ontdekken
**Input**: Oorzaak-analyse uit stap 1
**Output**: 6-8 alternatieve probleem formuleringen

**Gedetailleerde stappen:**
1. Schrijf kernprobleem in centrum van matrix
2. Reframe vanuit stakeholder perspectieven:
   - Burger: "Ik heb geen toegang tot zorg die ik nodig heb"
   - Overheid: "Ons zorgsysteem is niet efficiënt genoeg"
   - Expert: "Er is sprake van systeemfalen in zorgtoewijzing"
   - Economisch: "Zorgkosten zijn niet duurzaam verdeeld"
3. Reframe in verschillende abstractieniveaus:
   - Specifiek: "Wachttijden zijn te lang"
   - Algemeen: "Toegang tot basiszorg is ongelijk"
   - Kortetermijn: "Dit jaar stijgen zorgkosten"
   - Langetermijn: "Zorgsysteem is niet toekomstbestendig"
4. Test elke reframing tegen empirische data

##### 3. Context Mapping (60-90 min)
**Doel**: Systeemcontext begrijpen
**Input**: Reframing opties uit stap 2
**Output**: Context canvas met stakeholders, krachten, trends

**Gedetailleerde stappen:**
1. Identificeer relevante contextdomeinen:
   - **Sociaal**: Demografie, cultuur, gedragspatronen, ongelijkheid
   - **Politiek**: Beleid, regelgeving, machtsverhoudingen, coalities
   - **Economisch**: Budgetten, incentives, marktkrachten, subsidies
   - **Technologisch**: Digitale systemen, innovatiepotentieel, security
2. Map stakeholders per domein met hun belangen en macht
3. Identificeer drijvende krachten (trends, kansen) en remmende krachten (barrières)
4. Analyseer historische trends en mogelijke toekomstscenario's
5. Documenteer relaties tussen domeinen

#### Divergentie Fase - Envisioned Future Exploratie

##### 4. Visioning Exercises (45-60 min)
**Doel**: Creatieve toekomstbeelden genereren
**Input**: Context analyse uit stap 3
**Output**: 10-15 visionaire scenario's

**Gedetailleerde stappen:**
1. Start met onbeperkte vraag: "Wat als geld geen beperking was?"
2. Verken technologische perfectie: "Wat als AI perfect persoonlijke zorg kon bieden?"
3. Onderzoek ideale samenwerking: "Wat als alle stakeholders perfect samenwerkten?"
4. Creëer extreme scenario's:
   - Best case: Utopische zorgtoegang voor iedereen
   - Worst case: Systeem volledig falen
   - Wild card: Revolutie door nieuwe technologie
5. Focus op gewenste uitkomsten: gezondheid, gelijkheid, kwaliteit van leven

##### 5. Backcasting (60-90 min)
**Doel**: Realistische paden naar toekomst ontdekken
**Input**: Visionaire scenario's uit stap 4
**Output**: Stap-voor-stap roadmap naar toekomst

**Gedetailleerde stappen:**
1. Kies meest gewenste en haalbare toekomstscenario
2. Definieer eindtoestand in concrete termen:
   - Welke resultaten?
   - Voor welke doelgroepen?
   - Op welke termijn?
3. Werk terugwaarts: "Wat moet daarvoor gebeuren?" per mijlpaal
4. Identificeer noodzakelijke tussenstappen en capabilities
5. Test haalbaarheid van elke stap tegen context uit stap 3
6. Creëer alternatieve paden voor verschillende risico's

##### 6. Future State Storyboarding (45-60 min)
**Doel**: Emotionele connectie met toekomst creëren
**Input**: Backcasting resultaten uit stap 5
**Output**: Visuele verhalen van gewenste toekomst

**Gedetailleerde stappen:**
1. Kies 3-5 meest veelbelovende scenario's voor storyboarding
2. Creëer voor elk scenario:
   - **Gebruiker journey**: Typische dag van burger in nieuwe systeem
   - **Emotionele hoogtepunten**: Momenten van vertrouwen, trots, verbetering
   - **Sociale impact**: Hoe samenleving verandert
   - **Technologische elementen**: Rol van innovatie
3. Test verhalen op:
   - Geloofwaardigheid (realistisch?)
   - Aantrekkingskracht (motiverend?)
   - Waardeduidelijkheid (welke publieke waarden centraal?)
4. Identificeer kernwaarden die elk storyboard vertegenwoordigt

#### Integratie Fase

##### 7. PVC Foundation Synthesis (30-45 min)
**Doel**: Problem en Future samenbrengen
**Input**: Alle divergentie outputs (stappen 1-6)
**Output**: Geïntegreerde Problem + Envisioned Future statements

**Gedetailleerde stappen:**
1. Selecteer beste probleem formulering uit stap 2
2. Kies meest haalbare toekomst visie uit stap 5
3. Creëer logische brug: "Deze toekomst lost dit probleem op door..."
4. Test samenhang: Beantwoordt toekomst alle aspecten van probleem?
5. Documenteer assumpties, risico's en succesfactoren
6. Creëer stakeholder-specifieke verbindingen

##### 8. Hypothesis Formation (30 min)
**Doel**: Testbare proposities formuleren
**Input**: Geïntegreerde foundation uit stap 7
**Output**: 3-5 testbare hypotheses voor volgende fase

**Gedetailleerde stappen:**
1. Formuleer "Als... dan..." statements:
   - "Als we digitale zorgnavigatoren inzetten, dan vermindert ongelijke toegang met 30%"
   - "Als we lokale zorghubs creëren, dan verbeteren participatie-cijfers met 25%"
2. Maak hypotheses meetbaar met KPI's
3. Identificeer bewijs dat hypotheses ondersteunt of weerlegt
4. Prioriteer hypotheses op maatschappelijke impact en haalbaarheid
5. Definieer eerste experimenten om hypotheses te testen

### Stakeholder Analysis Workflow

**Doel**: Uitgebreide stakeholder mapping en belangenanalyse, inclusief relatie met publieke waarden
**Input**: Initiële stakeholder lijst uit Context Mapping (Problem Exploratie stap 3)
**Output**: Gedetailleerde stakeholder profielen met waarden-belangen analyse en engagement strategie
**Duur**: 2-3 dagen | **VSD Focus**: Empirical Research

#### Voorbereiding (2 uur)
1. **Stakeholder Database Setup**: Creëer gestructureerde database voor stakeholder data
2. **Analysis Framework Definition**: Definieer analysematrix (macht, belang, invloed, attitude, waarden-alignment)
3. **Data Collection Planning**: Plan interviews, surveys en secondary research
4. **Public Values Framework Integration**: Koppel publieke waarden inventory aan analyse framework

#### Stakeholder Identification Phase (4 uur)

##### 1. Primary Stakeholder Mapping (90 min)
**Doel**: Identificeer directe stakeholders met directe belangen
**Input**: Context mapping resultaten
**Output**: Primaire stakeholder lijst met initiële classificatie

**Stappen:**
1. Identificeer direct betrokken partijen:
   - **Gebruikers**: Burgers, patiënten, klanten die dienst gebruiken
   - **Leveranciers**: Organisaties die inputs leveren
   - **Partners**: Samenwerkende organisaties
   - **Regulatoren**: Overheden en toezichthouders
2. Classificeer per stakeholder type met initiële machtsinschatting
3. Documenteer huidige relatie niveau (neutraal, positief, negatief)

##### 2. Secondary Stakeholder Identification (90 min)
**Doel**: Identificeer indirect betrokken partijen met indirecte invloed
**Input**: Primaire stakeholder lijst
**Output**: Uitgebreide stakeholder ecosysteem map

**Stappen:**
1. Identificeer indirect betrokken partijen:
   - **Belangengroepen**: Vakbonden, patiëntenverenigingen, brancheorganisaties
   - **Media**: Journalisten, influencers, opinieleiders
   - **Experts**: Academici, consultants, thought leaders
   - **Publiek**: Brede samenleving, belastingbetalers
2. Analyseer mogelijke invloed kanalen (social media, politiek, juridisch)
3. Creëer stakeholder invloed netwerk diagram

#### Stakeholder Analysis Phase (8 uur)

##### 3. Power & Interest Analysis (120 min)
**Doel**: Creëer macht-belang matrix voor stakeholder prioritering
**Input**: Uitgebreide stakeholder lijst
**Output**: Geprioriteerde stakeholder matrix

**Stappen:**
1. Beoordeel **macht niveau** per stakeholder:
   - Hoge macht: Kunnen veranderingen blokkeren of afdwingen
   - Lage macht: Beperkte invloed op uitkomsten
2. Beoordeel **belang niveau**:
   - Hoog belang: Sterk beïnvloed door uitkomsten
   - Laag belang: Minimaal beïnvloed
3. Plot stakeholders in macht-belang matrix:
   - **Key Players** (hoog macht, hoog belang): Intensief betrekken
   - **Keep Satisfied** (hoog macht, laag belang): Voldoen houden
   - **Keep Informed** (laag macht, hoog belang): Informeren
   - **Monitor** (laag macht, laag belang): Minimal engagement

##### 4. Public Values-Stakeholder Alignment Analysis (240 min)
**Doel**: Analyseer relatie tussen stakeholder belangen en publieke waarden
**Input**: Stakeholder matrix en publieke waarden inventory
**Output**: Waarden-belangen alignment matrix per stakeholder

**Stappen per key stakeholder:**
1. **Waarden identification**: Welke publieke waarden zijn relevant voor deze stakeholder?
   - Map tegen Jørgensen & Bozeman inventory (72 waarden)
   - Identificeer primary vs instrumental waarden voor stakeholder
2. **Belangen-waarden mapping**:
   - Welke publieke waarden ondersteunen hun belangen? (alignment)
   - Welke publieke waarden conflicteren met hun belangen? (tension)
   - Welke waarden negeren ze of zijn ze onbewust van?
3. **Waarden interpretatie analyse**:
   - Hoe interpreteert stakeholder publieke waarden? (verschillende frames)
   - Voorbeeld: "Efficiency" als kostenbesparing vs toegankelijkheid
   - Identificeer waarden-framing verschillen tussen stakeholders
4. **Waarden-belangen conflict assessment**:
   - Waar ontstaan spanningen tussen stakeholder belangen en publieke waarden?
   - Welke compromissen zijn mogelijk? Onmogelijk?
   - Impact op VSD waardehiërarchie
5. **Waarden-based engagement opportunities**:
   - Welke waarden kunnen gebruikt worden om stakeholder te overtuigen?
   - Welke waarden-framing strategie werkt het beste?

##### 5. Stakeholder Profile Development (180 min)
**Doel**: Creëer gedetailleerde profielen voor key stakeholders inclusief waarden relatie
**Input**: Alignment analyse resultaten
**Output**: Stakeholder profiel database met waarden-belangen matrix

**Stappen per key stakeholder:**
1. **Demografische data**: Grootte, locatie, demographics
2. **Belangen analyse**: Wat willen ze bereiken? Wat vrezen ze?
3. **Huidige positie**: Attitude ten opzichte van probleem/oplossing
4. **Publieke waarden relatie** (samenvatting uit stap 4):
   - Alignment matrix: Welke waarden ondersteunen/conflicteren?
   - Interpretatie verschillen: Hoe zien ze waarden?
   - Waarden-based leverage points: Hoe beïnvloeden?
5. **Invloed strategieën**: Hoe oefenen ze invloed uit?
6. **Communicatie voorkeuren**: Hoe willen ze benaderd worden?
7. **Succes criteria**: Wat zou hen overtuigen? (gekoppeld aan waarden)

##### 6. Relationship & Coalition Analysis (120 min)
**Doel**: Analyseer stakeholder relaties en mogelijke coalities inclusief waarden dimensie
**Input**: Stakeholder profielen met waarden analyse
**Output**: Coalitie map en relatie matrix met waarden alignment

**Stappen:**
1. Map relaties tussen stakeholders met waarden dimensie:
   - Gedeelde vs conflicterende waarden interpretaties
   - Historische samenwerking gebaseerd op waarden alignment
   - Potentiële coalities rond gedeelde waarden
2. Identificeer mogelijke coalities:
   - Waarden-gebaseerde bondgenoten (zelfde interpretatie)
   - Waarden-conflicten die allianties blokkeren
   - Neutrale partijen die via waarden te beïnvloeden zijn
3. Analyseer machtsbalans tussen coalities inclusief waarden leverage

#### Stakeholder Engagement Phase (4 uur)

##### 7. Values-Based Engagement Strategy (120 min)
**Doel**: Ontwikkel stakeholder-specifieke engagement strategieën gebaseerd op waarden relatie
**Input**: Stakeholder profielen met waarden alignment
**Output**: Waarden-informed stakeholder engagement plan

**Stappen per stakeholder groep:**
1. Definieer engagement doelstellingen gekoppeld aan waarden
2. Selecteer waarden-based engagement methoden:
   - **Sterke alignment**: Waarden co-creatie, gezamenlijke waarden statements
   - **Matige alignment**: Waarden dialoog, compromis exploratie
   - **Conflicterende waarden**: Waarden reframing, alternatieve interpretaties
3. Ontwikkel waarden-based communication strategieën
4. Plan engagement timing rekening houdend met waarden sensiviteit

##### 8. Communication Planning (120 min)
**Doel**: Creëer stakeholder-specifieke communicatie strategieën met waarden focus
**Input**: Engagement strategieën
**Output**: Stakeholder communication matrix met waarden messaging

**Stappen:**
1. Ontwikkel key messages per stakeholder groep gekoppeld aan hun waarden
2. Kies communicatie kanalen gebaseerd op waarden-voorkeuren
3. Plan stakeholder-specifieke content met waarden-reframing waar nodig
4. Creëer feedback mechanismen voor waarden dialoog

#### Validatie & Integratie (2 uur)

##### 9. Stakeholder Analysis Validation (60 min)
**Doel**: Valideer compleetheid en accuratesse van analyse inclusief waarden aspect
**Input**: Complete stakeholder analyse met waarden alignment
**Output**: Gevalideerde stakeholder strategie met waarden assurance

**Stappen:**
1. Cross-check waarden-belangen mapping tegen empirische data
2. Valideer waarden interpretaties met stakeholders
3. Test stakeholder strategie tegen historische cases
4. Assess impact op VSD waardehiërarchie

##### 10. PVC & VSD Integration (60 min)
**Doel**: Koppel stakeholder analyse aan PVC elementen en VSD framework
**Input**: Gevalideerde stakeholder analyse
**Output**: PVC stakeholder integratie rapport voor VSD empirical research

**Stappen:**
1. Koppel stakeholders aan PVC Team element
2. Integreer waarden-belangen analyse in PVC Support element
3. Update PVC Environment met stakeholder-waarden dynamics
4. Creëer stakeholder monitoring plan voor VSD voortgang
5. Document waarden conflicts voor VSD tension analysis

**Output Deliverables:**
- Stakeholder Power-Interest Matrix
- Public Values-Stakeholder Alignment Matrix
- Stakeholder Profile Database (inclusief waarden relatie)
- Values-Based Engagement Strategy Document
- Communication Plan met waarden messaging
- PVC-VSD Integration Report voor empirical research

### Value Hierarchy Development Workflow

**Doel**: Systematische ontwikkeling van waardehiërarchieën (waarden → normen → ontwerpeisen) voor ethisch verantwoorde publieke dienst ontwerp
**Input**: Publieke waarden inventory en initiële stakeholder waarden-alignment (uit Stakeholder Analysis)
**Output**: Gevalideerde waardehiërarchie met conflict analyse en ontwerp implicaties
**Duur**: 1-2 dagen | **VSD Focus**: Conceptual Research

#### Voorbereiding (1 uur)
1. **Values Framework Setup**: Koppel Jørgensen & Bozeman inventory aan project context
2. **Hierarchy Template Creation**: Creëer lege hiërarchie template (waarden → normen → eisen)
3. **Stakeholder Values Integration**: Importeer waarden-alignment data uit Stakeholder Analysis
4. **Validation Criteria Definition**: Stel criteria vast voor hiërarchie consistentie

#### Values Identification Phase (3.75 uur)

##### 1. Primary Values Extraction (60 min)
**Doel**: Identificeer meest relevante publieke waarden voor het vraagstuk
**Input**: Problem statement en Envisioned Future
**Output**: Gekorte lijst primaire waarden (8-12 waarden)

**Stappen:**
1. Map probleem tegen waarden inventory:
   - Welke waarden worden geschonden door huidige situatie?
   - Welke waarden worden gerealiseerd in gewenste toekomst?
2. Identificeer domein-specifieke waarden:
   - Gezondheidszorg: equity, accessibility, quality
   - Onderwijs: opportunity, meritocracy, inclusion
   - Milieu: sustainability, stewardship, intergenerational equity
3. Prioriteer op basis van:
   - Impact op probleemoplossing
   - Stakeholder salience (uit Stakeholder Analysis)
   - Constitutionele/fundamentele status

##### 1b. Values Gap Analysis (45 min)
**Doel**: Identificeer ontbrekende waarden, normen en eisen
**Input**: Problem + Envisioned Future vs geïdentificeerde waarden
**Output**: Gap analyse rapport met ontbrekende elementen

**Stappen:**
1. **Problem-to-Values Gap**:
   - Welke waarden zouden moeten gelden maar worden geschonden?
   - Welke impliciete waarden ontbreken in probleemanalyse?
   - Voorbeeld: "Privacy" ontbreekt maar cruciaal voor digitale zorgtoegang

2. **Future-to-Values Gap**:
   - Welke waarden zijn nodig om gewenste toekomst te bereiken?
   - Welke nieuwe waarden ontstaan in toekomstscenario?
   - Voorbeeld: "Digital equity" als nieuwe waarde voor inclusieve toegang

3. **Values-to-Norms Gap**:
   - Welke normen ontbreken voor geïdentificeerde waarden?
   - Welke bestaande normen zijn ontoereikend?
   - Voorbeeld: Waarde "equity" heeft norm "gelijke toegang" maar mist "digitale inclusie"

4. **Norms-to-Requirements Gap**:
   - Welke ontwerpeisen ontbreken voor bestaande normen?
   - Welke eisen conflicteren met gewenste toekomst?
   - Voorbeeld: Norm "privacy bescherming" mist eis "data minimalisatie"

5. **Cross-Context Gaps**:
   - Welke waarden uit andere domeinen zijn relevant?
   - Welke internationale standaarden (zoals UDHR) ontbreken?
   - Welke toekomstige maatschappelijke trends vragen nieuwe waarden?

6. **Gap Prioritization**:
   - Welke gaps zijn kritisch voor probleemoplossing?
   - Welke gaps zijn essentieel voor toekomstrealisatie?
   - Welke gaps hebben hoogste stakeholder impact?

##### 2. Values Clustering & Relationships (60 min)
**Doel**: Analyseer relaties tussen geïdentificeerde waarden
**Input**: Gekorte waarden lijst inclusief gap analyse
**Output**: Waarden relatie matrix met clusters en conflicts

**Stappen:**
1. Creëer waarden affinity matrix:
   - Welke waarden versterken elkaar? (synergie)
   - Welke waarden conflicteren? (trade-offs)
   - Welke waarden zijn neutraal?
2. Identificeer waarden clusters:
   - **Core values**: Fundamenteel voor probleemoplossing
   - **Context values**: Belangrijk in bredere context
   - **Stakeholder values**: Specifiek voor bepaalde groepen
3. Document initiële conflicts:
   - Efficiency vs Equity (kosten vs toegankelijkheid)
   - Privacy vs Transparency (bescherming vs verantwoording)
   - Innovation vs Stability (verandering vs betrouwbaarheid)

##### 3. Stakeholder Values Validation (60 min)
**Doel**: Valideer waarden tegen stakeholder perspectieven
**Input**: Waarden relatie matrix
**Output**: Stakeholder-gevalideerde waarden lijst

**Stappen:**
1. Cross-reference met Stakeholder Analysis:
   - Welke waarden zien stakeholders als primair?
   - Welke waarden worden verschillend geïnterpreteerd?
2. Identificeer waarden interpretatie verschillen:
   - "Efficiency" als kostenbesparing vs kwaliteit vs snelheid
   - "Equity" als gelijke kansen vs gelijke uitkomsten
3. Update waarden lijst met stakeholder insights en gap findings

#### Hierarchy Development Phase (4 uur)

##### 4. Values to Norms Translation (90 min)
**Doel**: Vertaal abstracte waarden naar concrete normen
**Input**: Gevalideerde waarden lijst
**Output**: Initiële waarde-norm hiërarchie

**Stappen per waarde:**
1. Definieer waarde in context van vraagstuk
2. Identificeer afgeleide normen:
   - **Voorbeeld - Equity**: "Iedereen heeft gelijke toegang" (norm)
   - **Voorbeeld - Privacy**: "Persoonsgegevens worden beschermd" (norm)
3. Test norm specificiteit:
   - Is de norm meetbaar/actioneerbaar?
   - Is de norm direct afleidbaar van de waarde?
4. Document rationale voor elke norm

##### 5. Norms to Design Requirements Translation (90 min)
**Doel**: Vertaal normen naar concrete ontwerpeisen
**Input**: Waarde-norm hiërarchie
**Output**: Complete waardehiërarchie (waarden → normen → eisen)

**Stappen per norm:**
1. Identificeer functionele requirements:
   - **Voorbeeld norm "Iedereen heeft gelijke toegang"**:
     - Eis: "Digitale toegankelijkheid voor alle burgers"
     - Eis: "Taalondersteuning voor niet-Nederlands sprekenden"
2. Identificeer niet-functionele requirements:
   - **Voorbeeld**: "Response tijd < 24 uur"
   - **Voorbeeld**: "Privacy compliant met AVG"
3. Test eis haalbaarheid:
   - Technisch mogelijk?
   - Juridisch compliant?
   - Stakeholder acceptable?

##### 6. Hierarchy Consistency Validation (60 min)
**Doel**: Valideer logische consistentie van hiërarchie
**Input**: Complete waardehiërarchie
**Output**: Consistentie rapport met aandachtspunten

**Stappen:**
1. Test verticale consistentie:
   - Leiden eisen terug naar normen? Naar waarden?
   - Zijn er ontbrekende schakels?
2. Test horizontale consistentie:
   - Conflicteren eisen met elkaar?
   - Ondersteunen eisen elkaar?
3. Identificeer aandachtspunten:
   - Zwakke schakels in hiërarchie
   - Potentiële conflicts tussen eisen

#### Conflict Resolution & Refinement Phase (3 uur)

##### 7. Values Conflict Analysis (90 min)
**Doel**: Analyseer en adresseer conflicts tussen waarden
**Input**: Waarden relatie matrix en hiërarchie
**Output**: Conflict resolution strategieën

**Stappen:**
1. Categoriseer conflicts:
   - **Direct conflicts**: Tegenstrijdige eisen (privacy vs transparency)
   - **Indirect conflicts**: Waarden die elkaar beperken
   - **Context conflicts**: Verschillende interpretaties
2. Analyseer impact van conflicts:
   - Op welke ontwerpeisen?
   - Voor welke stakeholders?
   - In welke scenario's?
3. Ontwikkel resolution strategieën:
   - **Prioritering**: Welke waarde weegt zwaarder?
   - **Balancing**: Hoe beide waarden realiseren?
   - **Contextualisering**: Wanneer welke waarde?

##### 8. Hierarchy Refinement & Optimization (60 min)
**Doel**: Optimaliseer hiërarchie gebaseerd op conflict analyse
**Input**: Conflict resolution strategieën
**Output**: Geoptimaliseerde waardehiërarchie

**Stappen:**
1. Pas hiërarchie aan voor conflicts:
   - Voeg conditional logic toe
   - Creëer sub-hiërarchieën voor verschillende contexten
   - Stel prioriteit regels vast
2. Test refined hiërarchie:
   - Lost het conflicts op?
   - Behoudt het waarde integriteit?
3. Document refinement rationale

##### 9. Stakeholder Alignment Validation (60 min)
**Doel**: Valideer hiërarchie tegen stakeholder perspectieven
**Input**: Geoptimaliseerde hiërarchie
**Output**: Stakeholder-gevalideerde waardehiërarchie

**Stappen:**
1. Presenteer hiërarchie aan key stakeholders
2. Verzamel feedback op:
   - Betekenis van waarden voor hen
   - Acceptatie van normen en eisen
   - Concerns over conflicts
3. Integreer stakeholder feedback
4. Finaliseer hiërarchie

#### Integration & Documentation (1 uur)

##### 10. PVC Integration Mapping (30 min)
**Doel**: Koppel waardehiërarchie aan PVC elementen
**Input**: Finale waardehiërarchie
**Output**: PVC-waarden integratie matrix

**Stappen:**
1. Map hiërarchie naar PVC elementen:
   - **Purpose**: Strategische waarden en normen
   - **Public Value Proposition**: Kern ontwerpeisen
   - **Public Value Account**: Verwachte waarde realisatie
2. Identificeer integratie punten voor andere workflows
3. Creëer traceability matrix

##### 11. Documentation & Handover (30 min)
**Doel**: Documenteer hiërarchie voor gebruik in andere workflows
**Input**: Complete hiërarchie en mappings
**Output**: Waardehiërarchie documentatie package

**Stappen:**
1. Creëer hiërarchie visualisatie
2. Document rationale en besluiten
3. Definieer gebruiksrichtlijnen voor andere workflows
4. Stel validatie protocol vast

**Output Deliverables:**
- Complete Value Hierarchy Document
- Values Conflict Analysis Report
- PVC Integration Mapping
- Stakeholder Validation Summary
- Hierarchy Usage Guidelines

### Ecosystem Design Workflow

**Doel**: Ontwerp multi-level samenwerkingsverbanden voor publieke dienst ecosystemen met value co-creation mechanismen
**Input**: PVC foundation, stakeholder analyse en waardehiërarchie
**Output**: Gedetailleerde ecosystem architectuur met governance, processen en monitoring
**Duur**: 2-3 dagen | **VSD Focus**: Technical Research + Ecosystem Integration

#### Voorbereiding (2 uur)
1. **Ecosystem Framework Setup**: Koppel Public Service Logic (PSL) aan project context
2. **Multi-level Architecture Template**: Creëer template voor verschillende ecosystem schalen
3. **Existing Systems Integration**: Import stakeholder ecosystem data
4. **Governance Structure Planning**: Stel governance ontwerp principes vast

#### Ecosystem Analysis Phase (6 uur)

##### 1. Ecosystem Boundaries Definition (120 min)
**Doel**: Definieer scope en grenzen van het te ontwerpen ecosystem
**Input**: PVC foundation en stakeholder analyse
**Output**: Ecosystem boundary matrix met inclusie/exclusie criteria

**Stappen:**
1. Definieer **geografische scope**:
   - Lokaal, regionaal, nationaal, internationaal niveau
   - Natuurlijke grenzen (gemeenten, provincies, landen)
   - Functionele grenzen (dienstketens, waardeketens)
2. Definieer **functionele scope**:
   - Welke diensten en activiteiten behoren tot ecosystem?
   - Welke waarde-creatie processen zijn inbegrepen?
   - Welke grensprocessen verbinden met andere ecosystemen?
3. Definieer **tijdelijke scope**:
   - Korte termijn (0-2 jaar): Basis ecosystem opzetten
   - Middellange termijn (3-5 jaar): Uitbreiding en maturatie
   - Lange termijn (5+ jaar): Volledig geïntegreerd systeem

##### 2. Actor Network Analysis (120 min)
**Doel**: Creëer gedetailleerde netwerkkaart van alle ecosystem actoren
**Input**: Stakeholder analyse resultaten
**Output**: Dynamic actor network diagram met relaties en afhankelijkheden

**Stappen:**
1. Categoriseer actor typen per schaalniveau:
   - **Individueel niveau**: Burgers, professionals, experts
   - **Organisatorisch niveau**: Overheden, bedrijven, NGO's
   - **Institutioneel niveau**: Regelgevers, toezichthouders, financiers
   - **Systeem niveau**: Platformen, standaarden, technologieën
2. Map afhankelijkheidsrelaties:
   - Resource afhankelijkheden (inputs/outputs)
   - Informatie stromen (data uitwisseling)
   - Governance relaties (autoriteit, accountability)
3. Identificeer machtsdynamieken:
   - Wie controleert kritieke resources?
   - Welke actoren hebben vetorecht?
   - Hoe zijn besluitvormingsprocessen georganiseerd?

##### 3. Value Co-creation Pathways (120 min)
**Doel**: Ontwerp mechanismen voor gezamenlijke waarde-creatie
**Input**: Waardehiërarchie en actor netwerk
**Output**: Value co-creation pathway map met interactiepatronen

**Stappen:**
1. Identificeer **waarde-creatie domeinen** per schaalniveau:
   - Individueel: Persoonlijke ervaringen en empowerment
   - Organisatorisch: Service kwaliteit en efficiency
   - Systeem: Maatschappelijke impact en duurzaamheid
2. Ontwerp **co-creation mechanismen**:
   - Participatie platforms voor burger input
   - Samenwerkingsnetwerken tussen organisaties
   - Kennisdeling communities voor professionals
   - Monitoring systemen voor impact meting
3. Definieer **waarde-verdelingsprincipes**:
   - Hoe wordt gecreëerde waarde verdeeld?
   - Welke incentives motiveren deelname?
   - Hoe worden kosten en baten gebalanceerd?

#### Ecosystem Architecture Phase (6 uur)

##### 4. Multi-level Governance Design (180 min)
**Doel**: Creëer governance structuur voor verschillende ecosystem schalen
**Input**: Actor netwerk en institutionele context
**Output**: Governance architectuur document met rollen en verantwoordelijkheden

**Stappen:**
1. Ontwerp **governance lagen**:
   - **Operationeel niveau**: Dagelijkse besluitvorming en coördinatie
   - **Tactisch niveau**: Programma management en resource allocatie
   - **Strategisch niveau**: Visie, beleid en lange termijn richting
2. Definieer **besluitvormingsprocessen**:
   - **Consensus-based**: Voor gedeelde visie en strategie
   - **Representative**: Voor dagelijkse operaties
   - **Expert-based**: Voor technische beslissingen
   - **Participatory**: Voor burger involvement
3. Creëer **accountability mechanismen**:
   - Performance monitoring en rapportage
   - Conflict resolution procedures
   - Escalatie paden voor knelpunten

##### 5. Process Integration Design (120 min)
**Doel**: Ontwerp geïntegreerde processen voor cross-actor samenwerking
**Input**: Value co-creation pathways
**Output**: Integrated process flows met interfaces en handovers

**Gedetailleerde stappen per kernproces:**
1. **Service Delivery Process**:
   - Hoe stromen diensten tussen actoren?
   - Welke interfaces en API's zijn nodig?
   - Hoe wordt kwaliteit geborgd?

2. **Information Exchange Process**:
   - Welke data wordt gedeeld tussen actoren?
   - Welke privacy en security maatregelen?
   - Hoe wordt data kwaliteit gecontroleerd?

3. **Resource Coordination Process**:
   - Hoe worden resources gealloceerd?
   - Welke scheduling en capaciteitsplanning?
   - Hoe worden bottlenecks opgelost?

4. **Innovation & Learning Process**:
   - Hoe worden verbeteringen geïdentificeerd?
   - Welke feedback loops bestaan?
   - Hoe wordt kennis verspreid?

##### 6. Technology Integration Architecture (120 min)
**Doel**: Ontwerp technologische infrastructuur voor ecosystem connectiviteit
**Input**: Process flows en actor capabilities
**Output**: Technology architecture blueprint met integratieprincipes

**Stappen:**
1. Identificeer **technologische bouwstenen**:
   - Shared platforms en digitale diensten
   - Data uitwisselingsformaten en standaarden
   - Identiteits- en toegangsmanagement systemen
   - Monitoring en analytics capabilities
2. Ontwerp **integratieprincipes**:
   - API-first approach voor interoperabiliteit
   - Federated identity management
   - Event-driven architecture voor flexibiliteit
   - Privacy-by-design voor data bescherming
3. Definieer **technologische governance**:
   - Wie beheert welke systemen?
   - Welke compliance vereisten?
   - Hoe worden updates gecoördineerd?

#### Implementation Planning Phase (4 uur)

##### 7. Ecosystem Implementation Roadmap (120 min)
**Doel**: Creëer gefaseerde implementatie aanpak
**Input**: Complete ecosystem architectuur
**Output**: Implementatie roadmap met mijlpalen en dependencies

**Stappen:**
1. Identificeer **implementatie fases**:
   - **Fase 1**: Kern ecosystem opzetten (kritieke actoren en processen)
   - **Fase 2**: Uitbreiding naar volledige scope
   - **Fase 3**: Optimalisatie en maturatie
2. Definieer **success criteria** per fase:
   - Welke metrics meten voortgang?
   - Welke stakeholder acceptatie is nodig?
   - Welke risico's moeten worden gemitigeerd?
3. Creëer **resource planning**:
   - Welke capabilities zijn nodig per fase?
   - Welke training en change management?
   - Welke budgettering en financiering?

##### 8. Risk Assessment & Mitigation (120 min)
**Doel**: Identificeer en adresseer ecosystem-specifieke risico's
**Input**: Governance en proces ontwerp
**Output**: Risk mitigation strategieën voor geïntegreerd systeem

**Stappen per risicocategorie:**
1. **Coördinatie risico's**:
   - Vertrouwensproblemen tussen actoren
   - Onvoldoende commitment van deelnemers
   - Ontbrekende incentives voor deelname
2. **Technologische risico's**:
   - Interoperabiliteitsproblemen
   - Data security en privacy breaches
   - Technologische afhankelijkheden
3. **Institutionele risico's**:
   - Conflicterende reguleringen tussen domeinen
   - Changing politieke prioriteiten
   - Budget onzekerheden
4. **Sociale risico's**:
   - Ongelijke machtsverhoudingen
   - Culturele weerstand tegen verandering
   - Inclusie uitdagingen

##### 9. Monitoring & Evaluation Framework (120 min)
**Doel**: Ontwerp systeem voor voortdurende ecosystem evaluatie
**Input**: Value co-creation pathways en governance structuur
**Output**: Monitoring framework met KPI's en rapportage structuur

**Stappen:**
1. Definieer **comprehensive ecosystem KPI framework** gebaseerd op wetenschappelijke literatuur (Graça & Camarinha-Matos, 2017):

   **A. Structurele Network Indicators (uit Social Network Analysis):**
   - **Centrality Measures**: Degree centrality (netwerk connectiviteit), betweenness centrality (brug functie), closeness centrality (toegankelijkheid)
   - **Cohesion Measures**: Network density, clustering coefficient, reciprocity measures
   - **Resilience Indicators**: Size of largest connected component, network adaptability, disruption recovery capacity

   **B. Collaboration Performance Indicators:**
   - **Effectiviteit** (Service kwaliteit en gebruiker tevredenheid):
     - *Publieke waarden*: Equity, Accessibility, Quality, Human Dignity
     - *Stakeholder focus*: Gebruikers (burgers/patiënten), Service providers
     - *Meetmethode*: Service quality scores, user satisfaction surveys, outcome achievement rates
   - **Efficiency** (Resource gebruik en kosteneffectiviteit):
     - *Publieke waarden*: Sustainability, Accountability, Transparency
     - *Stakeholder focus*: Overheden (belastingbetalers), Service providers (kosten)
     - *Meetmethode*: Cost-benefit ratios, resource utilization efficiency, value-for-money analyses
   - **Innovation** (Nieuwe oplossingen en verbeteringen):
     - *Publieke waarden*: Progress, Adaptability, Future Orientation
     - *Stakeholder focus*: Professionals (ontwikkeling), Innovators (markt kansen)
     - *Meetmethode*: Innovation adoption rates, knowledge creation metrics, learning velocity
   - **Inclusie** (Stakeholders participatie en vertegenwoordiging):
     - *Publieke waarden*: Democracy, Participation, Equity, Social Justice
     - *Stakeholder focus*: Marginalized groups, Community representatives
     - *Meetmethode*: Participation rates, representation equity metrics, inclusion quality scores

   **C. Sustainable Development Indicators (Triple Bottom Line):**
   - **Economische Sustainability**: Long-term financial viability, value capture distribution, ROI stability
   - **Sociale Sustainability**: Community impact, stakeholder equity, social capital building
   - **Ecologische Sustainability**: Environmental impact, resource stewardship, carbon footprint

   **D. Ecosystem Health Indicators:**
   - **Collaborative Capacity**: Trust levels, communication quality, conflict resolution effectiveness
   - **Adaptive Capacity**: Response to changes, innovation absorption, learning agility
   - **Systemic Resilience**: Recovery from disruptions, redundancy levels, system robustness

2. Ontwerp **evidence-based monitoring infrastructuur**:
   - **Structural Network Analytics**: Real-time centrality en cohesion metrics tracking
   - **Value Tracking Layer**: Continue monitoring van publieke waarden realisatie per stakeholder groep
   - **Stakeholder Dashboard**: Real-time inzicht in belangen bevrediging en participatie levels
   - **Resilience Monitoring System**: Automatische detectie van systeem kwetsbaarheden
   - **Sustainability Assessment Framework**: Triple bottom line continuous evaluation
   - **Dynamic KPI Framework**: Self-evolving metrics gebaseerd op ecosystem maturiteit

3. Ontwerp **comprehensive monitoring mechanismen** gebaseerd op wetenschappelijke frameworks:
   - Real-time dashboards voor operationele metrics met waarden en structurele breakdown
   - Periodieke stakeholder surveys met SNA-geïnspireerde participatie analyses
   - Impact assessments voor maatschappelijke waarde creation met sustainability lens
   - Automated alerts voor structurele veranderingen (density shifts, centrality changes)
   - Peer reviews voor systeem verbeteringen met coalition analysis
   - Benchmarking tegen collaborative network best practices

4. Creëer **evidence-based feedback loops** voor continuous improvement:
   - **Data-Driven Decision Making**: Beslissingen gebaseerd op structurele network analytics
   - **Stakeholder Impact Assessment**: SNA-based analyse van decision ripple effects
   - **Resilience Testing Protocols**: Reguliere stresstests voor systeem robustness
   - **Adaptive KPI Evolution**: Metrics die meegroeien met ecosystem complexity
   - **Collaborative Learning Cycles**: Structure-based knowledge sharing optimization
   - **Sustainability Safeguards**: Triple bottom line constraint checking in alle besluiten

#### Validatie & Handover (2 uur)

##### 10. Ecosystem Validation (60 min)
**Doel**: Valideer haalbaarheid en consistentie van ecosystem ontwerp
**Input**: Complete ecosystem architectuur
**Output**: Gevalideerd ontwerp klaar voor implementatie

**Stappen:**
1. Cross-check tegen PVC elementen:
   - Ondersteunt ecosystem de Purpose?
   - Past het binnen Capacity constraints?
   - Bevordert het Public Value Proposition?
2. Stakeholder validation sessies:
   - Actoren commitment check
   - Proces haalbaarheid assessment
   - Risk acceptance evaluatie
3. Technical feasibility review:
   - Systeem integratie test
   - Security en privacy audit
   - Scalability assessment

##### 11. Documentation & Handover (60 min)
**Doel**: Creëer complete documentatie voor ecosystem implementatie
**Input**: Gevalideerde architectuur
**Output**: Implementation package voor ecosystem lancering

**Stappen:**
1. Creëer **ecosystem blueprint document**:
   - Architectuur overzicht en principes
   - Gedetailleerde proces flows
   - Governance structuur document
   - Technologie specificaties
2. Ontwikkel **implementation guides**:
   - Step-by-step onboarding voor nieuwe actoren
   - Operationele procedures en protocols
   - Training materials voor stakeholders
3. Stel **governance kick-off** voor:
   - Eerste vergadering agenda en doelstellingen
   - Initiële besluitvormingsprocessen
   - Monitoring setup en baseline metingen

**Output Deliverables:**
- Ecosystem Architecture Blueprint
- Governance Framework Document
- Implementation Roadmap
- Risk Register & Mitigation Plan
- Monitoring & Evaluation Framework
- Stakeholder Onboarding Package

### Validation & Ethics Check Workflow

**Doel**: Comprehensive validatie van alle PVC-VSD deliverables tegen kwaliteit, ethiek en haalbaarheid criteria
**Input**: Complete PVC document, VSD rapporten, stakeholder analyse, waardehiërarchie
**Output**: Gevalideerd en gecertificeerd ontwerp klaar voor implementatie
**Duur**: 1-2 dagen | **VSD Focus**: Complete Integration & Validation

#### Voorbereiding (1 uur)
1. **Validation Framework Setup**: Stel validatie criteria vast gebaseerd op onze principes
2. **Checklist Compilation**: Creëer comprehensive checklists voor alle aspecten
3. **Review Team Assembly**: Stel onafhankelijke review team samen
4. **Documentation Review**: Controleer compleetheid van alle input deliverables

#### Technische Validatie Phase (3 uur)

##### 1. PVC Completeness Check (60 min)
**Doel**: Verificeer dat alle PVC elementen volledig en consistent zijn
**Input**: Complete PVC document
**Output**: PVC validation rapport

**Validatie criteria:**
- **Problem**: Duidelijk, evidence-based, stakeholder-validated
- **Envisioned Future**: Realistisch, meetbaar, probleem-relevant
- **Purpose**: Strategisch, waarden-anchored, stakeholder-aligned
- **Team**: Complete coverage, commitment levels, governance
- **Environment**: Comprehensive context, institutional fit
- **Support**: Political viability, stakeholder buy-in
- **Capacity**: Resource adequacy, capability gaps addressed
- **Plan**: SMART milestones, risk mitigation, change management
- **Public Value Proposition**: Clear offering, stakeholder value
- **Public Value Account**: Measurable benefits, equity analysis

##### 2. VSD Integration Validation (60 min)
**Doel**: Controleer VSD principes correct toegepast
**Input**: VSD Integration Report
**Output**: VSD compliance assessment

**Validatie criteria:**
- **Conceptual Research**: Waarden geïdentificeerd, hiërarchie compleet
- **Empirical Research**: Stakeholder data robust, belangen gemapped
- **Technical Research**: Ontwerpeisen afleidbaar, haalbaarheid aangetoond
- **Value Conflicts**: Geïdentificeerd en geadresseerd
- **Ethical Integration**: UDHR compliance, mensenrechten gerespecteerd

##### 3. Ecosystem Architecture Validation (60 min)
**Doel**: Valideer ecosystem ontwerp tegen technische en operationele criteria
**Input**: Ecosystem Architecture Blueprint
**Output**: Technical feasibility assessment

**Validatie criteria:**
- **Multi-level Integration**: Processen werken cross-schaal
- **Governance Clarity**: Besluitvorming helder, accountability gedefinieerd
- **Technology Stack**: Interoperabel, scalable, secure
- **Implementation Roadmap**: Realistisch tijdschema, dependencies gemapped

#### Ethiek & Waarden Validatie Phase (4 uur)

##### 4. Public Values Compliance Check (90 min)
**Doel**: Verificeer alignment met publieke waarden inventory
**Input**: Waardehiërarchie, PVC document
**Output**: Values compliance rapport

**Validatie checklist:**
- **Jørgensen & Bozeman Inventory**: Alle relevante waarden geadresseerd
- **Value Conflicts**: Transparant gedocumenteerd en gebalanceerd
- **Stakeholder Values**: Belangen correct geïnterpreteerd en gerespecteerd
- **Implementation Impact**: Ontwerp versterkt (niet ondermijnt) publieke waarden

##### 5. Universal Human Rights Assessment (90 min)
**Doel**: Controleer UDHR compliance van volledige oplossing
**Input**: Complete ontwerp deliverables
**Output**: Human rights impact assessment

**UDHR Checklist (30 artikelen):**
- **Artikel 1-2**: Gelijkheid, non-discriminatie
- **Artikel 3-5**: Leven, vrijheid, bescherming tegen foltering
- **Artikel 6-11**: Rechtspraak, due process, fair trial
- **Artikel 12-17**: Privacy, eigendom, nationaliteit
- **Artikel 18-20**: Vrijheid van meningsuiting, vereniging
- **Artikel 21-22**: Politieke participatie, sociale zekerheid
- **Artikel 23-26**: Arbeid, onderwijs, gezondheid
- **Artikel 27-28**: Cultuur, internationale orde

##### 6. Ethical Dilemma Analysis (60 min)
**Doel**: Identificeer en adresseer ethische trade-offs
**Input**: Value conflicts, stakeholder tensions
**Output**: Ethical decision framework

**Analyse framework:**
- **Dilemma Identification**: Waar ontstaan onoplosbare conflicts?
- **Impact Assessment**: Gevolgen voor verschillende stakeholder groepen
- **Mitigation Strategies**: Hoe minimaliseren we negatieve impact?
- **Transparency Requirements**: Hoe communiceren we besluiten?

##### 7. Equity & Inclusion Audit (60 min)
**Doel**: Controleer eerlijke verdeling van baten en lasten
**Input**: Public Value Account, stakeholder analyse
**Output**: Equity assessment rapport

**Equity criteria:**
- **Benefit Distribution**: Wie profiteert, wie draagt kosten?
- **Access Equity**: Gelijke toegang voor kwetsbare groepen?
- **Procedural Fairness**: Inclusieve besluitvorming?
- **Outcome Equity**: Maatschappelijke impact eerlijk verdeeld?

#### Stakeholder & Feasibility Validatie Phase (3 uur)

##### 8. Stakeholder Validation Sessions (120 min)
**Doel**: Verkrijg stakeholder commitment en feedback
**Input**: Complete ontwerp, stakeholder engagement plan
**Output**: Stakeholder validation rapport

**Validatie aanpak:**
- **Key Players**: Deep-dive review sessies
- **Keep Satisfied**: Confirmation of support
- **Keep Informed**: Feedback op communicatie
- **Monitor**: Minimal validation, focus op concerns

##### 9. Feasibility Assessment (60 min)
**Doel**: Valideer operationele en financiële haalbaarheid
**Input**: Implementation roadmap, capacity analysis
**Output**: Feasibility validation rapport

**Feasibility criteria:**
- **Technical Feasibility**: Technologie beschikbaar, expertise aanwezig
- **Operational Feasibility**: Processen werkbaar, change management plan adequaat
- **Financial Feasibility**: Budget realistisch, funding secured
- **Political Feasibility**: Stakeholder support, regulatory approval

##### 10. Risk Assessment Review (60 min)
**Doel**: Valideer risk mitigation strategieën
**Input**: Risk register, mitigation plans
**Output**: Risk validation assessment

**Risk validation:**
- **Identification**: Alle significante risico's geïdentificeerd
- **Assessment**: Impact en waarschijnlijkheid correct ingeschat
- **Mitigation**: Effectieve strategieën ontwikkeld
- **Monitoring**: Risk tracking mechanisms aanwezig

#### Certification & Handover Phase (1 uur)

##### 11. Final Certification Review (30 min)
**Doel**: Officiële goedkeuring van ontwerp voor implementatie
**Input**: Alle validation rapporten
**Output**: Certification document met implementatie approval

**Certification criteria:**
- **Technical**: Alle kwaliteitseisen gehaald
- **Ethical**: UDHR compliant, publieke waarden gerespecteerd
- **Stakeholder**: Commitment verkregen van key partijen
- **Feasibility**: Operationeel en financieel haalbaar

##### 12. Implementation Handover Package (30 min)
**Doel**: Creëer complete implementatie package
**Input**: Gevalideerd ontwerp, certification
**Output**: Implementation readiness package

**Package contents:**
- **Certified PVC Document**: Officieel goedgekeurde versie
- **VSD Compliance Certificate**: Ethiek en waarden assurance
- **Implementation Roadmap**: Gedetailleerde plan met mijlpalen
- **Risk Mitigation Guide**: Actieplannen voor geïdentificeerde risico's
- **Monitoring Framework**: KPI's en evaluatie methoden
- **Stakeholder Communication Plan**: Engagement strategie voor lancering

**Output Deliverables:**
- Validation Summary Report
- Ethics & Values Compliance Certificate
- Stakeholder Commitment Agreements
- Implementation Readiness Assessment
- Final Design Certification Document

### Implementation Planning Workflow

**Doel**: Gedetailleerde operationalisering van PVC-VSD ecosystem ontwerp met dynamic capabilities voor succesvolle implementatie en duurzaam beheer
**Input**: Gevalideerd PVC document, VSD compliance certificate, ecosystem architectuur, stakeholder commitment
**Output**: Uitvoerbaar implementatieplan met adaptive monitoring en ecosystem leadership capabilities
**Duur**: 1-2 dagen | **Focus**: Operational Excellence & Dynamic Ecosystem Leadership

#### Voorbereiding (1 uur)
1. **Implementation Leadership Assessment**: Evalueer ecosystem leadership capabilities (sensing, seizing, reconfiguring) van beoogde leider
2. **Stakeholder Commitment Validation**: Bevestig ongoing commitment levels en engagement bereidheid
3. **Resource Readiness Check**: Inventariseer beschikbare resources en capability gaps adresseren
4. **Success Definition**: Stel duidelijke success criteria vast gebaseerd op PVC Purpose en ecosystem KPIs

#### Ecosystem Leadership Setup (2 uur)

##### 1. Leadership Capability Mapping (60 min)
**Doel**: Identificeer en versterk dynamic capabilities voor implementation leadership
**Input**: Leadership assessment en ecosystem architectuur
**Output**: Leadership capability roadmap voor implementatie

**Dynamic Capabilities Assessment:**
- **Sensing Capability**: Breed monitoring perspectief en adaptive visie
- **Seizing Capability**: Commitment building en stakeholder persuasion
- **Reconfiguring Capability**: Adaptive probleemoplossing en continuous alignment
- **Gaps & Development Needs**: Ontbrekende capabilities en ontwikkelplan

##### 2. Leadership Role Definition (60 min)
**Doel**: Definieer concrete leadership rollen en verantwoordelijkheden in implementatie
**Input**: Governance framework en leadership capabilities
**Output**: Implementation leadership charter

**Leadership Rollen:**
- **Ecosystem Captain**: Overall visie en strategic direction (sensing focus)
- **Change Orchestrator**: Stakeholder engagement en commitment building (seizing focus)
- **Adaptation Facilitator**: Probleemoplossing en continuous improvement (reconfiguring focus)

#### Roadmap Development Phase (4 uur)

##### 3. Adaptive Implementation Roadmap (120 min)
**Doel**: Creëer dynamische roadmap die inspeelt op veranderende omstandigheden
**Input**: Statische roadmap en sensing capabilities
**Output**: Adaptive implementation roadmap met trigger points

**Adaptive Roadmap Principes:**
- **Phased maar Flexibel**: Milestones als ankerpunten, niet absolute deadlines
- **Trigger-Based Adaptation**: Vooraf gedefinieerde conditions voor course correction
- **Parallel Tracks**: Technische en organisatorische implementatie simultaan
- **Risk-Driven Sequencing**: Hoogste risico's eerst adresseren

##### 4. Resource Allocation Strategy (120 min)
**Doel**: Ontwikkel dynamic resource allocatie gebaseerd op seizing capabilities
**Input**: Budget plan en capability gaps
**Output**: Adaptive resource allocation framework

**Resource Allocation Approach:**
- **Commitment-Based Allocation**: Resources volgen stakeholder commitment
- **Milestone-Gated Releases**: Gefaseerde resource beschikbaarstelling
- **Contingency Reserves**: Flexible buffer voor unforeseen behoeften
- **Value-Based Prioritization**: Resources naar hoogste maatschappelijke impact

#### Change Management Phase (4 uur)

##### 5. Sensing-Driven Change Strategy (120 min)
**Doel**: Ontwikkel change management met continuous monitoring van stakeholder response
**Input**: Stakeholder profiles en sensing capabilities
**Output**: Adaptive change management plan

**Sensing in Change Management:**
- **Sentiment Monitoring**: Continue meting van stakeholder attitude
- **Resistance Detection**: Early warning system voor implementation blockers
- **Engagement Tracking**: Monitor participatie en commitment levels
- **Feedback Integration**: Real-time aanpassing van change aanpak

##### 6. Seizing-Based Commitment Building (120 min)
**Doel**: Bouw en onderhoud ongoing stakeholder commitment tijdens implementatie
**Input**: Stakeholder engagement strategieën
**Output**: Commitment management framework

**Seizing Techniques in Implementation:**
- **Ongoing Persuasion**: Continue reinforcement van waardepropositie
- **Commitment Renewal**: Periodieke reaffirmation van buy-in
- **Participation Incentives**: Rewards voor actieve deelname
- **Alliance Building**: Sterke coalities rond gedeelde belangen

##### 7. Reconfiguring Crisis Management (120 min)
**Doel**: Ontwikkel capability voor adaptive response op implementation challenges
**Input**: Risk register en contingency plannen
**Output**: Dynamic crisis management framework

**Reconfiguring in Implementation:**
- **Rapid Problem Solving**: Ad hoc oplossingen voor unforeseen issues
- **Resource Reallocation**: Flexible deployment van capabilities
- **Process Adaptation**: Continue optimalisatie van implementatie aanpak
- **Stakeholder Re-engagement**: Herstel van commitment bij setbacks

#### Success Measurement & Monitoring Phase (3 uur)

##### 8. Dynamic Success Framework (90 min)
**Doel**: Creëer adaptive success measurement dat meegroeit met ecosystem ontwikkeling
**Input**: Ecosystem KPIs en success metrics framework
**Output**: Dynamic success measurement systeem

**Dynamic Success Measurement:**
- **Evolving Metrics**: Success criteria die mee veranderen met maturity
- **Multi-Level Tracking**: Individueel → organisatorisch → systeem niveau
- **Value-Based Assessment**: Focus op publieke waarde realisatie
- **Learning Integration**: Lessons learned feeden terug in metrics

##### 9. Continuous Monitoring System (90 min)
**Doel**: Implement real-time monitoring voor proactive adaptation
**Input**: Success framework en monitoring capabilities
**Output**: Integrated monitoring dashboard en alert systemen

**Continuous Monitoring Componenten:**
- **Real-Time Dashboards**: Ecosystem health indicators
- **Automated Alerts**: Early warning voor afwijkingen
- **Stakeholder Pulse Checks**: Continue sentiment monitoring
- **Adaptive KPI Adjustment**: Metrics die evolueren met ecosystem

##### 10. Learning & Adaptation Framework (90 min)
**Doel**: Creëer systematische learning loops voor continuous improvement
**Input**: Monitoring data en reconfiguring capabilities
**Output**: Adaptive learning framework voor ongoing optimalisatie

**Learning Framework:**
- **Implementation Reviews**: Regelmatige evaluatie van progress
- **Lesson Capture**: Systematische vastlegging van insights
- **Knowledge Sharing**: Ecosystem-wide verspreiding van learnings
- **Process Optimization**: Continue verbetering gebaseerd op data

#### Implementation Leadership Phase (2 uur)

##### 11. Ongoing Leadership Development (60 min)
**Doel**: Ontwikkel leadership capabilities voor post-implementatie ecosystem management
**Input**: Leadership capability assessment
**Output**: Leadership development roadmap voor ecosystem maturity

**Leadership Development Focus:**
- **Sensing Enhancement**: Uitbreiding monitoring en foresight capabilities
- **Seizing Refinement**: Verbetering stakeholder relationship management
- **Reconfiguring Mastery**: Advanced probleemoplossing en crisis management
- **Succession Planning**: Voorbereiding op leadership transitions

##### 12. Transition to Ecosystem Operations (60 min)
**Doel**: Zorgen voor smooth overgang van implementation naar ongoing operations
**Input**: Complete implementation deliverables
**Output**: Operational readiness assessment en handover plan

**Transition Planning:**
- **Capability Transfer**: Knowledge en process handover naar operations
- **Leadership Continuity**: Ongoing aanwezigheid van leadership capabilities
- **Monitoring Transition**: Van implementation naar operational monitoring
- **Succession Setup**: Structurele borging van ecosystem capabilities

**Output Deliverables:**
- Adaptive Implementation Roadmap
- Ecosystem Leadership Charter
- Dynamic Resource Allocation Plan
- Continuous Monitoring System
- Change Management Playbook
- Success Measurement Framework
- Learning & Adaptation Framework
- Post-Implementation Operations Guide

**Ecosystem Leadership Integration:**
Deze workflow integreert Foss/Schmidt/Teece dynamic capabilities framework:
- **Sensing**: Continuous ecosystem monitoring en stakeholder sensing
- **Seizing**: Ongoing commitment building en resource securing  
- **Reconfiguring**: Adaptive probleemoplossing en ecosystem evolution

Dit zorgt voor een implementation dat niet statisch is, maar dynamisch meegroeit met het ecosystem en uitdagingen adequaat aanpakt.

### Comprehensive PVC-VSD Integration Workflow
**Doel**: Iteratieve ontwikkeling van complete publieke dienst ecosystemen
**Input**: PVC foundation (Problem + Envisioned Future)
**Output**: Valideerbaar ontwerp klaar voor implementatie
**Totale duur**: 2-4 weken (iteratief proces)

#### Voorbereiding (1 dag)
1. **PVC Foundation Review**: Bevestig Problem + Envisioned Future statements
2. **Team Alignment**: Stel kernteam samen en defineer governance regels
3. **Planning**: Creëer overzicht cyclus aanpak en tijdschema
4. **VSD Framework Setup**: Bereid waardehiërarchie template voor

#### Iteratieve Development Cycles (4 cycles × 3-5 dagen)

##### Phase 1: Strategische Context Cycle (Problem → Purpose → Team)

**Doel**: Strategische fundamenten leggen en waarden verankeren
**Duur**: 4-5 dagen | **VSD Focus**: Conceptual Research

**Gedetailleerde stappen:**

1. **Problem Refinement Workshop** (90 min)
   - Deep-dive analyse van probleem statement
   - Stakeholder journey mapping voor huidige situatie
   - Identificeer root cause clusters

2. **Purpose Development Session** (120 min)
   - Afleiden strategische doelstellingen uit Problem-Envisioned Future brug
   - Creëer Purpose statements: "Wat willen we bereiken?"
   - Koppel aan publieke waarden uit inventory

3. **Conceptual VSD Research** (180 min)
   - Identificeer relevante waarden voor strategische context
   - Ontwikkel initiële waardehiërarchie (waarden → normen)
   - Test conceptual consistency tussen Purpose statements

4. **Team Assembly & Roles** (120 min)
   - Identificeer strategische partners en stakeholders
   - Definieer rollen, verantwoordelijkheden en engagement niveau
   - Creëer communication plan voor team

5. **Cycle Synthesis & Validation** (60 min)
   - Beoordeel compleetheid van strategische context
   - Check alignment tussen Problem, Purpose en Team
   - Identificeer escalatie items voor volgende cycles

**Validatie Checkpoint**: PVC-elementen 20-30% compleet, initiële waardehiërarchie vastgesteld

##### Phase 2: Institutionele Context Cycle (Environment → Support)

**Doel**: Institutionele haalbaarheid en legitimiteit waarborgen
**Duur**: 4-5 dagen | **VSD Focus**: Empirical Research

**Gedetailleerde stappen:**

6. **Environment Assessment Deep-Dive** (180 min)
   - **Politiek**: Beleidsanalyse, coalitievorming, besluitvormingsprocessen
   - **Sociaal**: Stakeholders mapping, machtsverhoudingen, cultuur
   - **Economisch**: Budget cycles, incentives, markt dynamics
   - **Juridisch**: Regelgeving, mensenrechten compliancy, risks

7. **Multi-Stakeholder Workshops** (240 min × 2 sessies)
   - Voer VSD Empirical Research uit met betrokken stakeholders
   - Identificeer belangen, concerns en win-win mogelijkheden
   - Valideer institutionele assumpties uit Phase 1

8. **Support Strategy Development** (180 min)
   - Ontwikkel legitimiteit strategie gebaseerd op stakeholder input
   - Creëer politiek draagvlak plan met concrete acties
   - Ontwerp change management aanpak

9. **Legal & Ethics Integration** (120 min)
   - Controleer mensenrechten compliance (UDHR checklist)
   - Identificeer ethische dilemma's en mitigerende maatregelen
   - Integreer compliance vereisten in Support strategie

10. **Institutional Fit Validation** (90 min)
    - Test of voorgesteld ontwerp past binnen institutioneel kader
    - Identificeer institutionele barrières en oplossingen
    - Valideer stakeholder commitment en capaciteit

**Validatie Checkpoint**: PVC-elementen 50% compleet, empirische stakeholder data verwerkt

##### Phase 3: Operationele Context Cycle (Capacity → Plan)

**Doel**: Uitvoering operationaliseren en technische haalbaarheid verzekeren
**Duur**: 4-5 dagen | **VSD Focus**: Technical Research

**Gedetailleerde stappen:**

11. **Capacity Inventory & Assessment** (180 min)
    - Catalogiseer beschikbare middelen, competenties en technologie
    - Beoordeel kwaliteit en beschikbaarheid van capabilities
    - Identificeer capability gaps die Purpose belemmeren

12. **Technical VSD Research** (180 min × 2 sessies)
    - Technical haalbaarheidsanalyse met experts
    - Prototype testing in beperkte setting (proof-of-concept)
    - Iteratieve refinement gebaseerd op technische constraints
    - Validatie van ontwerpeisen uit waardehiërarchie

13. **Resource Gap Analysis** (120 min)
    - Kwantificeer wat ontbreekt om Purpose te bereiken
    - Ontwikkel capability development roadmap
    - Identificeer partnership mogelijkheden voor gaps

14. **Detailed Plan Development** (240 min)
    - Creëer uitvoeringsstrategie met SMART mijlpalen
    - Ontwikkel risico mitigatie strategie (operationeel & politiek)
    - Integreer change management en training requirements
    - Definieer success metrics en monitoring approach

15. **Operational Prototyping** (120 min)
    - Minimal Viable Product (MVP) specificaties
    - Pilot design voor beperkte uitrol
    - Learning objectives voor pilot fase

**Validatie Checkpoint**: PVC-elementen 80% compleet, technische haalbaarheid aangetoond

##### Phase 4: Waarde Context Cycle (Public Value Proposition → Public Value Account)

**Doel**: Waarde propositie finaliseren en maatschappelijke impact verankeren
**Duur**: 4-5 dagen | **VSD Focus**: Complete Integration

**Gedetailleerde stappen:**

16. **Proposition Crafting & Refinement** (180 min)
    - Kernaanbod aan samenleving formuleren op basis van eerdere fases
    - Creëer compelling narrative rond publieke waarde
    - Koppel propositie aan strategische doelstellingen (Purpose)

17. **Value Quantification & Measurement** (180 min)
    - Definieer meetbare publieke baten en outcomes
    - Ontwikkel impact indicators en baseline metingen
    - Creëer logic model: hoe inputs → activities → outputs → outcomes

18. **Impact Modeling & Forecasting** (120 min)
    - Modelleer verwachte maatschappelijke effecten (direct & indirect)
    - Kwantificeer distributie van baten over stakeholders
    - Sensitivity analyse voor verschillende scenario's

19. **Benefit Distribution Analysis** (120 min)
    - Hoe waarde over stakeholders wordt verdeeld (equity analysis)
    - Identificeer win-win opportunities en trade-offs
    - Ontwikkel fairness criteria gebaseerd op publieke waarden

20. **Comprehensive VSD Validation** (120 min)
    - Complete waardehiërarchie toetsen tegen eindpropositie
    - Stakeholder validatie van Proposition en Account
    - Ethiek review en mensenrechten compliance check

**Validatie Checkpoint**: PVC 100% compleet, volledig VSD geïntegreerd

#### Continue Relatie Monitoring & Aanpassingen

**Daily Stand-ups** (15 min/dag):
- Wat is bereikt sinds vorige stand-up?
- Welke impediments zijn geïdentificeerd?
- Wat is de focus voor vandaag?

**Weekly Retrospectives** (90 min/week):
- Wat ging goed in deze cycle/sprint?
- Wat kan verbeterd worden?
- Welke lessons learned voor volgende cycle?

**PVC-VSD Relationship Tracking**:
- Matrix van afhankelijkheden tussen PVC elementen
- Waardeconflict logging en resolution tracking
- Ethiek dilemma's register en besluiten

**Iteratieve Aanpassingen Protocol**:
- Trigger: Verandering >15% impact op andere elementen
- Process: Rapid assessment → Team consultation → Adjustment plan
- Documentation: Rationale en impact analyse

#### Output Deliverables
- **Complete PVC Document**: Alle 11 elementen ingevuld
- **VSD Integration Report**: Waardehiërarchie, stakeholder analyse, ethiek review
- **Implementation Roadmap**: Gedetailleerde plan met mijlpalen
- **Validation Package**: Evidence voor besluiten en assumpties
- **Risk Register**: Operationele, politieke en ethische risico's met mitigatie

## Integratie Principes

### PVC-VSD Integratie
- **Conceptual Research** → PVC Problem/Purpose/Public Value Account
- **Empirical Research** → PVC Team/Environment/Support
- **Technical Research** → PVC Capacity/Plan/Public Value Proposition

### Ecosystem Perspective
- **Multi-level Analysis**: Stakeholders en waarden op verschillende schaalniveaus
- **Co-creation Focus**: Waarde-creatie als systeemeigenschap
- **Institutional Fit**: Ontwerp dat past binnen bestaande arrangementen

### Ethical Framework
- **Human Rights Foundation**: UDHR als ethische bodem
- **Public Values Priority**: Maatschappelijke waarde boven individuele belangen
- **Participatory Design**: Inclusieve besluitvorming

## Validatie Criteria

### Technisch
- Alle PVC elementen ingevuld en onderling consistent
- VSD waardehiërarchie compleet en getest
- Stakeholder belangen geïdentificeerd en gebalanceerd

### Ethiek & Waarden
- Conform UDHR mensenrechten
- Publieke waarden gerespecteerd en bevorderd
- Spanningen tussen waarden geanalyseerd en geadresseerd

### Ecosystem
- Multi-level samenwerking mogelijk
- Institutionele arrangementen onderbouwd
- Value co-creation mechanismen gedefiniëerd

## Implementatie Aandachtspunten

### BMAD Framework Integration
- Workflow structuur volgens BMAD Core Task standards
- Agent configuratie via BMB/BMM modules
- Logging en audit trails voor design decisions

### Team Facilitatie
- Participatieve methoden voor stakeholder engagement
- Iteratieve feedback loops
- Escalatie procedures voor ethische dilemma's

---

*Dit document vertegenwoordigt de huidige stand van de PVC Agent ontwikkeling gebaseerd op uitgebreide brainstorming sessies. De specificatie is iteratief en kan worden uitgebreid met aanvullende expertise, workflows en validatie criteria.*
