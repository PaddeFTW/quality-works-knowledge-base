# App-template – startmall och produktfiler

**Källa:** GitHub `PaddeFTW/app-template` (officiell GitHub-template, senast pushad 2026-08-30)  
**Datum analys:** 2026-08-30  
**Typ:** Originalmall / Projektunderlag / AI-underlag  
**Repo:** https://github.com/PaddeFTW/app-template  

---

## Vad det är

Officiell startmall för framtida Quality Works-appar.  
Enligt källan är repot **en plattformsgrund, inte en produkt**.

Ingår:

- delad arkitektur
- design tokens
- layout-skal
- UI-primitiver
- dokumentationsstandard
- produktprinciper i markdown

Ingår **inte** (enligt PROJECT_BRIEF och README):

- affärslogik
- produktspecifika sidor
- domänspecifika formulär
- mockade arbetsflöden som “riktiga funktioner”

---

## Produktfiler i markdown (kunskapskällor)

| Fil i repot | Syfte |
|-------------|-------|
| `PROJECT_BRIEF.md` | Syfte, vad det är/inte är, produktfamiljer, constraints |
| `AGENTS.md` | Regler för AI-agenter och bidrag |
| `DESIGN_SYSTEM.md` | Semantiska tokens, tema, komponentlager |
| `ARCHITECTURE.md` | Lagerregler, layouts, routing |
| `ROADMAP.md` | Fas 1–4 för mallen (inte produktroadmaps) |
| `README.md` | Översikt och non-goals |
| `CHANGELOG.md` | Versionshistorik |
| `docs/QUALITY_WORX_PRODUCT_PRINCIPLES.md` | 15 produktprinciper + Guided Workflow Engine |
| `docs/getting-started.md` | Startguide |
| `docs/extending-the-template.md` | Hur mallen utökas |

Dessa MD-filer är **produkt- och plattformskunskap**. De ska användas i Knowledge Base. Själva koden i `app/` och `components/` är inte kunskapsbankens uppdrag.

---

## Produktfamiljer som enligt brief ska byggas ovanpå mallen

- Onboarding
- Quality Plan / Kvalitetsplan
- Work Environment Plan / Arbetsmiljöplan
- Risk Assessment / Riskbedömning
- Environmental Inspection / Miljöutredning
- Self Inspection / Egenkontroll
- Control Plan / Kontrollplan
- Document Management
- ISO Manual

---

## Layoutskal (endast struktur, enligt källan)

- AppLayout
- DashboardLayout
- DocumentLayout
- SettingsLayout

---

## Koppling till Knowledge Base

Kunskapsbanken levererar innehåll (processer, checklistor, termer, frågor) som senare kan användas av appar som klonas från denna mall.

Knowledge Base ska **inte** utveckla eller ändra `app-template`.
