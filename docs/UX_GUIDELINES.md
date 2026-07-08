# UX_GUIDELINES

## Syfte

Detta dokument definierar användarupplevelsen för **Egenkontroll App**.

Riktlinjerna utgår från tidigare kunskapsdokument och KvalitetsDokument.se:s originalmaterial. Originalmaterialet visar en tydlig arbetslogik: välj dokument, fyll i rätt uppgifter, kontrollera moment, markera resultat, skriv kommentar vid brist, signera, granska och skapa rapport.

Appens uppgift är att göra den arbetslogiken enkel, trygg och användbar i vardagen för små och medelstora byggföretag.

## UX-Vision

Egenkontroll App ska kännas som en erfaren arbetsledare som står bredvid användaren och säger:

- vad som ska göras nu
- varför det behövs
- vad som kan vänta
- vad som saknas
- vad som bör kontrolleras innan nästa steg

Appen ska inte kännas som:

- en digital Word-blankett
- ett tungt verksamhetssystem
- ett myndighetsformulär
- en ISO-manual
- ett avancerat dokumenthanteringssystem

## Målgrupp

Appen byggs för användare som ofta har mer byggvana än systemvana.

Primära användare:

- små byggföretag
- medelstora byggföretag
- entreprenörer
- underentreprenörer
- platschefer
- arbetsledare
- yrkesarbetare
- kvalitetsansvariga
- kontrollansvariga eller granskare

Många användare kan vara:

- stressade
- ute på arbetsplatsen
- på mobil eller surfplatta
- ovana vid digitala system
- osäkra på byggadministrativa begrepp
- mer intresserade av att bli klara än att läsa instruktioner

## Grundprinciper

### Appen Leder Användaren

Användaren ska aldrig behöva gissa nästa steg.

Appen ska hela tiden visa:

- var användaren är
- vad som ska göras nu
- vad som är klart
- vad som saknas
- hur användaren går vidare

Bra upplevelse:

```text
Välj mall
→ Fyll i projektinformation
→ Anpassa kontrollpunkter
→ Starta kontroll
→ Granska sammanställning
→ Signera
→ Slutför
```

Dålig upplevelse:

```text
Visa alla fält, alla inställningar och alla val på samma sida.
```

### Ett Beslut I Taget

Varje steg ska ha ett tydligt huvudbeslut.

Exempel:

- På mallsteget väljer användaren mall.
- På projektsteget fyller användaren projektuppgifter.
- På anpassningssteget justerar användaren kontrollpunkter.
- På kontrollsteget bedömer användaren en punkt i taget eller en tydlig grupp.
- På slutförandesteget tar användaren ställning till om dokumentationen är klar.

Undvik att blanda flera beslut:

- välj mall
- skapa projekt
- ändra kontrollpunkter
- signera
- exportera

på samma yta.

### Progressive Disclosure

Visa det viktigaste först. Visa mer när användaren behöver det.

Första nivån ska visa:

- huvudhandling
- nödvändiga fält
- aktuell status
- nästa steg

Andra nivån kan visa:

- hjälptext
- exempel
- avancerade val
- detaljer om referenser
- bilagor
- foton
- åtgärder

Användaren ska kunna göra en enkel egenkontroll utan att möta alla möjliga funktioner på en gång.

### Smarta Standardvärden

Appen ska minska onödigt arbete, men aldrig gissa ansvar eller resultat.

Bra standardvärden:

- ny egenkontroll startar som Utkast
- kontrollpunkter startar som Ej bedömd
- dagens datum föreslås
- aktuell användare föreslås som kontrollant om det finns inloggning
- vald mall kopieras till egenkontrollen
- kommentar öppnas automatiskt vid Ej godkänd
- kommentar öppnas automatiskt vid Ej kontrollerad
- exportnamn föreslås från egenkontrollens namn och datum

Undvik standardvärden som:

- markerar punkter som Godkänd automatiskt
- signerar automatiskt
- döljer ej bedömda punkter
- antar att beställare och byggherre alltid är samma sak
- fyller i juridiska standardtexter utan sakgranskning

### Exempel Före Instruktion

Oerfarna användare förstår ofta snabbare av exempel än av långa förklaringar.

Använd exempel när användaren ska skriva:

- referens
- kommentar
- åtgärd
- projektnamn
- kontrollpunkt
- övriga anteckningar

Exempel:

- "Ritning A-40.1-101, rev B"
- "Tätskikt saknas vid genomföring. Åtgärdas innan nästa moment."
- "Punkten kunde inte kontrolleras eftersom ytan var inbyggd."

Undvik långa instruktioner som försöker beskriva alla möjliga fall.

### Hjälp När Den Behövs

Hjälp ska finnas där användaren fastnar, inte som långa textsidor före arbetet.

Använd:

- tooltip för begrepp
- hjälptext vid fält
- exempel vid textfält
- varning vid risk
- checklista inför slutförande
- info-box när något måste förstås innan beslut

Hjälpen ska svara på:

- Vad betyder detta?
- Vad ska jag fylla i?
- Varför behövs det?
- Vad händer om jag går vidare?

### Minimera Osäkerhet

Osäkerhet uppstår när användaren inte vet:

- vilken mall som passar
- vad ett begrepp betyder
- hur mycket text som ska skrivas
- om något är sparat
- om kontrollen är klar
- om det går att ändra senare

Appen ska minska osäkerhet genom:

- tydliga steg
- tydliga statusar
- synlig autosparning eller sparbekräftelse
- exempel i rätt fält
- sammanställning före slutförande
- varningar för saknad information
- tydlig skillnad mellan Utkast, Pågående och Slutförd

### Minimera Fel

Appen ska förebygga vanliga misstag innan de blir problem.

Vanliga fel att förebygga:

- fel mall väljs
- kontrollen startas utan anpassning
- referenser saknas
- ej godkända punkter saknar kommentar
- ej kontrollerade punkter saknar orsak
- ej bedömda punkter slinker igenom vid slutförande
- utförare och granskare blandas ihop
- signering misstolkas som BankID eller avancerad e-signering
- användaren tror att foto ersätter kommentar

Förebygg med:

- stegvis flöde
- obligatorisk kommentar vid negativa resultat
- sammanställning
- tydliga varningar
- enkla bekräftelser
- bra standardvärden

## Huvudflöde

### 1. Start

Startsidan ska vara enkel.

Den ska hjälpa användaren att snabbt:

- skapa ny egenkontroll
- fortsätta pågående egenkontroll
- hitta slutförd egenkontroll
- öppna mallbibliotek

Startsidan ska inte vara en tung dashboard.

Visa inte för mycket statistik, administration eller framtida funktioner. Första frågan ska vara: "Vad vill du göra nu?"

### 2. Välj Mall

Mallvalet ska kännas som att välja rätt startpunkt, inte som att förstå ett system.

Varje mall bör visa:

- namn
- kort beskrivning
- typ av arbete
- antal kontrollpunkter
- möjlighet att välja tom mall

Appen ska hjälpa användaren förstå att mallen kan anpassas.

Bra hjälptext:

"Välj den mall som bäst motsvarar arbetet. Du kan ändra punkterna innan kontrollen startas."

### 3. Fyll I Projektinformation

Projektinformationen ska samla det som gör rapporten begriplig i efterhand.

Visa bara nödvändiga fält först:

- egenkontrollens namn
- projekt
- arbetsplats
- beställare / byggherre
- entreprenör
- referenser

Förklara svåra begrepp nära fältet.

Exempel:

- Beställare: den som beställt arbetet.
- Byggherre: den som låter utföra byggarbetet.

### 4. Anpassa Kontrollpunkter

Detta steg är viktigt eftersom originaldokumentens mallar är kunskapskällor, inte låsta sanningar.

Användaren ska kunna:

- läsa igenom punkterna
- ta bort sådant som inte gäller
- lägga till egna punkter
- ändra formuleringar
- ändra ordning
- gruppera punkter vid behov

Appen ska tydligt säga:

"Ändringar gäller bara denna egenkontroll. Originalmallen ändras inte."

### 5. Starta Kontroll

När kontrollen startar ska appen byta från förberedelse till genomförande.

Visa:

- egenkontrollens namn
- projekt och plats
- framsteg
- aktuell grupp eller kontrollmoment
- kontrollpunkter
- resultatval
- kommentar
- datum
- kontrollant

Det ska vara lätt att fortsätta på mobil.

### 6. Bedöm Kontrollpunkt

Varje kontrollpunkt ska vara lätt att bedöma.

Visa tydliga resultatval:

- Ej bedömd
- Godkänd
- Ej godkänd
- Ej kontrollerad

När användaren väljer **Ej godkänd**:

- öppna kommentarfält
- visa hjälptext: "Skriv vad som inte stämmer och vad som behöver göras."
- erbjud foto, bilaga eller åtgärd om relevant

När användaren väljer **Ej kontrollerad**:

- öppna kommentarfält
- visa hjälptext: "Skriv varför punkten inte har kontrollerats."

### 7. Hantera Avvikelse Och Åtgärd

Avvikelser ska inte kännas som ett separat tungt system.

De ska kännas som en naturlig följd av en punkt som inte är godkänd.

Visa enkelt:

- vad är bristen?
- vad behöver göras?
- vem ansvarar?
- är det åtgärdat?
- behövs ny kontroll?

Första versionen ska hålla detta enkelt och undvika avancerad ärendehantering.

### 8. Granska Sammanställning

Sammanställningen ska ge användaren kontroll innan signering och slutförande.

Visa:

- antal godkända
- antal ej godkända
- antal ej kontrollerade
- antal ej bedömda
- punkter som kräver kommentar
- avvikelser
- åtgärder
- övriga anteckningar
- signering
- granskning

Sammanställningen ska besvara frågan:

"Är detta tydligt nog att lämna vidare?"

### 9. Signera Och Granska

Signering ska vara enkel bekräftelse med namn och tidpunkt.

Appen ska inte antyda BankID, avancerad e-signering eller juridiskt godkännande som den inte stödjer.

Skriv tydligt:

"Signering i appen är en bekräftelse med namn och tidpunkt."

Granskning ska kännas som att en ansvarig person läser igenom och bekräftar helheten.

### 10. Slutför Och Exportera

Slutförande ska vara ett medvetet steg.

Innan slutförande ska appen visa:

- vad som är klart
- vad som saknas
- vilka punkter som kräver uppföljning
- om kommentarer saknas
- om det finns ej bedömda punkter

När egenkontrollen är slutförd ska appen bekräfta:

"Egenkontrollen är slutförd."

Exporten ska kännas som ett professionellt byggdokument, inte som en skärmdump av appen.

## Progressive Disclosure I Praktiken

### Nivå 1: Det användaren måste göra

Visa alltid:

- aktuell uppgift
- huvudknapp
- nödvändiga fält
- status
- nästa steg

### Nivå 2: Det användaren kan behöva

Visa vid behov:

- hjälptext
- exempel
- tooltip
- bilaga
- foto
- åtgärd
- mer information

### Nivå 3: Det vana användare sällan behöver

Göm bakom val eller sekundär yta:

- avancerade inställningar
- versionsinformation
- detaljerade dokumentuppgifter
- extra kommentarer
- arkivering

## Smarta Standardvärden I UX

Standardvärden ska göra användaren snabbare, inte mindre ansvarig.

### Bra UX-standarder

- Föreslå dagens datum.
- Föreslå användarens namn som kontrollant om möjligt.
- Låt kontrollpunkter börja som Ej bedömd.
- Behåll senast valt beställare/byggherre-val i samma egenkontroll.
- Visa senast öppnade pågående egenkontroller på startsidan.
- Föreslå rapportnamn från egenkontrollens namn och datum.
- Öppna rätt kommentarfält när kommentar krävs.

### UX-standarder Som Ska Undvikas

- Förifyll Godkänd.
- Dölj avvikelser efter åtgärd utan historik.
- Anta att alla kontroller görs samma dag.
- Anta att utförare och granskare är samma person.
- Anta att foto alltid behövs.

## Hjälpstrategi För Låg Digital Vana

### Visa Hellre Än Förklara Långt

Använd:

- exempel
- korta hjälptexter
- tydliga steg
- tydliga knappar
- visuell status
- sammanställning

Undvik:

- långa introduktioner
- manualtext i arbetsflödet
- många val samtidigt
- tekniska begrepp

### Gör Återupptag Enkelt

Många användare kommer att avbryta och fortsätta senare.

Appen ska visa:

- pågående egenkontroller
- senaste ändring
- hur långt användaren kommit
- nästa sak att göra

Exempel:

"Fortsätt där du slutade: 6 av 17 punkter är bedömda."

### Bekräfta Att Saker Sparas

Ovana användare behöver trygghet.

Använd enkla bekräftelser:

- "Utkastet är sparat."
- "Kommentaren är sparad."
- "Fotot är tillagt."
- "Egenkontrollen är slutförd."

## Minimera Fel I Kritiska Lägen

### Innan Start

Kontrollera att:

- mall är vald
- projektinformation finns
- minst en kontrollpunkt finns
- referenser kan anges eller aktivt lämnas tomma

### Vid Negativt Resultat

Kräv kommentar när:

- punkt är Ej godkänd
- punkt är Ej kontrollerad

Gör kommentaren enkel att skriva direkt.

### Innan Slutförande

Visa varning om:

- punkter är Ej bedömda
- Ej godkänd saknar kommentar
- Ej kontrollerad saknar orsak
- signering saknas
- granskning förväntas men saknas

### Vid Export

Visa förhandsgranskning eller tydlig sammanställning så användaren ser vad rapporten kommer innehålla.

## Mobil Och Byggplats

Appen ska fungera bra på mobil eftersom många kontroller sker på plats.

Prioritera:

- stora klickytor
- tydliga statusknappar
- korta texter
- enkel navigering
- sparat läge
- snabb återupptagning
- tydlig kontrast
- möjlighet att arbeta stegvis

Undvik:

- täta tabeller i arbetsläget
- små kryssrutor
- långa horisontella rader
- för många fält samtidigt
- viktig information endast i hover-tooltip

Tooltips får inte vara enda sättet att förstå viktiga saker på mobil.

## Från Word-Blankett Till Arbetsflöde

Originaldokumentens Word-layout ska inte kopieras rakt av i arbetsläget.

Word har:

- tabeller
- rutor
- underskriftsrader
- tomma fält
- instruktioner på papper

Appen ska i stället ha:

- steg
- kort
- listor
- statusknappar
- tydliga kommentarer
- automatisk datumhantering
- sammanställning
- exportvänlig rapport

Word-känslan är viktig i slutrapporten, inte i arbetsflödet.

## Visuell Hierarki

Varje vy ska ha tydlig ordning:

1. Sidans rubrik.
2. Kort förklaring eller status.
3. Huvudhandling.
4. Nödvändiga fält eller kontrollpunkter.
5. Hjälp och exempel vid behov.
6. Sekundära handlingar.

Använd visuella signaler för:

- Godkänd
- Ej godkänd
- Ej kontrollerad
- Ej bedömd
- Pågående
- Slutförd

Färg får aldrig vara enda informationsbärare. Visa alltid text.

## Ton I Upplevelsen

UX ska kännas som en erfaren arbetsledare.

Det betyder:

- appen visar nästa steg
- appen säger till när något saknas
- appen ger exempel i stället för föreläsning
- appen låter användaren göra jobbet utan onödiga hinder
- appen sparar och sammanfattar
- appen gör avvikelser synliga utan att överdramatisera

Appen ska inte:

- skälla
- överförklara
- använda myndighetston
- gömma viktiga problem
- låta användaren signera utan tydlig sammanställning

## UX-Regler Per Innehållstyp

### Tooltip

Använd för kort begreppsförklaring.

Exempel:

"Byggherre: Den som låter utföra byggarbetet."

### Hjälptext

Använd när användaren behöver veta vad som ska fyllas i.

Exempel:

"Lägg till ritningar, krav eller anvisningar som kontrollen görs mot."

### Exempel

Använd före långa instruktioner.

Exempel:

"Ritning A-40.1-101, rev B"

### Varning

Använd när något riskerar att bli otydligt eller fel.

Exempel:

"Det finns kontrollpunkter som inte är bedömda. Kontrollera dem innan du slutför."

### Bekräftelse

Använd när något är sparat eller klart.

Exempel:

"Utkastet är sparat."

### Checklista

Använd inför viktiga steg.

Exempel:

- Kontrollera ej bedömda punkter.
- Läs kommentarer på ej godkända punkter.
- Signera egenkontrollen.

## Tillgänglighet Och Trygghet

Appen ska kunna användas av personer med olika vana, olika enheter och olika arbetsmiljöer.

Riktlinjer:

- tydlig kontrast
- stora klickytor
- text tillsammans med ikoner
- tangentbordsstöd där det är relevant
- begriplig feltext
- sparat arbete ska inte försvinna
- svenska datumformat
- inga dolda kritiska steg

## UX-Do And Do Not

### Gör

- Led användaren steg för steg.
- Visa ett beslut i taget.
- Ge exempel där användaren ska skriva.
- Förklara begrepp nära fältet.
- Visa status tydligt.
- Kräv kommentar när spårbarhet behövs.
- Sammanfatta innan signering.
- Bekräfta när något sparats.
- Gör det lätt att återuppta arbete.

### Gör Inte

- Visa allt på en gång.
- Kopiera Word-tabellen som arbetsvy.
- Använd svåra systemord.
- Göm avvikelser.
- Förifyll kontrollpunkter som Godkänd.
- Låt färg vara enda signal.
- Tvinga användaren att läsa långa instruktioner.
- Bygg appen som om användaren är administratör på heltid.

## Mått På Bra UX

En vy är bra när användaren snabbt kan svara på:

- Vad är detta?
- Vad ska jag göra nu?
- Varför behövs det?
- Vad saknas?
- Kan jag fortsätta senare?
- Vad händer när jag slutför?

Om användaren måste gissa, läsa långa texter eller förstå systemlogik har vyn misslyckats.

## Sammanfattning

Egenkontroll App ska göra byggdokumentation lättare, inte tyngre.

Den bästa upplevelsen är när användaren känner:

- jag vet vad jag ska göra
- jag kan rätta misstag innan rapporten blir klar
- jag behöver inte förstå ett stort system
- jag får hjälp när jag behöver det
- rapporten blir tydlig nog att lämna vidare

Appen ska vara enkel nog för den ovana användaren och tydlig nog för den erfarna arbetsledaren.
