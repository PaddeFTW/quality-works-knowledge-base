# Quality Works Platform – Arkitektur och Teknisk Dokumentation

**Källa:** qualityworksplatform.txt (utvecklarlogg från arkitekturtransformation)  
**Datum:** Cirka 15 dagar före 2026-07-12  
**Syfte:** Beskriva den färdiga, enhetliga arkitekturen för Quality Works-plattformen (Next.js + Supabase) efter omfattande refaktorering  
**Målgrupp:** Utvecklare, arkitekter och produktteam som bygger eller underhåller Quality WorX Apps

---

## Sammanfattning av arkitekturtransformationen

Plattformen har genomgått en fullständig arkitekturöversyn:

- **Från:** Många isolerade, silade moduler med duplicerad kod och saknade komponenter.
- **Till:** En enhetlig domänmodell med 13 centrala entiteter i Supabase, delad typ/hook-lager och konsekvent navigation.

Builden är nu stabil, dev servern körs på port 3000, och appen redirectar korrekt till `/auth/login` när ingen session finns.

---

## Core Domain Model (Supabase)

**13 unified entity tables** med korrekta relationer och auto-numbering:

1. **Departments** – Organisationens avdelningar/struktur
2. **Processes** – Processhantering (Process Engine)
3. **Objectives** – Mål (kvalitet, miljö, arbetsmiljö, affär)
4. **Risks** – Risker med sannolikhet × konsekvens-matris
5. **Legal Requirements** – Lagar och krav (LegalEngine)
6. **Suppliers** – Leverantörer och utvärdering
7. **Customers** – Kunder och kundnöjdhet
8. **Incidents** – Avvikelser/incidenter (auto INC-)
9. **Corrective Actions** – Åtgärder (auto CA-, från planerad → verifierad)
10. **Audits** – Revisioner (auto AUD-)
11. **Audit Findings** – Revisionsfynd
12. **Management Reviews** – Ledningens genomgång
13. **Entity Links** – Kopplingar mellan entiteter (multi-link-stöd)

**Tekniska detaljer:**
- Auto-numbering triggers för Incidents, Corrective Actions och Audits
- Full Row Level Security (RLS) policies på alla tabeller
- Performance indexes på kritiska lookup-kolumner
- Delad TypeScript-interface i `types.ts` (med korrekt nullability och enums)
- Reusable SWR-baserade hooks i `hooks.ts` med felhantering

---

## Shared Domain Layer

- **`/api/domain/*`** – 13 konsekventa API-routes som stödjer GET, POST, PATCH
- Enhetlig dataåtkomst istället för silade moduler
- Stark typning genom hela stacken

---

## Unified Dashboard Navigation

`DashboardLayout` har en ren, konsekvent sidebar med 4 huvudsektioner:

**Kärnprocesser**
- Processer (Process Engine)

**Kvalitetshantering**
- Avvikelser (IncidentsEngine)
- Risker (RiskEngine)
- Mål (ObjectivesEngine)
- Åtgärder (CorrectiveActionsEngine)

**Stödfunktioner**
- Lagar (LegalEngine)
- Leverantörer (SuppliersEngine)
- Kunder (CustomersEngine)
- Årshjul (Annual Cycle)
- Personal (Competency Management / Personal)

---

## 7 Complete Module Engines

1. **ProcessEngine** – Full processhantering med ägarskap
2. **IncidentsEngine** – Avvikelsehantering med multi-link-funktion
3. **RiskEngine** – Riskmatriser med sannolikhet × konsekvens-beräkningar
4. **ObjectivesEngine** – Målspårning över kvalitet/miljö/säkerhet/affär
5. **CorrectiveActionsEngine** – Åtgärdsflöde från planerad → verifierad med evidens
6. **SuppliersEngine** – Leverantörsutvärdering och kritiska leverantörer
7. **CustomersEngine** – Kundnöjdhet och relationshantering

**Ytterligare moduler:**
- **LegalEngine** – Lagar och kravuppföljning (nybyggd)
- **OrganisationEngine** – Avdelningar och struktur
- **Personal** – Kompetensmatris och utvecklingssamtal (uppdaterad)
- **Årshjul** – Årlig aktivitetsplanering (uppdaterad)

---

## Cleanup och teknisk sanering

- 12 gamla, isolerade moduler togs bort (t.ex. miljoutredning och andra icke-anslutna moduler)
- Gamla API-routes raderades
- Konsolidering till en enda enhetlig datamodell
- Shadcn/ui-komponenter installerades vid behov (Select, Input, Dialog m.fl.)
- Byggfel åtgärdades systematiskt (missing components, extra divs, Supabase config, etc.)

---

## Teknisk stack (bekräftad)

- **Frontend:** Next.js (App Router)
- **Backend:** Supabase (PostgreSQL + Auth + RLS)
- **UI:** shadcn/ui + Tailwind
- **Data fetching:** SWR
- **TypeScript:** Fullständig typning via central `types.ts`

---

## Värde för Quality WorX Knowledge Base

Detta dokument är **extremt värdefullt** eftersom det beskriver exakt hur plattformen är uppbyggd. All kunskap i Knowledge Base (onboarding, projektplaner, ISO-referenser, policys, checklistor etc.) kan nu kopplas direkt till:

- Rätt entiteter (t.ex. Risks, Incidents, Legal Requirements)
- Rätt moduler/engines
- Rätt navigation och användarflöden

Detta gör det möjligt att skapa mycket precisa RAG-svar, kodexempel och dokumentation som är 100 % i linje med den faktiska app-arkitekturen.

---

**Status:** Arkitekturen är stabil, builden passerar, och plattformen är redo för vidare utveckling och integration med Quality WorX Knowledge Base.