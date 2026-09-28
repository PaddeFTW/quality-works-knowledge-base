# Quality Works Knowledge Base

Professionell kunskapsbank som Quality Works-appar hämtar från.

Detta paket bygger inte appar. Det samlar förädlad Markdown från projektet.

**Paketdatum:** 2026-09-28  
**Språk i apptext:** Enkelt svenska (krav/avsnitt, inte klausul).

## Appar som hämtar härifrån

- Quality Works Light
- Quality Works Small
- QW Web / ISO Quiz
- Miljöutredning
- Egenkontroll
- Arbetsmiljöplan / skyddsrond / riskbedömning
- Dokumentgeneratorer, onboarding, revision, checklistor

## Struktur

```
quality-works-knowledge-base/
├── README.md
├── originals/
│   ├── README.md
│   └── registry/
│       └── SOURCE_REGISTRY.md
├── processed/
│   ├── reports/
│   ├── hr-onboarding/
│   ├── arbetsmiljo/
│   ├── forbattring/
│   ├── ledning/
│   ├── implementering/
│   ├── miljo/
│   └── kb/
├── products/
│   ├── _templates/
│   └── introduktion-nyanstalld/
├── standards/
├── source-briefs/
└── registry/
```

## Vad som ligger var

| Mapp | Innehåll |
|------|----------|
| `originals/registry/` | Register över källor. Originalfiler ligger kvar i projektmappen och kopieras inte hit. |
| `processed/reports/` | Steg 1-rapporter: ANALYSIS_REPORT, CONTENT_INDEX, METADATA, DOCUMENT_CLASSIFICATION, DUPLICATES, OUTDATED_CONTENT, MANUAL_REVIEW |
| `processed/hr-onboarding/` | Onboarding-moduler (HR) |
| `processed/arbetsmiljo/` | SAM-relaterat + AMP-paket 2026-09-04 (Markdown) |
| `processed/forbattring/` | Förbättringsverksamhet |
| `processed/ledning/` | Ledningssystem, KMA-översikt, UCP |
| `processed/implementering/` | ISO-projektplan och plattformsunderlag |
| `processed/miljo/` | Miljöplan-moduler 2026-08-19 |
| `processed/kb/` | MVP-moduler 2026-09-17 (ISO 9001:2026 / 14001, frågebank ägare) |
| `products/_templates/` | Fragobank_v2 produktpaket 00–21 |
| `products/introduktion-nyanstalld/` | Samma HR-onboarding som produktvy |
| `standards/` | Katalog/index över ISO-källor (inte standard-PDF) |
| `source-briefs/` | Korta källkopplingar |
| `registry/` | Paketregister |

## Hårda regler

- Originalfiler ändras inte.
- Upphovsrättsskyddad standardtext kopieras inte verbatim.
- ISO-PDF ligger i `artifacts/Standarder/` (SIS-licens), inte i detta paket.
- Föråldrat material är märkt i `processed/reports/OUTDATED_CONTENT.md`.
- `arbetsmiljo_sakerhet.md` ska inte användas som SAM-kravkälla (AFS 2001:1).

## MVP som fortfarande saknas

kb-iso-9001-krav, kb-iso-14001-krav, kb-iso-45001-krav, kb-iso-27001-krav, kb-fragobank (kanon), kb-skyddsrond, kb-riskbedomning, kb-miljoaspekter-kemikalier, kb-laglista-efterlevnad, kb-internrevision-gap, kb-ledningens-genomgang.

Delar täcks av AMP-paketet och miljöplan-MD utan MVP-id.
