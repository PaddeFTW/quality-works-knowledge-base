# CONTENT_GUIDE

## Syfte

Detta dokument beskriver när **Egenkontroll App** ska använda olika typer av innehållsstöd: tooltip, hjälptext, exempel, placeholder, varning, information, bekräftelse, checklistor, bilder och ikoner.

Målet är att hjälpa oerfarna användare att förstå vad de ska göra, utan att appen blir tung, pratig eller svår att använda på byggplatsen.

## Grundprincip

Använd rätt stöd på rätt plats.

En oerfaren användare behöver ofta hjälp med tre saker:

- Vad betyder ordet?
- Vad ska jag fylla i?
- Vad händer om jag går vidare?

Appen ska svara på dessa frågor där de uppstår. Den ska inte samla all hjälp i långa manualtexter.

## Beslutsregel

Välj innehållstyp så här:

- Använd **tooltip** för kort begreppsförklaring.
- Använd **hjälptext** när användaren behöver förstå ett fält eller steg.
- Använd **exempel** när användaren behöver se rätt nivå eller format.
- Använd **placeholder** för kort exempel inne i ett tomt fält.
- Använd **varning** när användaren kan göra något riskabelt eller ofullständigt.
- Använd **information** när användaren behöver förstå sammanhang innan beslut.
- Använd **bekräftelse** när något har sparats, ändrats eller slutförts.
- Använd **checklistor** när flera saker måste kontrolleras innan nästa steg.
- Använd **bilder** när text inte räcker för att visa vad som menas.
- Använd **ikoner** för snabb igenkänning, inte som enda informationsbärare.

## Tooltip

### När används tooltip?

Använd tooltip när ett ord kan vara oklart men användaren inte behöver en lång förklaring.

Bra för:

- Byggherre
- Beställare
- Entreprenör
- Kontrollpunkt
- Referens
- Ej bedömd
- Ej kontrollerad
- Signering
- Granskning

### Varför?

Tooltips hjälper oerfarna användare utan att störa vana användare. De gör att appen kan använda rätt byggterm och ändå vara lätt att förstå.

### Hur ska tooltip skrivas?

- En kort mening.
- Förklara ordet, inte hela arbetsflödet.
- Använd vardagssvenska.
- Undvik juridisk eller teknisk fördjupning.

### Exempel

- **Byggherre:** "Den som låter utföra byggarbetet."
- **Beställare:** "Den som har beställt arbetet."
- **Kontrollpunkt:** "En sak som ska kontrolleras och få ett resultat."
- **Referens:** "Ritning, krav eller anvisning som kontrollen görs mot."
- **Signering:** "Bekräftelse med namn och tidpunkt."

### När används inte tooltip?

Använd inte tooltip när:

- användaren måste läsa informationen för att kunna fortsätta
- texten behöver vara mer än en mening
- det gäller ett fel eller en varning
- samma information redan syns tydligt på sidan

Då passar hjälptext, information eller varning bättre.

## Hjälptext

### När används hjälptext?

Använd hjälptext nära ett fält, val eller steg när användaren behöver förstå vad som ska göras.

Bra för:

- mallval
- projektinformation
- beställare / byggherre
- referenser
- anpassning av kontrollpunkter
- ej godkänd
- ej kontrollerad
- signering
- granskning

### Varför?

Hjälptext minskar osäkerhet och fel. För oerfarna användare är det ofta skillnaden mellan att våga fortsätta och att fastna.

### Hur ska hjälptext skrivas?

- En eller två meningar.
- Säg vad användaren ska göra.
- Förklara varför om det behövs.
- Använd konkreta ord.
- Placera texten nära fältet eller steget.

### Exempel

**Projektinformation**
"Ange uppgifter som gör att egenkontrollen går att koppla till rätt projekt och plats."

**Referenser**
"Lägg till ritningar, krav eller anvisningar som kontrollen görs mot."

**Ej godkänd**
"Skriv vad som inte stämmer och vad som behöver göras."

**Ej kontrollerad**
"Skriv varför punkten inte har kontrollerats."

### När används inte hjälptext?

Använd inte hjälptext när:

- fältetiketten redan är självklar
- texten bara upprepar rubriken
- användaren behöver en visuell kontrollista
- användaren behöver se ett konkret format

Då passar exempel, placeholder eller checklista bättre.

## Exempel

### När används exempel?

Använd exempel när användaren behöver förstå format, nivå eller typ av information.

Bra för:

- referenser
- kommentarer
- åtgärder
- övriga anteckningar
- projektnamn
- kontrollpunkter
- fotobeskrivningar

### Varför?

Oerfarna användare kan förstå en uppgift men ändå vara osäkra på hur detaljerat de ska skriva. Exempel visar rätt nivå utan långa instruktioner.

### Hur ska exempel skrivas?

- Realistiskt.
- Kort.
- Byggnära.
- Inte för perfekt eller akademiskt.
- Gärna flera exempel om det finns olika situationer.

### Exempel

**Referenser:**

- "Ritning A-40.1-101, rev B"
- "Monteringsanvisning från leverantör"
- "Teknisk beskrivning, kapitel målning"

**Kommentar vid ej godkänd:**

- "Tätskikt saknas vid genomföring. Åtgärdas innan nästa moment."
- "Material överensstämmer inte med beställning."

**Kommentar vid ej kontrollerad:**

- "Punkten kunde inte kontrolleras eftersom ytan var inbyggd."
- "Momentet ingår inte i detta uppdrag."

### När används inte exempel?

Använd inte exempel när:

- det kan uppfattas som förvalt svar
- användaren behöver skriva helt egen information
- exemplet riskerar att styra användaren fel
- fältet är så enkelt att exempel stör

## Placeholder

### När används placeholder?

Använd placeholder inne i ett tomt fält för att visa ett kort exempel på format.

Bra för:

- egenkontrollens namn
- projekt
- arbetsplats
- beställare / byggherre
- entreprenör
- referens
- kontrollant
- kommentar

### Varför?

Placeholder hjälper användaren snabbt se vilken typ av text som passar i fältet.

### Hur ska placeholder skrivas?

- Kort exempel.
- Ingen viktig instruktion.
- Ingen text som måste läsas för att förstå fältet.
- Byggnära och realistiskt.

### Exempel

- Egenkontrollens namn: "Egenkontroll badrum, plan 2"
- Projekt: "Ombyggnad kontor, kv. Exemplet"
- Arbetsplats: "Hus A, plan 3"
- Referens: "Ritning A-40.1-101, rev B"
- Kommentar: "Beskriv brist, orsak eller åtgärd"

### När används inte placeholder?

Använd inte placeholder när:

- informationen är viktig och måste synas efter att användaren börjat skriva
- texten blir lång
- fältet redan har ett tydligt exempel bredvid
- användaren kan tro att placeholdern är ett riktigt värde

Då passar hjälptext eller exempel bättre.

## Varning

### När används varning?

Använd varning när användaren kan fortsätta men riskerar att skapa en ofullständig eller otydlig egenkontroll.

Bra för:

- ej bedömda kontrollpunkter vid slutförande
- ej godkända punkter utan kommentar
- ej kontrollerade punkter utan orsak
- saknade referenser
- signering innan sammanställningen är genomgången
- slutförande av kontroll med öppna brister

### Varför?

Varningar hjälper oerfarna användare att upptäcka misstag innan rapporten blir fel eller svår att förstå.

### Hur ska varning skrivas?

- Säg vad som saknas eller är riskabelt.
- Säg vad användaren bör göra.
- Var tydlig men inte hotfull.
- Undvik skuld.

### Exempel

- "Det finns kontrollpunkter som inte är bedömda. Kontrollera dem innan du slutför."
- "Kommentar krävs när en punkt är ej godkänd."
- "Skriv varför punkten inte har kontrollerats."
- "Kontrollera att referenserna stämmer innan du slutför."
- "Foto ersätter inte kommentar. Skriv kort vad bilden visar."

### När används inte varning?

Använd inte varning för:

- normal information
- lyckade handlingar
- tips som inte påverkar kvaliteten
- små visuella förklaringar

För många varningar gör användaren blind för viktiga varningar.

## Information

### När används information?

Använd information när användaren behöver förstå sammanhang, men det inte är ett fel eller en risk.

Bra för:

- skillnaden mellan beställare och byggherre
- vad signering betyder i appen
- att en mall kan anpassas
- att originalmallen inte ändras
- vad en referens är
- vad som händer vid slutförande

### Varför?

Information bygger trygghet. Den hjälper oerfarna användare att förstå varför steget finns utan att appen känns kontrollerande.

### Hur ska information skrivas?

- Kort rubrik.
- En till tre meningar.
- Praktisk förklaring.
- Inga långa regler.

### Exempel

**Om mallar**
"Mallen är en startpunkt. Du kan ta bort punkter som inte gäller och lägga till egna punkter."

**Om signering**
"Signering i appen är en bekräftelse med namn och tidpunkt. Det är inte BankID eller avancerad e-signering."

**Om referenser**
"Referenser är ritningar, krav eller anvisningar som kontrollen görs mot."

### När används inte information?

Använd inte information när:

- användaren har gjort fel
- en obligatorisk uppgift saknas
- det krävs ett aktivt beslut
- texten bara upprepar sidan

Då passar varning, felmeddelande eller hjälptext bättre.

## Bekräftelse

### När används bekräftelse?

Använd bekräftelse när appen ska visa att något har hänt.

Bra för:

- sparat utkast
- skapad egenkontroll
- uppdaterad kontrollpunkt
- tillagd bilaga
- tillagt foto
- signerad egenkontroll
- granskad egenkontroll
- slutförd egenkontroll
- skapad rapport

### Varför?

Bekräftelser ger trygghet, särskilt för ovana användare. De visar att arbetet inte har försvunnit.

### Hur ska bekräftelse skrivas?

- Kort.
- Konkret.
- Ange vad som hänt.
- Undvik tekniska ord.

### Exempel

- "Utkastet är sparat."
- "Egenkontrollen är skapad."
- "Kontrollpunkten är uppdaterad."
- "Fotot är tillagt."
- "Egenkontrollen är signerad."
- "Egenkontrollen är slutförd."
- "Rapporten är klar för export."

### När används inte bekräftelse?

Använd inte bekräftelse för:

- saker som inte sparas eller ändras
- varje liten tangenttryckning
- fel eller risker
- information som användaren redan tydligt ser

För många bekräftelser kan störa arbetsflödet.

## Checklistor

### När används checklistor?

Använd checklistor när flera saker behöver gås igenom innan användaren går vidare.

Bra för:

- innan kontrollen startar
- innan slutförande
- vid granskning
- vid export
- vid uppföljning av avvikelser

### Varför?

Checklistor hjälper oerfarna användare att inte missa viktiga steg. De passar särskilt bra när användaren behöver känna sig säker innan ett beslut.

### Hur ska checklistor skrivas?

- Kort punktlista.
- En sak per rad.
- Börja gärna med verb.
- Visa gärna vad som är klart och vad som saknas.
- Använd inte för långa listor.

### Exempel

**Innan du startar kontrollen:**

- Kontrollera att rätt mall är vald.
- Ta bort punkter som inte gäller.
- Lägg till projektspecifika punkter.
- Kontrollera att referenserna stämmer.

**Innan du slutför:**

- Kontrollera ej bedömda punkter.
- Läs kommentarer på ej godkända punkter.
- Kontrollera orsaker till ej kontrollerade punkter.
- Gå igenom avvikelser och åtgärder.
- Signera egenkontrollen.

### När används inte checklistor?

Använd inte checklistor när:

- det bara finns en sak att göra
- användaren redan är mitt i ett snabbt formulärflöde
- listan blir så lång att den känns som manual
- informationen passar bättre som sammanställning

## Bilder

### När används bilder?

Använd bilder när text inte räcker för att hjälpa användaren förstå eller dokumentera något.

I Egenkontroll App kan bilder betyda två saker:

- bilder i appens stödmaterial, till exempel illustrationer
- foton som användaren lägger till som dokumentation

### Varför?

Byggarbete är visuellt. En bild kan visa placering, brist, utförande eller åtgärd snabbare än text.

### Bilder som stöd i appen

Använd sparsamt för:

- onboarding
- förklaring av flöde
- exempel på rapport
- exempel på foto som dokumentation

Undvik dekorativa bilder som inte hjälper användaren.

### Foton som dokumentation

Använd foto när användaren behöver visa:

- utfört arbete
- brist
- dold installation innan inbyggnad
- material eller märkning
- åtgärdat fel

### Viktig regel

Foto ersätter inte resultat, kommentar eller ansvar. Det ska stödja dokumentationen, inte vara hela dokumentationen.

### När används inte bilder?

Använd inte bilder när:

- text räcker
- bilden bara är dekoration
- bilden gör sidan långsam eller rörig
- användaren kan tro att foto ersätter kontrollresultat

## Ikoner

### När används ikoner?

Använd ikoner för snabb igenkänning och visuell struktur.

Bra för:

- statusar
- dokument
- bilaga
- foto
- varning
- bekräftelse
- export
- utskrift
- signering
- granskning

### Varför?

Ikoner gör appen snabbare att skanna, särskilt på mobil och i listor. De kan hjälpa ovana användare hitta rätt funktion.

### Hur ska ikoner användas?

- Tillsammans med text.
- Konsekvent.
- Enkla och välkända symboler.
- Inte för många på samma yta.
- Inte som enda informationsbärare.

### Exempel

- Check-symbol + "Godkänd"
- Varningssymbol + "Ej godkänd"
- Kameraikon + "Foto"
- Dokumentikon + "Bilaga"
- Penna/signaturikon + "Signera"
- Skrivarsymbol + "Skriv ut rapport"

### När används inte ikoner?

Använd inte ikoner när:

- ikonen inte är självklar
- texten redan är tydlig och ytan är trång
- flera ikoner konkurrerar om uppmärksamhet
- ikonen riskerar att tolkas fel

## Kombinationer Som Fungerar Bra

### Fält Med Oklart Begrepp

Använd:

- fältetikett
- tooltip
- kort hjälptext vid behov
- placeholder som exempel

Exempel:

- Etikett: "Beställare / byggherre"
- Tooltip: "Beställare är den som beställt arbetet. Byggherre är den som låter utföra byggarbetet."
- Placeholder: "AB Exempel"

### Kontrollpunkt Med Negativt Resultat

Använd:

- tydlig status
- hjälptext
- obligatorisk kommentar
- möjlighet till foto eller bilaga
- varning om kommentar saknas

Exempel:

- Status: "Ej godkänd"
- Hjälptext: "Skriv vad som inte stämmer och vad som behöver göras."
- Varning: "Kommentar krävs när en punkt är ej godkänd."

### Slutförande

Använd:

- sammanställning
- checklista
- varning för saknade uppgifter
- information om vad slutförande innebär
- bekräftelse när det är klart

Exempel:

- Information: "När egenkontrollen slutförs blir den färdig dokumentation."
- Varning: "Det finns kontrollpunkter som inte är bedömda."
- Bekräftelse: "Egenkontrollen är slutförd."

## Prioritet För Oerfarna Användare

När användaren är ny eller osäker ska appen prioritera:

1. Tydlig rubrik: vad gör jag nu?
2. Kort hjälptext: varför behövs detta?
3. Exempel: hur kan jag skriva?
4. Varning: vad får jag inte missa?
5. Bekräftelse: blev det sparat?

Undvik att visa allt på en gång. Visa stöd i rätt steg.

## Innehåll Som Ska Undvikas

Undvik:

- långa manualtexter i arbetsflödet
- flera hjälptexter som säger samma sak
- varningar för normala steg
- tooltips med långa stycken
- placeholders som innehåller viktiga instruktioner
- bilder som bara dekoration
- ikoner utan text
- konsultsvenska
- myndighetssvenska
- tekniska systemord

## Checklista För Innehållsstöd

Innan nytt innehållsstöd läggs till, fråga:

- Hjälper detta användaren att göra rätt?
- Är detta rätt innehållstyp?
- Kan texten kortas?
- Är språket vardagligt?
- Är det tydligt vad användaren ska göra?
- Stör stödet vana användare i onödan?
- Hjälper det särskilt oerfarna användare?
- Går det att visa exempel i stället för lång förklaring?

Om stödet inte hjälper användaren att komma vidare eller undvika misstag ska det tas bort eller skrivas om.
