# Guided Workflow Engine – produktprinciper

**Källa:** `PaddeFTW/app-template` → `docs/QUALITY_WORX_PRODUCT_PRINCIPLES.md` (v2.0)  
**Datum analys:** 2026-08-30  
**Typ:** Process / AI-underlag / Produktprincip  
**Avgränsning:** Principdokument. Implementerar inte en motor och innehåller inga ISO-krav.

---

## Grundbeslut

A = digitalt dokument/formulär  
B = guidad arbetsupplevelse  

**Rekommendation enligt källan: B.**

Dokument, formulär och tabeller får finnas, men de ska stödja arbetet – inte vara huvudupplevelsen.

Plattformsbegrepp: **Guided Workflow Engine**.  
Använd inte “Quiz Engine” som plattformsbegrepp. En quiz-liknande vy kan vara ett UI-mönster inuti motorn.

En Guided Workflow Engine omfattar enligt källan:

- arbetssteg
- frågor
- beslut
- hjälptexter
- branschbegrepp
- villkorad logik
- progressive disclosure
- dokumentgenerering i bakgrunden
- anpassning före start
- återanvändbara mönster mellan appar

---

## De 15 produktprinciperna (sammanfattade från källan)

1. **Digitalisera kunskap, inte dokument** – fråga vilken bedömning, vilket beslut eller vilken åtgärd som stöds.
2. **Originaldokument är kunskapskälla, inte UI-specifikation** – mallar styr inte UI rad för rad.
3. **Guided Workflow före formulär** – hjälp användaren fram till rätt svar.
4. **Dokument skapas i bakgrunden** – dokumentet är ett resultat av arbetet.
5. **Minsta möjliga skrivande** – val, korta beslut, standardvärden, fritext bara vid behov.
6. **Intelligent frågebank / arbetsstegsbank** – återanvändbara byggblock: fråga, beslut, förklaring, villkor, kategori, rekommendation, dokumenteffekt.
7. **Progressive Disclosure** – visa bara det som behövs nu.
8. **Positive Productivity** – hjälp, inte kontroll. Stödjande ton.
9. **Mobil först** – fullt användbart nära arbetet.
10. **Vardagssvenska och branschspråk** – konkret och professionellt.
11. **Produktupplevelse är lika viktig som funktion**
12. **Återanvändbar Guided Workflow Engine** – inte engångslösningar per app.
13. **Anpassning före start** – projekttyp, verksamhet, roll, omfattning, risknivå.
14. **En fråga/ett beslut i taget när det passar** – inte alltid, utan när det stödjer beslutet.
15. **Översikt/tabell endast där det ger tydligt värde**

---

## Tillämpning per produkttyp (enligt källan)

| Produkttyp | Fokus enligt principerna | Får inte bli |
|------------|--------------------------|--------------|
| Egenkontroll | Kontroller, avvikelser, åtgärder steg för steg | Mall att kopiera till andra produkter |
| Riskbedömning | Identifiera risk, konsekvens, sannolikhet, åtgärd | Kopia av egenkontroll |
| Skyddsrond | Observation, plats, åtgärdsbehov, ansvar (mobil) | Egenkontrollens struktur |
| Kontrollplan | Planering, ansvar, kontrollpunkter, spårbarhet | Checklista från egenkontroll |
| Arbetsmiljöplan | Anpassning före start, roller, planeringsbeslut | Egenkontroll-kopia |
| Miljöplan | Aspekter, krav, åtgärder i rätt ordning | Egenkontrollens kontrollflöde |
| Revision | Intervjuer, observationer, bevis, sammanfattning | Egenkontroll-kopia |

---

## Icke-mål i källan

Dokumentet skapar inte appimplementation, databasmodell, API, Egenkontroll-arkitektur eller färdiga workflow-komponenter. Det är ett styrdokument för produktbeslut.
