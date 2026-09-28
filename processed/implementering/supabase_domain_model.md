# Supabase Domänmodell – Quality Works Plattform

**Källa:** qualityworksplatform.txt (AI-rebuild log 2026)  
**Syfte:** Beskriva den enhetliga datamodellen som ligger till grund för Quality WorX-plattformen  
**Målgrupp:** Utvecklare, arkitekter, konsulter och AI-agenter som bygger eller integrerar med Quality WorX Apps  
**Version:** Baserad på rebuild 2026

---

## Översikt

Quality Works-plattformen använder en **enhetlig Supabase-domänmodell** med 13 kärntabeller. Modellen är designad enligt Annex SL-principer för att stödja integrerade ledningssystem (ISO 9001, ISO 14001, ISO 45001) i en enda databasstruktur.

Modellen ersatte en tidigare splittrad arkitektur med isolerade moduler och konsoliderades till ett gemensamt domänlager.

---

## De 13 enhetliga tabellerna

| Tabell | Beskrivning | Nyckelfunktioner |
|--------|-------------|------------------|
| **Departments** | Avdelningar och organisation | Hierarkisk struktur, koppling till processer och personal |
| **Processes** | Processer och processägarskap | Ägarskap, koppling till mål, risker och avvikelser |
| **Objectives** | Mål (kvalitet, miljö, arbetsmiljö, affär) | Måluppföljning, koppling till processer och åtgärder |
| **Risks** | Risker | Sannolikhet × Konsekvens-beräkning, riskmatris |
| **Legal Requirements** | Lagkrav och efterlevnad | Compliance-status, koppling till processer och revisioner |
| **Suppliers** | Leverantörer | Utvärdering, kritiska leverantörer, prestanda |
| **Customers** | Kunder | Nöjdhetsmätning, relationer, feedback |
| **Incidents** | Avvikelser och incidenter | Auto-nummerering (INC-), multi-länkning till andra entiteter |
| **Corrective Actions** | Korrigerande åtgärder | Livscykel (planerad → verifierad), evidens, koppling till incidenter |
| **Audits** | Revisioner | Auto-nummerering (AUD-), planering och genomförande |
| **Audit Findings** | Revisionsfynd | Koppling till revisioner och åtgärder |
| **Management Reviews** | Ledningens genomgång | Mötesprotokoll, beslut, uppföljning |
| **Entity Links** | Generisk länkning mellan entiteter | Flexibel relation mellan alla tabeller (t.ex. incident ↔ process ↔ risk) |

---

## Nyckelfunktioner i databasen

### Auto-numbering triggers
- **Incidents:** INC-XXXXX
- **Corrective Actions:** CA-XXXXX
- **Audits:** AUD-XXXXX

### Row Level Security (RLS)
- Full RLS-policies på alla tabeller
- Säkerställer att användare endast ser data de har behörighet till (baserat på organisation/avdelning)

### Performance indexes
- Index på kritiska lookup-kolumner (t.ex. status, owner_id, department_id, created_at)

### Entity Links
- Generisk länk-tabell som möjliggör flexibla relationer mellan alla entiteter utan att skapa dedikerade foreign keys för varje kombination.

---

## Gemensamt domänlager (Shared Domain Layer)

### types.ts
Kompletta TypeScript-interfaces för alla 13 entiteter med:
- Korrekt nullability
- Enums för status, typer och kategorier
- Relationer mellan entiteter

### hooks.ts
Återanvändbara SWR-baserade datahämtning-hooks med:
- Error handling
- Loading states
- Automatisk revalidering

### API-rutter
13 konsekventa domän-API:er under `/api/domain/*` som stödjer:
- GET (lista + detalj)
- POST (skapa)
- PATCH (uppdatera)

Exempel: `/api/domain/incidents`, `/api/domain/risks`, `/api/domain/corrective-actions`

---

## Stöd för ISO-standarder

Modellen är byggd för att direkt stödja:
- **ISO 9001** – Processer, mål, avvikelser, korrigerande åtgärder, revisioner, ledningens genomgång
- **ISO 14001** – Miljörisker, lagkrav, leverantörer, mål
- **ISO 45001** – Arbetsmiljörisker, incidenter, personal, lagkrav
- **Annex SL** – Gemensam struktur för integrerade ledningssystem

---

## Användning i Quality WorX Apps

- **ProcessEngine** – Hanterar processer med ägarskap och kopplingar
- **IncidentsEngine** – Fullständig avvikelsehantering med multi-länkning
- **RiskEngine** – Riskmatriser och beräkningar
- **ObjectivesEngine** – Måluppföljning över flera områden
- **CorrectiveActionsEngine** – Åtgärdscykel från planerad till verifierad
- **LegalEngine** – Efterlevnad av lagkrav
- **SuppliersEngine** & **CustomersEngine** – Intressenthantering

Modellen möjliggör en enhetlig vy över kvalitet, miljö och arbetsmiljö i en och samma plattform.

---

## Rekommendationer för vidareutveckling

- Utöka Entity Links för att stödja mer komplexa relationer
- Lägg till versionering på kritiska entiteter (t.ex. processer och policyer)
- Implementera audit-logs på alla ändringar (för spårbarhet)
- Skapa vyer för dashboards och rapportering direkt i Supabase

---

**Status:**  
Denna modul är redo att användas direkt i RAG, dokumentation, utbildningsmaterial och som referens vid vidareutveckling av Quality WorX Apps.

Den utgör kärnan i den digitala plattformen som stödjer hela kunskapsbanken.