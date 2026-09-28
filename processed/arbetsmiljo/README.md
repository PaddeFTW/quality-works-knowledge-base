---
id: kma-bygg-amp-paket-2026
title: Arbetsmiljöplan, riskbedömning och skyddsrond – kunskaps paket för bygg
typ: paketindex
sprak: sv
version: 1.0.0
datum: 2026-09-04
status: publicerad
malgrupp: [BAS-P, BAS-U, platschef, KMA, skyddsombud, Quality WorX Apps]
regelverk: [AML, AFS 2023:1, AFS 2023:3, AFS 2023:10, AFS 2023:13, AFS 2025:6, ISO 45001]
kallor_analyserade:
  - Arbetsmiljoplan för bygg - Avancerad mall för större projekt.docx
  - Riskbedömning - Arbetsmiljö - Avancerad (Bygg 2026).docx
  - Risker inför byggstart 2026.docx
  - Skyddsrond.docx
  - Master_Kallor_och_Bilagor_Paket.md
  - Standard_References_Index.md
beslut: ska_anvandas
---

# README – KMA bygg AMP-paket 2026

Kunskapspaket för Quality WorX Knowledge Base.  
Originalmallar är analyserade, inte kopierade. Texterna är nyskrivna, fältbaserade mallar med samma eller högre täckning.

Paketet är avsett för RAG, Guided Workflow Engine, dokumentgenerator och formulär – inte som färdig appkod.

## Filträd

```text
kma_bygg_amp_paket_2026/
├── README.md
├── ANALYSIS_REPORT_AMP_Paket_2026-09-04.md
├── _schema/
│   ├── faltkatalog.md
│   ├── platshallare.md
│   └── app_dataflode.md
├── 01_amp/
│   ├── amp_huvuddokument.md
│   ├── forhandsanmalan.md
│   └── arbetsberedning.md
├── 02_organisation/
│   ├── roller_bas_p_bas_u.md
│   └── projektorganisation.md
├── 03_risk/
│   ├── riskbedomning.md
│   └── riskmatris_atgardstrappa.md
├── 04_sarskilda_risker/
│   └── de_13_sarskilda_riskerna.md
├── 05_skyddsrond/
│   └── skyddsrond_bygg.md
├── 06_regler_beredskap/
│   ├── ordnings_skyddsregler.md
│   ├── nodlage_olycka.md
│   └── sdb_kemikalier.md
└── 07_uppfoljning/
    ├── kvittering_godkannande.md
    └── revision_version.md
```

## Vad paketet täcker

| Område | Fil | App-användning |
|--------|-----|----------------|
| AMP enligt AFS 2023:3 kap. 11 | `01_amp/amp_huvuddokument.md` | Skapa/redigera arbetsmiljöplan |
| Förhandsanmälan | `01_amp/forhandsanmalan.md` | Villkorat formulär + export |
| Arbetsberedning | `01_amp/arbetsberedning.md` | Steg före riskmoment |
| BAS-P / BAS-U / roller | `02_organisation/roller_bas_p_bas_u.md` | Rollväljare, ansvarskedja |
| Organisation, UE, yrkesarbetare | `02_organisation/projektorganisation.md` | Kontaktlistor, ID06, behörighet |
| Riskbedömning + handlingsplan | `03_risk/riskbedomning.md` | Formulär med status/deadline |
| 5×5-matris + åtgärdstrappa | `03_risk/riskmatris_atgardstrappa.md` | Beräkna residualrisk |
| 13 arbeten med särskild risk | `04_sarskilda_risker/de_13_sarskilda_riskerna.md` | Ja/nej-checklista + åtgärd per risk |
| Skyddsrond protokoll + byggchecklista | `05_skyddsrond/skyddsrond_bygg.md` | Rundaprotokoll, anmärkning, uppföljning |
| Ordnings- och skyddsregler | `06_regler_beredskap/ordnings_skyddsregler.md` | Introduktion + kvittering |
| Nödläge / olycka / anmälan | `06_regler_beredskap/nodlage_olycka.md` | Krissteg, kontaktfält |
| SDB-register | `06_regler_beredskap/sdb_kemikalier.md` | Kemikalielista på plats |
| Signatur, distribution | `07_uppfoljning/kvittering_godkannande.md` | Signaturflöde |
| Version och revision | `07_uppfoljning/revision_version.md` | Revisionshistorik |

## Dataflöde i appen

1. **Starta projekt** – fyll `{{projekt}}`, `{{plats}}`, byggherre, entreprenadform, period.
2. **Utses roller** – BAS-P, BAS-U, platschef, skyddsombud (`roller_bas_p_bas_u.md`).
3. **Bedöm om AMP krävs** – särskild risk enligt 11 kap. 12 § **eller** tröskel för förhandsanmälan.
4. **Förhandsanmälan** – om tröskel uppfylls; kopia anslås på plats.
5. **Identifiera de 13 riskerna** – ja/nej + åtgärd + ansvar + deadline.
6. **Riskbedömning 5×5** – sannolikhet × konsekvens, åtgärdstrappa, residualrisk.
7. **Skriv AMP** – organisation, regler, samordning, åtgärder för särskilda risker.
8. **Arbetsberedning** – före varje moment med särskild risk.
9. **Kvittering** – medarbetare och UE tar del av AMP + regler.
10. **Skyddsronder** – löpande, anmärkning → handlingsplan → stängd.
11. **Uppdatera AMP** – vid förändring, ny UE, ny metod, nytt skede.
12. **Revision** – intern kontroll mot AFS 2023:1 och 2023:3.

Dokument (PDF/utskrift) genereras i bakgrunden från ifyllda fält. UI ska vara guided workflow, inte en 24-sidig blankett.

## Relaterade moduler i kunskapsbanken

- `projektorganisation_bygg.md`
- `byggparm_kma_struktur.md` (flik 7 AMP, 21 skyddsrond, 28 riskbedömning)
- `arbetsmiljo_sakerhet.md`
- `ordnings_skotselregler.md`
- `nodlagesberedskap_miljo.md`
- `kemikaliehantering_bygg.md`
- `guided_workflow_engine.md`

## Regler för användning

- Originalfiler får inte ändras eller återpubliceras verbatim.
- Hitta inte på lagkrav. Hänvisa till AFS-nummer och låt jurist/BAS verifiera aktuell lydelse.
- Källmallarna blandar AFS-nummer. Detta paket använder officiell uppdelning:
  - **AFS 2023:1** systematiskt arbetsmiljöarbete
  - **AFS 2023:3** projektering och byggarbetsmiljösamordning (AMP, BAS, förhandsanmälan, 13 risker)
  - **AFS 2023:10** risker i arbetsmiljön (fall, ras, kemikalier, buller m.m.)
  - **AFS 2023:13** risker vid vissa typer av arbeten (byggkapitel + asbest m.m.)
  - **AFS 2025:6 / 2025:8** ändringar asbest i AFS 2023:13 (gäller från 2025-12-19)
- Mallarna är kommersiella underlag, inte juridisk rådgivning.

## Betyg på källbatchen

| Källa | Relevans | Kvalitet | Aktualitet | AI-värde | Digitalisering | Återanvändbarhet | Beslut |
|-------|----------|----------|------------|----------|----------------|------------------|--------|
| AMP bygg större projekt | 10 | 8 | 8 | 10 | 10 | 9 | ✅ Använd struktur |
| Riskbedömning bygg 2026 | 10 | 7 | 8 | 10 | 10 | 9 | ✅ Använd + rätta AFS-hänvisningar |
| Risker inför byggstart | 9 | 7 | 8 | 9 | 10 | 9 | ✅ Använd |
| Skyddsrond | 8 | 7 | 7 | 9 | 10 | 8 | ✅ Använd, bygg-anpassa |
