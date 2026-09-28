---
id: kb-fragobank-27001-agare
title: Informationsägare ISO 27001 (SME)
apps: [qw-web, quiz, internrevision]
domain: infosakerhet
audience: [vd, admin, kvalitetsansvarig, revisor]
source_files: [Fragobank_v2/templates/fragobank/04_ISO27001_Fragobank.md, Standarder/ISO 27001/ISO 27001 kravrubriker 2022.txt]
law_refs: [GDPR]
iso_refs: [ISO 27001:2022 avsnitt Kontext till Förbättring, Annex A]
updated: 2026-09-17
relevance: 9
aktualitet: 8
decision: ska_anvandas
simple_level: true
feeds_questions: [Q27-4.3, Q27-5.2, Q27-5.3, Q27-6.1.2, Q27-6.1.3, Q27-7.2, Q27-A.5, Q27-A.8, Q27-9.2]
evidence_type: [policy, tillgangsregister, soa, anvandarregister, backuptest, incidentlogg, avtal]
chunk_max_words: 700
status: current
---

# Informationsägare ISO 27001

I företag under 50 anställda finns sällan en säkerhetschef. VD äger beslutet. Den som sköter Microsoft 365, ekonomi eller webbhotellet äger detaljerna.

| Område | VD själv? | Typisk ägare | Var informationen finns | Hur quizet hjälper | Bevis vid revision |
|--------|-----------|--------------|-------------------------|--------------------|--------------------|
| ISMS-omfattning | Ja | VD | Lista system och platser | Vilka system: mejl, ekonomi, kundregister, byggprojekt | Skriven omfattning |
| Intressenter info | Delvis | VD + sälj | Kundavtal, personuppgiftsbiträde | Kunder, anställda, IT-leverantör, myndighet | Intressentlista |
| Policy och roller | Ja | VD | Policy, rollista | Namnge systemägare för mejl, ekonomi och projektfiler | Policy + roller |
| Tillgångar | Nej | Admin / IT-leverantör | Inventarielista, systemlista | Lista datorer, mobiler, molntjänster, pärmar | Tillgångsregister |
| Riskmetod och risker | Delvis | VD + admin | Risklista | Stöld av dator, felaktigt mejl, ransomeware, slarvig USB | Riskbedömning |
| SoA / valda åtgärder | Nej | Kvalitetsansvarig / konsult | SoA-mall | Quiz ska inte kräva 93 kontroller utantill. Visa vilka som gäller | SoA |
| Utbildning info | Nej | Admin | Introduktion, phishing-övning | Senaste genomgång lösenord och mejl | Kvittens |
| Åtkomst och avslut | Nej | Admin / IT-leverantör | Användarlista | Vad händer när någon slutar? | Kontolista + avslutsrutin |
| Backup och radering | Nej | IT-leverantör / admin | Backuprapport | Senaste återställningstest | Testprotokoll |
| Incidenter | Nej | Admin / VD | Incidentlogg, IMY-anmälan | Senaste dataincident, även “nästan” | Incidentrapport |
| Leverantörssäkerhet | Delvis | VD / inköp | Avtal, biträdesavtal | Moln, lönesystem, support | Avtal med säkerhetskrav |
| GDPR-register | Nej | Admin | Behandlingsregister | Personuppgifter kunder och personal | Register + laglig grund |
| Mätning | Nej | Admin | Loggar, ärendelista | Antal incidenter, misslyckade inloggningar | KPI |
| Internrevision ISMS | Delvis | Internrevisor / konsult | Protokoll | Stickprov: ett konto, en backup, ett avtal | Revisionsprotokoll |
| Ledningens genomgång | Ja | VD | Protokoll | Ta upp incidenter och leverantörer | Beslut i protokoll |

**Quizregel:** Ja på åtkomst, backup och SoA kräver utdrag från system eller leverantör – inte VD:s försäkran. I 1–10 personer är VD ofta samma som admin; quizet ska ändå kräva underlag.
