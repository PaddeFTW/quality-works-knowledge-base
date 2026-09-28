---
id: analysis-amp-paket-2026-09-04
title: Analysrapport – AMP, risk och skyddsrond
typ: analysrapport
datum: 2026-09-04
beslut: ska_anvandas
---

# ANALYSIS_REPORT – AMP-paket 2026-09-04

**Metod:** Innehållsläsning av original (inte bara filnamn). Tvåsteg: inventering av alla källor, förädling av högt värde. Original orörda.

## 1. Inventering

| Fil | Ämne | Målgrupp | Typ | Rel | Kval | Akt | AI | Dig | Åter | Beslut |
|-----|------|----------|-----|-----|------|-----|----|-----|------|--------|
| Arbetsmiljoplan för bygg - Avancerad mall för större projekt.docx | AMP bygg | BAS-U, platschef, byggherre | Originalmall / blankett | 10 | 8 | 8 | 10 | 10 | 9 | ✅ Struktur |
| Riskbedömning - Arbetsmiljö - Avancerad (Bygg 2026).docx | Riskregister AFS-lista | KMA, BAS | Originalmall | 10 | 7 | 8 | 10 | 10 | 9 | ✅ + rätta AFS |
| Risker inför byggstart 2026.docx | Startcheck särskild risk | BAS-P/U | Originalmall | 9 | 7 | 8 | 9 | 10 | 9 | ✅ |
| Skyddsrond.docx | Generell skyddsrond | Chef, skyddsombud | Originalmall | 8 | 7 | 7 | 9 | 10 | 8 | ✅ bygg-anpassad |
| Master_Kallor_och_Bilagor_Paket.md | Meta-index ISO | produktteam | Index | 7 | 8 | 9 | 7 | 6 | 7 | ⚠ |
| Standard_References_Index.md | Standardkatalog | GAP/RAG | Index | 9 | 9 | 9 | 9 | 8 | 9 | ✅ redan extraherad |

## 2. Kvalitetsfynd i originalen

- AMP-mallen täcker projektinfo, organisation, policy, risköversikt, rond, nödläge, kvittering. Bra digitaliseringsgrund.
- Riskmallen har duplicerade tabeller och blandar AFS 2023:2, 2023:3, 2023:10 och 2023:13 felaktigt. Officiellt: **AFS 2023:3** = samordning/AMP/13 risker. **AFS 2023:13** = risker vid vissa arbeten (bl.a. byggkapitel och asbest).
- "Risker inför byggstart" hänvisar till AFS 2023:3 men listar inte alla 13 officiella punkterna (saknar kassun och strålning; slår ihop andra).
- Skyddsrond är mer industri/lokal än byggplats (ventilation i lokal, truckbatteri). Byggpunkter från AMP-exemplet är mer relevanta på produktion.
- Kommersiella produkter från Kvalitetsgruppen. Ingen verbatim återpublicering.
- Asbeständring AFS 2025:6/2025:8 från 2025-12-19 är korrekt att nämna som tillägg, inte som fristående "AFS 2025:6 asbestföreskrift".

## 3. Överlapp mot befintlig KB

| Ny modul | Befintlig | Hantering |
|----------|-----------|-----------|
| ordnings_skyddsregler (paket) | `ordnings_skotselregler.md` | Kompletterande – denna är byggplats |
| nodlage_olycka | `arbetsmiljo_sakerhet.md`, `nodlagesberedskap_miljo.md` | Kompletterande – projektfält |
| projektorganisation | `projektorganisation_bygg.md` | Samma tema, AMP-fält |
| sdb | `kemikaliehantering_bygg.md` | Kort register + pekare |

Inga fullständiga dubbletter. Paketet ligger i egen mapp.

## 4. Förädling utförd

Skapat `kma_bygg_amp_paket_2026/` med YAML-mallar, platshållare, 5×5-matris, åtgärdstrappa, de 13 officiella riskerna med åtgärder, signatur- och revisionsflöde.

## 5. Manuell granskning kvar

- Licens: använd struktur och kunskap, inte originalens marknadsföring eller supporttexter.
- Jurist/BAS bör stickprovsgranska att åtgärdstexterna inte läses som föreskrift.
- Underliggande ISO-PDF i Master-paketet saknas fortfarande.
