# SOURCE_REGISTRY

Register över original. Inte filinnehåll.

**Uppdaterad:** 2026-10-26  
**Regel:** SHA-256 beräknas där originalfilen finns lokalt. Saknas filen i denna miljö = `sha256` tom, `status` = `saknas_här`.

## Premium-källor (onboarding + projektplan)

| source_id | filnamn | typ | sha256 | sekretess | beslut | status |
|-----------|---------|-----|--------|-----------|--------|--------|
| src-intro-nyanstalld-pdf-2026 | Introduktion_for_nyanstalld_2026_Premium.pdf | Original / Handbok | | intern / kommersiell | Ska användas (onboarding) | saknas_här |
| src-intro-nyanstalld-docx-2026 | Introduktion_for_nyanstalld_2026_Premium.docx | Originalmall | | intern / kommersiell | Ska användas (onboarding) | saknas_här |
| src-projektplan-impl-docx-2026 | Projektplan_ISO_9001_14001_Implementation_2026_Premium.docx | Originalmall | | intern / kommersiell | Ska användas (implementering) | saknas_här |
| src-projektplan-9001-14001-docx-2026 | Projektplan_ISO_9001_14001_2026_Premium.docx | Originalmall | | intern / kommersiell | Kräver manuell granskning / ev. dubblett mot Implementation | saknas_här |

Fält att fylla när filen finns: `sha256`, `size_bytes`, `lagringsplats`.

## Batchar (inte uppackad kunskap förrän Steg 2)

| source_id | batch | typ | beslut |
|-----------|-------|-----|--------|
| batch-kb-complete-2026-07-12 | QualityWorX_KnowledgeBase_Complete_2026-07-12.zip | Arkiv | Register only |
| batch-onboarding-2026-07-25 | QualityWorks_Onboarding_Knowledge_2026-07-25.zip | Arkiv | Register only |
| batch-onboarding-2026-07-26 | QualityWorks_Onboarding_Knowledge_Complete_2026-07-26.zip | Arkiv | Register only |
| batch-kma-ucp-2026-07-12 | QualityWorX_KMA_UCP_KnowledgeBase_2026-07-12.zip | Arkiv | Register only |
| batch-amp-2026-09-04 | KMA_Bygg_AMP_Paket_2026-09-04.zip | Arkiv / förädlad MD finns separat | Ska användas efter Steg 2-filter |
| batch-fragobank-v2 | Fragobank_v2/ | Produktmallar | Manuell / delvis outdated klausul-språk |
| batch-saas-2026-07-12 | Saas_Final_Paket_2026-07-12/ | Arkiv | Register only |
| batch-saas-iso-2026-07-17 | SaaS_ISO_Paket_2026-07-17/ | Arkiv | Register only |
| batch-standarder | Standarder/ | Standard (SIS) | Ej i git |

## Produktstyrning 2026-10-26 (Master Källor + Index)

| source_id | filnamn | typ | sha256 | sekretess | beslut | status |
|-----------|---------|-----|--------|-----------|--------|--------|
| src-master-kallor-bilagor-2026-05-11 | Master_Kallor_och_Bilagor_Paket.md | Index / AI-underlag | | intern | Ska användas | finns_i_source-briefs |
| src-standard-references-index-2026-05-11 | Standard_References_Index.md | Index / Central referens | | intern | Ska användas | finns_i_source-briefs |
| src-bilaga-a-produktkravsmatris-2026-10-26 | Bilaga_A_Produktkravsmatris.docx | Produktstyrning | | intern | Ska användas | finns_lokalt |
| src-bilaga-b-produktkoncept-2026-10-26 | Bilaga_B_Produktkoncept.docx | Produktstyrning | | intern | Ska användas | finns_lokalt |
| src-bilaga-c-saljmaterial-2026-10-26 | Bilaga_C_Saljmaterial.docx | Produktstyrning | | intern | Ska användas | finns_lokalt |
| src-bilaga-d-utveckling-lansering-2026-10-26 | Bilaga_D_Utveckling_Lansering.docx | Produktstyrning | | intern | Ska användas | finns_lokalt |
| src-bilaga-e-risker-compliance-2026-10-26 | Bilaga_E_Risker_Compliance.docx | Produktstyrning | | intern | Ska användas | finns_lokalt |

Källbrief: `source-briefs/MASTER_KALLOR_SOURCE_BRIEF.md`  
Bilagorna styr produktfunktioner mot ISO/AFS. AFS 2001:1 i index är föråldrad – mappa till AFS 2023:1.

## Bearbetade moduler från Premium-onboarding

Se `processed/hr-onboarding/` och `processed/arbetsmiljo/`.  
Källkoppling: `src-intro-nyanstalld-pdf-2026` / `src-intro-nyanstalld-docx-2026`.

`arbetsmiljo_sakerhet.md` ska inte användas som SAM-kravkälla (AFS 2001:1). Se `registry/OUTDATED_CONTENT.md`.
