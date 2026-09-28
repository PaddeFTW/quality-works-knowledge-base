# ANALYSIS_REPORT.md

**Quality WorX Knowledge Base – Analysrapport**  
**Senast uppdaterad:** 2026-09-19  
**Aktuell batch:** Kvalitetsdokument.se – ledningssystem + SAM <10 (Steg 1)  
**Steg denna körning:** Endast Steg 1 inventering. Inga nya kb-moduler.

Originalfiler orörda. Tidigare batcher (2026-08-19 miljöplan, 2026-09-04 AMP, 2026-09-17 ISO-frågebank) ligger kvar.

---

## 0. Batch 2026-09-19 – sammanfattning

Sju källor inlästa från `attachments/` (samma paket som delvis inventerades 2026-07-12). Ny fil mot tidigare KomIgång-rapport: **Arbetsmiljö under 10 anställda.dotx**.

| Nyckeltal | Värde |
|-----------|-------|
| Källfiler i denna batch | 7 |
| Ska användas (Steg 2 tillåten) | 2 |
| Kräver manuell granskning | 4 |
| Dubblett | 1 |
| Nya kb-moduler denna körning | 0 (Steg 1) |

Filter mot gällande: AFS 2023:1 / 2023:3 / 2023:13, ISO 9001:2026, ISO 14001:2015+AMD 2024 (14001:2026-PDF saknas), ISO 45001:2018+AMD 2024.

**Huvudfynd**

- Endast **Arbetsmiljö under 10 anställda.dotx** når både Relevans ≥ 8 och Aktualitet ≥ 7 *och* ger ny SAM-kunskap för QW Light (2–10 anställda).
- **Processbild PDCA och SWOT.pptx** når tröskeln som process-stomme (PDCA gäller fortfarande). Innehållet är tunt; Steg 2 ska bli en kort modul, inte slide-för-slide.
- **Kom igång** och **Kvalitets- och miljömanual** är fortfarande värdefulla som *struktur*, men aktualitet 6 mot 9001:2026. Får inte bli kravtext. Redan extraherad stomme finns i `komma_igang_ledningssystem.md` (utan MVP-frontmatter, 2015-språk).
- **Master-paketet** och **Standard_References_Index** listar AFS 2001:1 och DIS 9001:2025 som om de vore gällande 2026-krav. Katalogvärde kvar, kravvärde nej.
- Inget av dokumenten får kopieras verbatim (Kvalitetsdokument.se / SIS).

---

## 1. Steg 1 – klassificering (batch 2026-09-19)

| Fil | Syfte (en mening) | Ämne | Appar | Målgrupp | Ålder | Rel | Akt | Beslut |
|-----|-------------------|------|-------|----------|-------|-----|-----|--------|
| Master_Kallor_och_Bilagor_Paket.md | Påstår sig vara komplett källindex för ISO-produkter. | iso / ovrigt | — | produkt | 2026-05-11 | 7 | 5 | Kräver manuell granskning |
| Standard_References_Index.md | Detaljerad filkatalog över uppladdade standarder och föreskrifter. | iso | internrevision | revisor | 2026-05-11 | 8 | 5 | Kräver manuell granskning |
| Kom igång med ert ledningssystem.docx | Steg-för-steg för att införa integrerat kvalitets- och miljöledningssystem. | kvalitet / miljo / ledning | qw-light, qw-small, qw-web, quiz, onboarding | VD, kvalitetsansvarig | 2015-mall (Kvalitetsdokument.se) | 9 | 6 | Kräver manuell granskning |
| Kvalitets och miljömanual.docx | Ifyllbar Q+E-manualmall (policy, processer, mål, avvikelse, ledningens genomgång). | kvalitet / miljo / ledning | qw-web, dokumentgenerator, quiz | VD, kvalitetsansvarig | 2015-struktur + bygg-ÄTA | 9 | 6 | Kräver manuell granskning |
| Processbild PDCA och SWOT.pptx | Översikt PDCA, intressent/huvud/stöd/ledning plus tom SWOT. | ledning | qw-light, qw-web, quiz | VD | odaterad mall | 8 | 7 | Ska användas |
| Processer.pptx | Samma processkarta som ovan, utan SWOT/PDCA-lista. | ledning | qw-web | VD | odaterad mall | 7 | 7 | Dubblett |
| Arbetsmiljö under 10 anställda.dotx | SAM-stomme för arbetsgivare med färre än tio anställda. | arbetsmiljo / hr | qw-light, amp, onboarding, egenkontroll | VD, skyddsombud | AFS 2023:1 nämnd | 10 | 8 | Ska användas |

### Per fil – fastställt innehåll (läst, inte bara filnamn)

**Master_Kallor_och_Bilagor_Paket.md**  
Klassificering: AI-underlag / Index. Påstår juridisk 10/10 och att alla källor är “gällande lag 2026”. Listan innehåller AFS 2001:1, SOSFS 2011:9, ISO 9001:2015, ENQ-2092 DIS 9001:2025, OHSAS 18002:2009. Överlapp: `Standard_References_Index.md`, `standard_references_katalog.md`. Inte kravkälla.

**Standard_References_Index.md**  
Klassificering: Index / Standard-katalog. Samma luckor i lagår. Användbart som intern filförteckning, inte som “detta gäller”. Överlapp-id: Master-paketet.

**Kom igång med ert ledningssystem.docx**  
Klassificering: Originalmall. Producent Kvalitetsgruppen Hässleholm AB. 27 praktiska steg: arbetsgrupp, omfattning, intressenter, dokumentstyrning, miljöutredning, policy, mål, processer, leverantör, kundnöjdhet, avvikelse, internrevision, utbildning, ledningens genomgång, certifiera eller inte. Refererar ISO 9001:2015 och ISO 14001:2015 (en gång 14001:2014). Innehåller sälj för egen support och namngivna certifieringsbolag. Överlapp: `komma_igang_ledningssystem.md` (redan utdragen 2026-07-12), `projektplan_iso_implementering.md`.

**Kvalitets och miljömanual.docx**  
Klassificering: Originalmall. Kapitel 1–9: verksamhet, omfattning, ledarskap/policy, SWOT och miljöaspekter, processer (sälj–inköp–produktion–leverans, ÄTA), stöd, möten, dokumentstyrning, årlig utvärdering (kund, laglista, internrevision, avvikelse, förbättring, nödläge, ledningens möte). Exempelpolicyer är generiska säljtexter. Överlapp: `kma_manual_struktur_overview.md`, miljöplan-moduler 2026-08-19, Fragobank avsnitt ledning/verksamhet.

**Processbild PDCA och SWOT.pptx**  
Klassificering: Originalmall / Process. Innehåller: intressent → huvudprocess → nöjd intressent; ledningsprocesser (affärsplan, policy, mål); stöd (inköp, admin, utbildning, miljö); PDCA-lista kopplad till årliga LS-aktiviteter; tom SWOT-ruta. PDCA-cykeln stämmer mot hur 9001/14001/45001 fortfarande beskrivs. Inga lagår i sliden.

**Processer.pptx**  
Klassificering: Dubblett. Samma processkarta som Processbild, utan SWOT och utan PDCA-aktivitetslistan.

**Arbetsmiljö under 10 anställda.dotx**  
Klassificering: Originalmall. Säger uttryckligen AFS 2023:1 och att dokumentationskravet är lättare under tio anställda (uppgiftsfördelning och årlig uppföljning behöver inte dokumenteras). Innehåll: årshjul, arbetsgivare/arbetstagare, arbetsmiljöpolicy, diskrimineringspolicy, samråd, skyddsombud/skyddsrond/riskbedömning (inkl. kemikalier), information, medarbetarsamtal, introduktion, personalenkät, tillbud/arbetsskada (länk AV-blankett + anmalarbetsskada.se), säkerhetsdatablad, ordning och reda, årlig uppföljning. Överlapp: `arbetsmiljo_sakerhet.md` (fortfarande AFS 2001:1), AMP-paket skyddsrond (bygg/BAS, inte kontor/<10), `uppföljningssamtal.md`. Primär för QW Light SAM – inte ersättning för bygg-AMP.

---

## 2. Beslut mot Steg 2-tröskel

Steg 2 tillåten bara om Relevans ≥ 8 **och** Aktualitet ≥ 7 **och** beslut = Ska användas.

| Fil | Steg 2? | Tänkt modul om/när Steg 2 körs |
|-----|---------|--------------------------------|
| Arbetsmiljö under 10 anställda.dotx | Ja | `kb/kb-arbetsmiljo-sam-under-10.md` (årshjul, vad som måste / inte måste dokumenteras, skyddsrond, tillbud). Ev. delad: policy, diskriminering, SDS. Max 400–800 ord/fil. |
| Processbild PDCA och SWOT.pptx | Ja | `kb/kb-ledning-pdca-oversikt.md` – kort PDCA + processnivåer. Inte slidekopiering. |
| Övriga fem | Nej | Ingen ny kb-fil. Befintlig `komma_igang_ledningssystem.md` märks outdated/unverified mot 2026. |

MVP-luckor som denna batch **inte** fyller: `kb-iso-45001-krav`, `kb-iso-27001-krav`, `kb-laglista-efterlevnad`, `kb-internrevision-gap`, `kb-ledningens-genomgang` (manualen har avsnitt men aktualitet 6).

---

## 3. Luckor och varningar

- ISO 9001:2026 IS-text saknas fortfarande (DIS i `Standarder/`).
- ISO 14001:2026-PDF saknas.
- Kom igång / manualen får inte presenteras som “uppfyller 9001:2026”.
- `arbetsmiljo_sakerhet.md` i onboarding citerar fortfarande AFS 2001:1.
- Master-paketet nämner AFS 2001:1 som SAM-källa – fel mot AFS 2023:1.
- Kommersiell mall: sammanfatta, inte återge policytexter ordagrant.
- Certifieringsbolag och telefonnummer i Kom igång är sälj, inte kunskap.

---

## 4. Tidigare batch 2026-09-17 (oförändrad sammanfattning)

Filter då: bygg/entreprenad <50, ISO 9001:2026 + ISO 14001.

| Nyckeltal | Värde |
|-----------|-------|
| Källfiler | 12 |
| Ska användas | 8 |
| Nya kb-moduler | 6 + 5 informationsägare |

ISO 9001:2026 publicerad 2026-09-16. Paketet har ISO/DIS 9001:2025, inte IS. ISO 14001:2026-PDF saknas.

Se `kb/` för de modulerna. Fältkälla ISO Quiz: `Fragobank_v2/templates/fragobank/21_Information_och_Bevis.md`.

---

## 5. Äldre batcher

- 2026-08-19: Miljöplan + standardkatalog (8 MD).
- 2026-09-04: AMP-paket 19 MD i `kma_bygg_amp_paket_2026/`.
- 2026-07-12: KomIgång-paketet extraherat till `komma_igang_ledningssystem.md` med 2015-antagande. Den filen är inte MVP-frontmatter och ska inte användas som gällande ISO-krav.
