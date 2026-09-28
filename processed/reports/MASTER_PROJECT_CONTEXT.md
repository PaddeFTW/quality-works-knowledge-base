# ISO Quiz – Master Project Context

**Fil:** `MASTER_PROJECT_CONTEXT.md`  
**Uppdaterad:** 2026-09-19  
**Roll i Grok-projektet:** Produkt- och projektkontext för ISO Quiz. Kunskapsbanken (denna mapp) matar apparna. Den här filen beskriver vad ISO Quiz är och vad version 1 ska göra – inte ny ISO-kravtext.

---

## Projektöversikt

ISO Quiz är inte ett traditionellt quizverktyg.

Målet är inte att testa ISO-kunskap.

Målet är att hjälpa små och medelstora företag att bygga ett verkligt ledningssystem genom att besvara frågor om sin verksamhet.

Användaren ska kunna:

1. Skapa konto
2. Skapa företag
3. Besvara frågor
4. Beskriva hur verksamheten fungerar idag
5. Se vad som saknas
6. Få konkreta åtgärder
7. Skapa dokument
8. Bygga ett ledningssystem
9. Förbereda sig inför certifiering

---

## Målgrupp

Primär målgrupp:

- Små företag
- Medelstora företag
- 2–50 anställda

Typiska kunder:

- Byggföretag
- Transportföretag
- Konsultföretag
- Tillverkande företag
- Serviceföretag

De flesta kunder:

- Har liten kunskap om ISO
- Vill komma igång snabbt
- Vill inte läsa standardtexter
- Vill veta exakt vad som saknas

---

## ISO-standarder

Version 1 fokuserar på:

- ISO 9001
- ISO 14001
- ISO 45001

Senare kan fler standarder läggas till.

---

## Produktfilosofi

Användaren ska aldrig känna:

> Jag svarar på frågor utan anledning.

Varje svar ska användas för att:

- Förstå verksamheten
- Skapa dokument
- Identifiera brister
- Skapa åtgärder
- Skapa ledningssystem

Slutresultatet ska kännas som:

> Nu förstår jag vad vi har, vad vi saknar och vad vi behöver göra.

Inte:

> Jag fick 73 % på ett quiz.

---

## Nuvarande funktionalitet

Applikationen innehåller redan:

- 38 frågor
- ISO 9001
- ISO 14001
- ISO 45001
- Sparade svar
- Framstegsspårning
- Sektioner
- Guidance-texter
- Smart Workspace
- Anteckningar
- Uppgifter
- Sammanfattning
- DOCX-export
- PDF-export
- Supabase-integration

Projektet börjar **inte** från noll.

---

## Största problemet vi löser

Små företag vet ofta inte:

- Var de ska börja
- Vad som saknas
- Vilka dokument som krävs
- Vem som borde svara på vissa frågor

ISO Quiz ska guida användaren hela vägen.

---

## Unik funktion

För varje fråga ska systemet kunna visa vem som vanligtvis har informationen.

**Exempel**

Fråga: Hur hanterar ni kundklagomål?

Vanligtvis vet:

- VD
- Kundansvarig
- Administration

Fråga: Hur genomför ni medarbetarsamtal?

Vanligtvis vet:

- VD
- HR
- Arbetsledare

Det hjälper små företag att samla rätt information.

Fältkälla i kunskapsbanken: `Fragobank_v2/templates/fragobank/21_Information_och_Bevis.md`  
(`vd_kan_svara_direkt`, `information_finns_hos`, `var_informationen_finns`, `vanliga_bevis`)

---

## Statusöversikt

Använd inte konsultord som:

- Gap Analysis
- Compliance Score

Visa istället:

- Vad fungerar bra
- Vad behöver förbättras
- Vad saknas
- Vad behöver göras

**Exempel**

- Kompetensmatris finns
- Kundundersökningar saknas
- Internrevision saknas
- Avvikelsehantering finns

---

## Åtgärdsplan

Systemet ska automatiskt kunna skapa:

- Att-göra-punkter
- Ansvariga personer
- Prioritet
- Förfallodatum

**Exempel**

- Titel: Genomför kundundersökning
- Ansvarig: VD
- Prioritet: Hög
- Status: Ej påbörjad

---

## Dokumentgenerator

Version 1 ska kunna skapa:

- Ledningssystem
- Kvalitetspolicy
- Miljöpolicy
- Arbetsmiljöpolicy
- Mål och handlingsplan
- Riskregister
- Förbättringsregister
- Processöversikt
- Dokumentförteckning

Dokument ska kunna exporteras till:

- DOCX
- PDF

---

## Version 1 Roadmap

### Fas 1 – Authentication & Company Setup

Implementera:

- Registrering
- Inloggning
- Utloggning
- Glömt lösenord
- Session persistence
- Skyddade sidor

Databas:

- profiles
- organizations
- organization_members

Roller:

- Owner
- Manager
- Employee

Första användarflöde:

1. Skapa konto
2. Verifiera email
3. Skapa företag
4. Bli Owner
5. Kom till dashboard

### Fas 2 – Question Management

Flytta frågorna från kod till databas.

Lägg till:

- Ja/Nej
- Flerval
- Betygsskala
- Datum
- Nummer
- Bilagor

### Fas 3 – ISO Status Overview

Visa:

- Beredskapsgrad
- Vad som saknas
- Vad som fungerar
- Öppna åtgärder
- Försenade åtgärder

### Fas 4 – Action Plans

Automatiska uppgifter. Ansvariga. Prioritet. Status.

### Fas 5 – Document Generation

Bygg dokument från användarens svar.

### Fas 6 – Dashboard

Dashboard ska svara på: Vad ska jag göra härnäst?

### Fas 7 – Subscription Model

Lägg till först när övriga funktioner fungerar.

---

## Får inte prioriteras nu

Bygg inte:

- AI-genererade svar
- Enterprise-funktioner
- Avancerad statistik
- Mobilappar
- Komplex certifieringslogik
- Audit portals

**Fokus just nu:** Authentication + Company Setup

---

## Slutmål

ISO Quiz ska hjälpa små företag att gå från:

> Vi vet inte vad ISO kräver.

Till:

> Vi vet vad som saknas, vem som ansvarar för det och vi har dokumenten som behövs för att arbeta vidare mot certifiering.

---

## Produktpaket 00–21

Kanonisk plats: `Fragobank_v2/templates/fragobank/`. Grok läser härifrån. Inga nya ISO-krav.

| Fil | Roll |
|-----|------|
| `00_Gemensam_Metod.md` | Ja / Delvis / Nej |
| `00_Vad_betyder_orden.md` | Enkla ord |
| `01`–`04` | Kravbank per standard + beviskolumn |
| `06_Kort_Quiz_Per_Standard.md` | 5 startfrågor per standard |
| `07_Branscher.md` | Branschfilter och exempel |
| `08_Foretagsstorlek.md` | Språk efter 1–5 / 6–20 / 21–50 |
| `09_Manualgenerator_Regler.md` | Svar → manualtext |
| `10_Bred_Fragobank_Alla_Standarder.md` | A1–G3 (37 frågor) |
| `11_Quiz_Falt_Mall.md` | Fält i appen |
| `12_Quiz_Arkitektur.md` | Flöde företag → quiz → export |
| `13_Question_JSON_Schema.md` | Frågeschema |
| `14_Grok_Arbetsinstruktion.md` | Vad Grok får / inte får |
| `15_Produktvision.md` | Vision |
| `16_MVP_Roadmap.md` | Vad som ingår i version 1 |
| `17_Inloggning_och_Foretagskonto.md` | Konto och projekt |
| `18_Fragebanksstrategi.md` | Filter standard / bransch / storlek |
| `19_Exportkrav.md` | DOCX och PDF |
| `20_Grok_Workflow.md` | KB → fråga → manual |
| `21_Information_och_Bevis.md` | Vem som vet, var, bevis per fråga |

Informationshjälp hämtas bara från `21`. Schemafält enligt `13` + de fyra fälten i `21`.
