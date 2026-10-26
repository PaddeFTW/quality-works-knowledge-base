# CONTENT_INDEX.md

**Quality WorX Knowledge Base – Innehållsförteckning**  
**Senast uppdaterad:** 2026-10-26

---

## 0. Denna körning (2026-09-19) – inga nya kb-moduler

Steg 1 endast. Kandidater till Steg 2 (inte skapade ännu):

| Tänkt id | Källa | Appar | Domain | Status |
|----------|-------|-------|--------|--------|
| kb-arbetsmiljo-sam-under-10 | Arbetsmiljö under 10 anställda.dotx | qw-light, amp, onboarding, egenkontroll | arbetsmiljo | Steg 2 tillåten |
| kb-ledning-pdca-oversikt | Processbild PDCA och SWOT.pptx | qw-light, qw-web, quiz | ledning | Steg 2 tillåten, kort fil |

Ej Steg 2: Kom igång, Q+E-manual, Master, Index (aktualitet / manuell), Processer.pptx (dubblett).

---

## 1. MVP-moduler 2026-09-17 (ISO 9001:2026 + ISO 14001, bygg <50)

| Modul | Appar | Domain |
|-------|-------|--------|
| `kb/kb-iso-termer-bygg.md` | qw-light, qw-small, qw-web, quiz, onboarding | iso |
| `kb/kb-iso-9001-2026-nytt.md` | qw-light, qw-small, qw-web, quiz | iso |
| `kb/kb-iso-14001-2026-nytt.md` | qw-web, miljouredning, quiz | miljo |
| `kb/kb-fragobank-9001-bygg-kontext-planering.md` | qw-web, quiz | kvalitet |
| `kb/kb-fragobank-9001-bygg-verksamhet.md` | qw-web, quiz, egenkontroll | kvalitet |
| `kb/kb-fragobank-14001-bygg.md` | miljouredning, egenkontroll, quiz | miljo |
| `kb/kb-fragobank-informationsagare.md` | quiz, qw-web, internrevision | ledning |
| `kb/kb-fragobank-9001-agare.md` | quiz, internrevision | kvalitet |
| `kb/kb-fragobank-14001-agare.md` | quiz, miljouredning, internrevision | miljo |
| `kb/kb-fragobank-45001-agare.md` | quiz, amp, internrevision | arbetsmiljo |
| `kb/kb-fragobank-27001-agare.md` | quiz, internrevision | infosakerhet |

Ersätter som primär frågebank: `Fragobank_v2/templates/fragobank/01_ISO9001_Fragobank.md` och `02_ISO14001_Fragobank.md` (2015, klausul-språk).

MVP som fortfarande saknas: kb-iso-9001-krav, kb-iso-14001-krav, kb-iso-45001-krav, kb-iso-27001-krav, kb-fragobank (kanon), kb-skyddsrond, kb-riskbedomning, kb-miljoaspekter-kemikalier, kb-laglista-efterlevnad, kb-internrevision-gap, kb-ledningens-genomgang. Delar täcks av AMP-paket och miljöplan-MD utan MVP-id.

---

## 2. Onboarding (tidigare, oförändrade)

`onboarding_process.md`, `foretagsinformation.md`, `arbetstid_administration.md`, `ledighet_sjukdom_foraldraledighet.md`, `friskvard_foretagshalsovard.md`, `arbetsmiljo_sakerhet.md`, `forbattringsverksamhet.md`, `fackliga_fragor.md`, `ordnings_skotselregler.md`, `foretagspolicy.md`, `kvittering_foretags_egendom.md`, `larmrutiner.md`, `bekraftelse_information.md`, `uppföljningssamtal.md`

`arbetsmiljo_sakerhet.md` ska inte användas som SAM-kravkälla (AFS 2001:1). Se OUTDATED_CONTENT.md.

## 3. Miljöplan-moduler 2026-08-19

`miljoplan_byggprojekt.md`, `miljo_policy_exempel.md`, `miljoaspekter_bygg.md`, `nodlagesberedskap_miljo.md`, `kemikaliehantering_bygg.md`, `egenkontroll_miljo.md`, `avfall_kallsortering_bygg.md`, `standard_references_katalog.md`

## 3b. AMP-paket 2026-09-04

Mapp `kma_bygg_amp_paket_2026/` (AMP, BAS-roller, 13 särskilda risker, riskmatris, skyddsrond bygg). Byggplats – inte samma som SAM <10 på fast arbetsställe.

## 4. Relaterade startunderlag

| Fil | Roll |
|-----|------|
| `komma_igang_ledningssystem.md` | Äldre utdrag ur Kom igång-docx (2015). Inte MVP. |
| `kma_38_startfragor.md` | 38 startfrågor KMA |
| `iso_krav_mapping_kma.md` | Koppling 2015-avsnitt ↔ frågor |
| `Fragobank_v2/templates/fragobank/10_Bred_Fragobank_Alla_Standarder.md` | A–G-frågor ISO Quiz |
| `Fragobank_v2/templates/fragobank/21_Information_och_Bevis.md` | Fält per fråga: VD, ägare, ställe, bevis |
| `Fragobank_v2/templates/fragobank/` | Produktpaket 00–21 |
| `Standarder/ISO 9001/` | DIS 9001:2025 + 2015 + AMD 2024 |
| `Standarder/ISO 14001/` | 2015 + AMD 2024 |

## Status

**Steg 1:** Klar för batch 2026-09-19.  
**Steg 2:** Inte körda för 2026-09-19. Väntar godkännande av tröskelfilerna SAM <10 och PDCA-översikt.

---

## 5. Produktstyrning 2026-10-26 (Master Källor + Bilagor)

Källor integrerade i `source-briefs/`:

- `Master_Kallor_och_Bilagor_Paket.md` – komplett källpaket och laganalys.
- `Standard_References_Index.md` – centralt nav (>70 dokument).
- `MASTER_KALLOR_SOURCE_BRIEF.md` – användningsregler för produktutveckling.

Bilagor A–E (kravmatris, produktkoncept, säljmaterial, utveckling/lansering, risker/compliance) styr funktioner mot ISO 9001/14001/45001/27001, AFS 2023:1, SOSFS 2011:9 och klimatändringar 2024.

Beslut: Ska användas som styrunderlag. Äldre AFS 2001:1 och OHSAS märks outdated.  
Nästa: Förädla prioriterade delar till MVP-moduler enligt Bilaga A och D.
