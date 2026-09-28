---
id: amp-revision-version
title: Versionering, revision och intern uppföljning
typ: rutin
version: 1.0.0
datum: 2026-09-04
sprak: sv
regelverk: [AFS 2023:1, AFS 2023:3, ISO 45001 9, ISO 9001 7.5]
---

# Versionering

| Fält | Regel |
|------|-------|
| utgava | Löpnummer 01, 02, 03 … |
| version | valfritt semver för app |
| status | utkast / granskning / godkand / gallande / arkiverad |
| giltig_from | datum då utgåvan ersätter föregående |

Endast en `gallande` AMP per projekt.

## När ny utgåva krävs

- Ny särskild risk eller nytt moment för befintlig risk
- Ny BAS-P, BAS-U eller byggherre
- Väsentlig tidplansändring eller ny UE med egna risker
- Allvarlig avvikelse / olycka som ändrar åtgärder
- Skyddsrond visar att beskriven åtgärd inte fungerar

## Revisionshistorik

| Utgåva | Datum | Orsak | Författare | Godkänd av |
|--------|-------|-------|------------|------------|
| {{utgava}} | {{datum}} | Första gällande / ändring | {{upprattad_av}} | {{bas_u}} |
| | | | | |

## Intern revision – checklista bygg-AMP

Använd vid intern revision eller KMA-uppföljning.

| Nr | Fråga | Ja | Nej | Avvikelse |
|----|-------|----|-----|-----------|
| 1 | Finns utsedd BAS-P och BAS-U dokumenterat? | ☐ | ☐ | |
| 2 | Krävs AMP – och finns den gällande på plats? | ☐ | ☐ | |
| 3 | Är de 13 riskerna bedömda med ja/nej? | ☐ | ☐ | |
| 4 | Har varje ja-risk konkret åtgärd per moment? | ☐ | ☐ | |
| 5 | Är förhandsanmälan gjord och anslagen om den krävs? | ☐ | ☐ | |
| 6 | Introduceras personal och UE innan arbete? | ☐ | ☐ | |
| 7 | Genomförs skyddsronder enligt intervall? | ☐ | ☐ | |
| 8 | Stängs åtgärder med datum och ansvar? | ☐ | ☐ | |
| 9 | Anmäls allvarliga händelser enligt rutin? | ☐ | ☐ | |
| 10 | Stämmer organisation och UE-lista med verkligheten? | ☐ | ☐ | |

Avvikelser går till handlingsplan i `03_risk/riskbedomning.md`.

## Koppling ISO / SAM

| Kravområde | Standard / föreskrift | Evidens i paketet |
|------------|----------------------|-------------------|
| Roller och ansvar | ISO 45001 5.3 · AFS 2023:3 | organisationsfiler |
| Kompetens och medvetenhet | ISO 45001 7.2–7.3 | kvittering, behörighet |
| Dokumenterad information | ISO 45001 7.5 · AFS 2023:3 kap. 11 | AMP + versioner |
| Beredskap | ISO 45001 8.2 | nödläge |
| Uppföljning | ISO 45001 9.1 · AFS 2023:1 | rond + revision |
| Förbättring | ISO 45001 10 | åtgärd efter avvikelse |
