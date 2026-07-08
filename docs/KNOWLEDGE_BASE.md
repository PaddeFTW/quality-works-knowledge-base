# KNOWLEDGE_BASE

## Syfte

Detta dokument är kunskapsbas för **Egenkontroll App**.

Kunskapsbasen beskriver den byggspecifika arbetslogiken, språket, informationsstrukturen och användarvärdet som ska bevaras när originalmaterial från KvalitetsDokument.se omvandlas från dokumentmallar till en enkel digital produkt.

Originaldokumenten ska inte behandlas som teknisk specifikation. De är källor till fackkunskap, arbetsordning, kontrollspråk, ansvarsfördelning och dokumentationspraxis.

## Källprinciper

Primär kunskapskälla är KvalitetsDokument.se:s material inom bygg, särskilt:

- Word-mallen för egenkontroll i bygg.
- Masterlistan för egenkontroller.
- Quality Works-materialets återkommande arbetsmönster för dokument, ansvar, resultat, uppföljning och användarstöd.

Egenkontroll App ska endast använda den kunskap som är relevant för egenkontroll i bygg. Generella Quality Works-moduler som personalenkät, leverantörsbedömning, kundtillfredsställelse, internrevision, miljöaspekter, avvikelsehantering och ISO-ledningssystem är inte produktområden för denna app, men de visar återkommande mönster:

- tydlig startpunkt
- stegvis ifyllnad
- ansvarig roll
- resultat eller status
- kommentar vid avvikelse
- sammanställning
- export eller utskrift
- enkel svenska
- stöd för både administratör och vanlig användare

## Grundsyn På Produkten

Egenkontroll App ska inte digitalisera ett Word-dokument sida för sida. Appen ska bevara dokumentens professionella byggkunskap och göra den lättare att använda i verkligt arbete.

Det viktigaste användarvärdet är att en entreprenör, arbetsledare, platschef, kontrollant eller kontrollansvarig snabbt kan:

- välja rätt egenkontroll
- anpassa kontrollpunkterna till projektet
- genomföra kontrollerna utan att tappa spårbarhet
- dokumentera resultat och undantag
- signera eller bekräfta utfört arbete
- skapa en tydlig rapport som kan sparas, granskas och lämnas vidare

## Gemensamma Arbetsflöden

### Huvudflöde För Egenkontroll

Det återkommande arbetsflödet är:

1. Välj eller skapa egenkontroll.
2. Ange projektinformation.
3. Ange beställare eller byggherre.
4. Ange entreprenör.
5. Ange vilka krav, ritningar eller handlingar kontrollen avser.
6. Granska och anpassa kontrollpunkterna.
7. Starta kontrollen.
8. Bedöm varje kontrollpunkt.
9. Skriv kommentar när något inte är godkänt eller inte har kontrollerats.
10. Ange kontrollant och datum.
11. Granska sammanställning.
12. Signera som utförare.
13. Låt kontrollansvarig eller ansvarig person granska.
14. Exportera eller skriv ut rapport.

### Arbetsflöde För Anpassning

Originaldokumenten visar att egenkontroller ofta behöver anpassas till det faktiska projektet. Därför ska användaren förstå att en mall är en startpunkt, inte en låst sanning.

Anpassningsflödet är:

1. Välj relevant mall.
2. Läs kort beskrivning.
3. Ta bort irrelevanta punkter.
4. Lägg till projektspecifika punkter.
5. Justera formuleringar så de matchar arbetet.
6. Kontrollera att referenser till ritningar, krav och handlingar är korrekta.
7. Starta kontrollen först när listan motsvarar projektet.

### Arbetsflöde För Återupptag

Egenkontroll är ofta ett löpande arbete. Kunskapen i dokumenten antyder inte att allt sker vid ett enda tillfälle.

Återupptagsflödet är:

1. Öppna pågående egenkontroll.
2. Se tydligt vilka punkter som återstår.
3. Fortsätt från nästa ej bedömda punkt.
4. Ändra tidigare resultat vid behov innan slutförande.
5. Slutför först när alla nödvändiga punkter är behandlade.

### Arbetsflöde För Granskning

Granskningens syfte är inte avancerad juridisk e-signering. Syftet är att tydligt visa att en ansvarig person har kontrollerat sammanställningen.

Granskningsflödet är:

1. Läs sammanställning.
2. Kontrollera ej godkända och ej kontrollerade punkter.
3. Läs kommentarer.
4. Kontrollera att utförare och datum finns.
5. Lägg till granskningskommentar vid behov.
6. Bekräfta granskning med namn och tidpunkt.

## Återkommande Kontrollpunkter

Kontrollpunkter i egenkontroller är formulerade som verifierbara observationer eller bekräftelser. De ska inte vara långa instruktionstexter.

Återkommande kontrolltyper:

- kontroll mot ritning
- kontroll mot teknisk beskrivning
- kontroll mot beställarens krav
- kontroll av material
- kontroll av utförande
- kontroll av mått, placering eller nivå
- kontroll av infästning, montering eller anslutning
- kontroll av täthet, funktion eller provning
- kontroll av underlag innan nästa moment
- kontroll av egen dokumentation
- kontroll av städning, skydd eller säkerhet
- kontroll inför överlämning eller slutbesiktning

Kontrollpunkter bör vara skrivna så att användaren kan svara:

- godkänd
- ej godkänd
- ej kontrollerad
- ännu ej bedömd

Bra kontrollpunkter är korta, konkreta och handlingsnära.

Exempel på kunskapsmönster:

- "Kontrollera att arbetet är utfört enligt ritning."
- "Kontrollera att material överensstämmer med beställning och handling."
- "Kontrollera att genomföring är tätad."
- "Kontrollera att underlaget är rent, torrt och lämpligt för nästa moment."
- "Kontrollera att skyddsåtgärder är utförda innan arbetet fortsätter."

## Återkommande Dokument

Följande dokumenttyper och informationsbärare återkommer i källmaterialet och ska förstås av appen som referenser, inte som separata moduler:

- egenkontroll
- kontrollplan
- ritning
- teknisk beskrivning
- arbetsberedning
- monteringsanvisning
- produktblad
- materialintyg
- fotodokumentation
- avvikelse eller felnotering
- besiktningsprotokoll
- slutrapport
- utskrift eller PDF

I Egenkontroll App är de viktigaste dokumenten:

- vald egenkontrollmall
- skapad projektspecifik egenkontroll
- kontrollpunktslista
- kommentar- och avvikelseunderlag
- signeringsuppgift
- granskningsuppgift
- exporterad rapport

## Roller

### Beställare

Beställaren är den part som beställer arbetet. I vissa byggsammanhang används även byggherre. Appen ska låta användaren välja eller förstå båda begreppen.

### Byggherre

Byggherren är den som låter utföra byggnads-, rivnings- eller markåtgärder. Begreppet är viktigt i byggprojekt och bör inte förenklas bort.

### Entreprenör

Entreprenören är den som utför arbetet eller ansvarar för utförandet. Detta kan vara huvudentreprenör eller underentreprenör beroende på projektet.

### Underentreprenör

Underentreprenören utför ett avgränsat arbetsmoment åt en annan entreprenör. Rollen är relevant eftersom många egenkontroller genomförs på momentnivå.

### Utförare

Utföraren är den person eller organisation som faktiskt har utfört arbetet som kontrolleras.

### Kontrollant

Kontrollanten är den person som bedömer en eller flera kontrollpunkter. Det kan vara samma person som utfört arbetet eller en annan utsedd person.

### Kontrollansvarig

Kontrollansvarig är den roll som granskar att egenkontrollen är genomförd och dokumenterad. I appen ska rollen hanteras varsamt: granskning i appen är en dokumenterad bekräftelse, inte automatiskt en myndighetsformell signatur.

### Arbetsledare Eller Platschef

Arbetsledare eller platschef ansvarar ofta praktiskt för att kontroller utförs, följs upp och samlas in.

### Administratör

Administratörsmönstret från Quality Works-materialet visar behov av att någon kan förbereda mallar, användare eller inställningar. För Egenkontroll App ska detta hållas enkelt och inte bli en stor organisationsmodul i första versionen.

## Ansvar

Ansvar i egenkontroll handlar om spårbarhet:

- vem har utfört eller ansvarat för arbetet
- vem har kontrollerat punkten
- när gjordes kontrollen
- vilket underlag kontrollerades mot
- vad blev resultatet
- vad behöver förklaras
- vem har granskat slutresultatet

Appen ska hjälpa användaren att dokumentera ansvar utan att göra juridiska påståenden som källmaterialet inte stödjer.

## Arbetsmoment

Arbetsmomenten i egenkontroll kan grupperas i följande nivåer:

- projektuppstart
- val av kontrolltyp
- projektanpassning
- utförandekontroll
- kontroll av avvikelse eller brist
- komplettering
- sammanställning
- signering
- granskning
- export och arkivering

Vanliga byggmoment i mallbiblioteket:

- generell bygg
- elinstallation
- VVS
- badrum
- kök
- betong
- rivning
- tak
- målning
- slutbesiktning
- daglig säkerhet

Alla moment ska använda samma grundlogik. Skillnaden ska ligga i kontrollpunkternas innehåll, inte i ett nytt appflöde per yrkesområde.

## Begrepp

### Egenkontroll

En egenkontroll är en dokumenterad kontroll av att ett arbete, ett material eller ett arbetsmoment uppfyller krav, ritningar, anvisningar eller överenskomna handlingar.

### Kontrollpunkt

En kontrollpunkt är en avgränsad sak som ska bedömas. Den ska kunna få ett resultat och vid behov en kommentar.

### Kontrollmoment

Kontrollmoment är en grupp eller del av arbetet där flera kontrollpunkter kan ingå.

### Referens

Referens är det underlag kontrollen görs mot, till exempel ritning, beskrivning, krav, anvisning eller annan handling.

### Godkänd

Punkten är kontrollerad och uppfyller aktuellt krav eller underlag.

### Ej Godkänd

Punkten är kontrollerad men uppfyller inte aktuellt krav eller underlag. Kommentar ska krävas.

### Ej Kontrollerad

Punkten har inte kontrollerats, eller kunde inte kontrolleras. Kommentar ska krävas eftersom orsaken behöver vara spårbar.

### Ej Bedömd

Punkten är ännu inte behandlad. Detta är ett arbetsläge, inte ett slutresultat.

### Utfört Av

Person eller funktion som bekräftar att arbetet eller egenkontrollen är utförd.

### Granskad Av

Person eller funktion som bekräftar att egenkontrollen har granskats.

### Övriga Anteckningar

Sammanfattande fri text som hör till hela egenkontrollen. Punktvisa kommentarer ska helst ligga på respektive kontrollpunkt.

## Relationer

Kunskapsrelationerna i appen är:

- en mall kan skapa många egenkontroller
- en egenkontroll skapas från en mall eller som tom egenkontroll
- en egenkontroll tillhör ett projekt eller arbetsuppdrag
- en egenkontroll har en beställare eller byggherre
- en egenkontroll har en entreprenör
- en egenkontroll har en eller flera referenser
- en egenkontroll innehåller kontrollpunkter
- en kontrollpunkt kan tillhöra en grupp eller ett arbetsmoment
- en kontrollpunkt har exakt ett aktuellt resultat
- en kontrollpunkt kan ha kommentar, kontrollant och datum
- en egenkontroll kan ha övergripande anteckningar
- en egenkontroll kan signeras av utförare
- en egenkontroll kan granskas av kontrollansvarig eller ansvarig person
- en slutförd egenkontroll kan exporteras som rapport

## Informationshierarki

Informationen ska prioriteras enligt följande:

1. Vad användaren gör just nu.
2. Vilken egenkontroll och vilket projekt det gäller.
3. Vilken kontrollpunkt som ska bedömas.
4. Vilket underlag kontrollen avser.
5. Vilka resultatval som finns.
6. Om kommentar krävs.
7. Vem som kontrollerar.
8. Datum för kontroll.
9. Sammanställning av resultat.
10. Signering, granskning och export.

Appen ska undvika att lägga juridisk eller administrativ text före själva arbetsuppgiften. Hjälptext ska finnas nära rätt fält, men inte dominera flödet.

## Återkommande Språk

Källmaterialet använder enkel, praktisk och handlingsorienterad svenska.

Återkommande verb:

- välj
- fyll i
- kontrollera
- granska
- signera
- godkänn
- skriv
- lägg till
- ta bort
- ändra
- exportera
- skriv ut

Återkommande substantiv:

- kontroll
- kontrollpunkt
- kontrollmoment
- dokument
- ritning
- krav
- handling
- beställare
- byggherre
- entreprenör
- utförare
- kontrollansvarig
- kommentar
- anteckning
- resultat
- datum
- signatur

Ton:

- kort
- tydlig
- saklig
- byggnära
- utan marknadsföringsspråk
- utan onödigt system- eller ISO-språk i användarflödet

## Rekommenderade Formuleringar

### Primära Handlingar

- "Skapa ny egenkontroll"
- "Välj mall"
- "Fyll i projektinformation"
- "Anpassa kontrollpunkter"
- "Starta kontroll"
- "Granska sammanställning"
- "Signera egenkontroll"
- "Markera som granskad"
- "Exportera PDF"
- "Skriv ut rapport"

### Statusar

- "Ej bedömd"
- "Godkänd"
- "Ej godkänd"
- "Ej kontrollerad"
- "Pågående"
- "Slutförd"
- "Klar för granskning"
- "Granskad"

### Bekräftelser

- "Jag bekräftar att uppgifterna är korrekta."
- "Jag har granskat egenkontrollen."
- "Egenkontrollen är slutförd."
- "Rapporten är klar för export."

### Varningar

- "Det finns kontrollpunkter som inte är bedömda."
- "Kommentar krävs när en punkt är ej godkänd."
- "Kommentar krävs när en punkt är ej kontrollerad."
- "Kontrollera att referenserna stämmer innan du slutför."
- "En slutförd egenkontroll bör inte ändras utan ny version eller återöppning."

## Vanliga Misstag

Vanliga misstag som appen bör förebygga:

- användaren väljer fel mall
- användaren startar kontrollen utan att anpassa punkterna till projektet
- beställare och byggherre blandas ihop utan förklaring
- referenser till ritningar eller handlingar saknas
- kontrollpunkter lämnas ej bedömda men egenkontrollen betraktas ändå som färdig
- ej godkända punkter saknar kommentar
- ej kontrollerade punkter saknar orsak
- samma kommentar skrivs endast i övriga anteckningar i stället för på rätt kontrollpunkt
- datum saknas eller blir otydligt
- kontrollant saknas
- utförare och granskare blandas ihop
- enkel signering misstolkas som avancerad elektronisk signatur
- Word-layoutens rutor och linjer kopieras i appen i stället för att skapa ett tydligt arbetsflöde
- för många funktioner läggs till innan kärnflödet är stabilt

## Word-Layout Kontra Kunskap

### Delar Som Är Word-Layout

Följande delar ska inte kopieras bokstavligt till appens arbetsflöde:

- sidhuvud och sidfot
- fasta tabellrader
- manuella kryssrutor
- tomma linjer för handskriven text
- statiska underskriftsrader
- layoutstyrda mellanrubriker
- upprepade instruktioner som finns för att användaren läser ett papper
- utrymme som bara behövs för utskrift
- manuell placering av datum och signatur per rad

Word-layouten är däremot relevant för exporten. Slutrapporten ska vara tydlig, utskriftsvänlig och kännas som ett professionellt byggdokument.

### Delar Som Innehåller Kunskap

Följande delar innehåller produktkunskap och ska bevaras:

- vilka uppgifter som krävs innan kontroll
- skillnaden mellan beställare, byggherre och entreprenör
- att kontrollen ska hänvisa till krav, ritningar eller andra handlingar
- kontrollpunkternas ämnen och ordning
- statusarna för resultat
- behovet av datum och kontrollant
- behovet av signering
- behovet av kontrollansvarigs granskning
- förklaring av resultat
- övriga anteckningar
- export som dokumentation

### Delar Som Ger Användaren Värde

Högst användarvärde finns i:

- mallbiblioteket
- färdiga kontrollpunkter
- möjlighet att anpassa kontrollpunkter
- tydligt statusval
- krav på kommentar vid brist eller utebliven kontroll
- automatisk sammanställning
- sparade utkast
- tydlig signering
- tydlig granskningsmarkering
- PDF eller utskrift
- enkel återupptagning av pågående kontroll

Lågt användarvärde finns i:

- att exakt återskapa Word-tabellen i arbetsläget
- att visa långa instruktioner innan användaren får börja
- att införa stora administrationsmoduler
- att blanda in andra Quality Works-funktioner
- att skapa avancerad statistik i första versionen

## Hjälptexter

Hjälptexter ska vara korta och placeras nära den handling de förklarar.

### Mallval

"Välj den mall som bäst motsvarar arbetet. Du kan ändra, lägga till och ta bort kontrollpunkter innan kontrollen startas."

### Projektinformation

"Ange uppgifter som gör det möjligt att koppla egenkontrollen till rätt projekt, plats eller arbetsmoment."

### Beställare Eller Byggherre

"Använd Beställare när du vill ange den som beställt arbetet. Använd Byggherre när projektet kräver den byggjuridiska rollen."

### Entreprenör

"Ange företaget eller parten som ansvarar för utförandet av arbetet."

### Referenser

"Ange ritningar, beskrivningar, krav, anvisningar eller andra handlingar som kontrollen ska göras mot."

### Anpassa Kontrollpunkter

"Kontrollera att punkterna passar projektet innan du startar. Ta bort sådant som inte gäller och lägg till projektspecifika kontroller."

### Ej Godkänd

"Använd Ej godkänd när punkten är kontrollerad men inte uppfyller krav eller underlag. Skriv vad som behöver åtgärdas."

### Ej Kontrollerad

"Använd Ej kontrollerad när punkten inte kunde eller skulle kontrolleras. Skriv varför."

### Ej Bedömd

"Ej bedömd betyder att punkten återstår. Den bör inte användas som slutresultat."

### Signering

"Signering innebär att du bekräftar uppgifterna med namn och tidpunkt. Detta är inte avancerad elektronisk signering."

### Granskning

"Granskning visar att en ansvarig person har läst igenom egenkontrollen och bekräftat den."

## Exempel

Exempel ska hjälpa användaren att förstå rätt nivå på informationen.

### Exempel På Referenser

- "Ritning A-40.1-101"
- "Teknisk beskrivning, kapitel målning"
- "Monteringsanvisning från leverantör"
- "Beställarens krav daterade 2026-06-15"
- "Kontrollplan för projektet"

### Exempel På Kommentar Vid Ej Godkänd

- "Tätskikt saknas vid genomföring. Åtgärdas innan nästa moment."
- "Material överensstämmer inte med beställd produkt."
- "Infästning är inte utförd enligt anvisning."
- "Mått avviker från ritning. Behöver kontrolleras med arbetsledare."

### Exempel På Kommentar Vid Ej Kontrollerad

- "Punkten kunde inte kontrolleras eftersom ytan var inbyggd."
- "Momentet ingår inte i detta uppdrag."
- "Kontroll skjuts upp till efter komplettering."
- "Underlag saknas vid kontrolltillfället."

### Exempel På Övriga Anteckningar

- "Egenkontrollen avser etapp 1."
- "Kompletterande kontroll görs efter leverans av återstående material."
- "Samtliga ej godkända punkter ska följas upp innan överlämning."

## Tooltips

Tooltips ska förklara begrepp eller korta fält utan att ersätta hjälptexter.

Rekommenderade tooltips:

- Beställare: "Den som har beställt arbetet."
- Byggherre: "Den som låter utföra byggnads-, rivnings- eller markåtgärder."
- Entreprenör: "Företag eller part som utför eller ansvarar för arbetet."
- Referens: "Ritning, krav, beskrivning eller annan handling som kontrollen görs mot."
- Kontrollpunkt: "En sak som ska kontrolleras och få ett resultat."
- Ej bedömd: "Punkten är ännu inte behandlad."
- Godkänd: "Kontrollerad och utan noterad brist."
- Ej godkänd: "Kontrollerad men brist finns. Kommentar krävs."
- Ej kontrollerad: "Inte kontrollerad. Orsak krävs."
- Kontrollant: "Personen som har gjort bedömningen."
- Utfört av: "Personen som bekräftar egenkontrollen."
- Kontrollansvarig: "Personen som granskar eller godkänner sammanställningen."

## Placeholders

Placeholders ska visa format och förväntad nivå, inte ersätta etiketter.

### Projekt Och Parter

- Egenkontrollens namn: "Egenkontroll badrum, plan 2"
- Projekt: "Ombyggnad kontor, kv. Exemplet"
- Plats: "Hus A, plan 3"
- Beställare/byggherre: "AB Exempel"
- Entreprenör: "Byggfirma Exempel AB"
- Referens: "Ritning A-40.1-101, rev B"

### Kontrollpunkt

- Kontrollpunkt: "Kontrollera att underlaget är rent och torrt"
- Grupp: "Underlag"
- Kommentar: "Beskriv brist, orsak eller åtgärd"
- Kontrollant: "För- och efternamn"

### Signering

- Utfört av: "Namn på utförare"
- Granskad av: "Namn på kontrollansvarig"
- Granskningskommentar: "Eventuell kommentar till granskningen"

## Smarta Standardvärden

Smarta standardvärden ska minska friktion utan att dölja ansvar.

Rekommenderade standardvärden:

- Ny egenkontroll får status Utkast.
- Alla kontrollpunkter startar som Ej bedömd.
- Datum föreslås som dagens datum.
- Kontrollant föreslås som aktuell användare om inloggning finns.
- Beställare/byggherre behåller senast valt etikettval i samma egenkontroll.
- Mallens kontrollpunkter kopieras till egenkontrollen så originalmallen inte ändras.
- Kommentarfält öppnas automatiskt när användaren väljer Ej godkänd.
- Kommentarfält öppnas automatiskt när användaren väljer Ej kontrollerad.
- Sammanställningen visar antal per status.
- Slutförande varnar om någon punkt är Ej bedömd.
- Exportnamn föreslås från egenkontrollens namn och datum.
- PDF/utskrift innehåller förklaring av statusar.

Standardvärden som bör undvikas:

- att automatiskt markera punkter som godkända
- att automatiskt signera
- att dölja ej bedömda punkter
- att anta att beställare och byggherre alltid är samma sak
- att lägga in juridiska standardtexter utan sakgranskning

## Mallbibliotekets Kunskap

Mallbiblioteket är kärnan i produktens värde. Det ska uppfattas som ett professionellt startbibliotek för byggkontroller.

Version 1.0 bör innehålla:

- Bygg - generell
- Elinstallation
- VVS
- Badrum
- Kök
- Betong
- Rivning
- Tak
- Målning
- Slutbesiktning
- Daglig säkerhet
- Tom egenkontroll

Varje mall bör ha:

- namn
- kort beskrivning
- kategori
- kontrollpunkter
- eventuell gruppering
- versionsinformation
- aktiv eller inaktiv status

Mallar ska inte vara tekniska flöden. De är innehåll. Samma appflöde ska kunna användas för alla mallar.

## Resultatmodell

Varje kontrollpunkt ska ha exakt ett resultat åt gången.

Resultat:

- Ej bedömd: punkten är inte behandlad.
- Godkänd: punkten är kontrollerad och godkänd.
- Ej godkänd: punkten är kontrollerad men inte godkänd.
- Ej kontrollerad: punkten kunde eller skulle inte kontrolleras.

Kunskapsregel:

- Ej godkänd kräver kommentar.
- Ej kontrollerad kräver kommentar.
- Ej bedömd ska tillåtas under pågående arbete men ska synas tydligt i sammanställningen.
- Godkänd ska inte kräva kommentar, men kommentar ska kunna lämnas.

## Livscykel För Egenkontroll

Rekommenderad livscykel:

- Utkast: projektinformation eller kontrollpunkter förbereds.
- Pågående: kontrollen har startats.
- Klar för granskning: alla obligatoriska delar är behandlade.
- Granskad: ansvarig person har granskat.
- Slutförd: egenkontrollen är färdig och bör låsas för normal redigering.
- Arkiverad: egenkontrollen sparas men är inte aktiv.

För en enkel första version räcker:

- Utkast
- Pågående
- Slutförd

Granskning kan visas som egen markering även om appens livscykel hålls enkel.

## Export Och Rapport

Exporten är den plats där Word-dokumentets dokumentkänsla är mest relevant.

Rapporten ska innehålla:

- dokumentnamn
- projektuppgifter
- beställare eller byggherre
- entreprenör
- referenser
- samtliga kontrollpunkter
- resultat per punkt
- datum per punkt
- kontrollant per punkt
- kommentarer
- övriga anteckningar
- utfört av
- granskad av eller kontrollansvarig
- förklaring av statusar

Rapporten ska vara:

- tydlig
- utskriftsvänlig
- läsbar utan appen
- begriplig för beställare, entreprenör och granskare
- fri från onödiga appspecifika uttryck

## UX-Innehåll Per Yta

### Startsida

Viktigast:

- skapa ny egenkontroll
- fortsätt pågående egenkontroll
- hitta slutförd egenkontroll
- öppna mallbibliotek

Startsidan ska inte bli en tung dashboard.

### Mallval

Viktigast:

- mallnamn
- kort beskrivning
- antal kontrollpunkter
- kategori
- möjlighet att välja tom mall

### Projektinformation

Viktigast:

- namn på egenkontroll
- projekt eller arbetsplats
- beställare eller byggherre
- entreprenör
- referenser

### Anpassa Kontrollpunkter

Viktigast:

- se alla punkter innan start
- ändra text
- lägga till punkt
- ta bort punkt
- ändra ordning
- förstå att originalmallen inte påverkas

### Genomför Kontroll

Viktigast:

- aktuell punkt
- resultatval
- kommentar
- datum
- kontrollant
- framsteg
- nästa punkt

### Sammanställning

Viktigast:

- antal godkända
- antal ej godkända
- antal ej kontrollerade
- antal ej bedömda
- lista över punkter som kräver uppföljning
- övriga anteckningar
- signering
- granskning

### Export

Viktigast:

- förhandsgranska
- skriva ut
- skapa PDF
- tydligt dokumentnamn

## Innehåll Som Inte Ska Ingå

Följande hör inte till kunskapsbasen för Egenkontroll App v1.0:

- full Quality Works-plattform
- ISO-ledningssystem
- personalenkät
- leverantörsbedömning
- kundtillfredsställelse
- internrevision
- aktivitetsplan
- lagregister som separat modul
- miljöaspektsmodul
- avvikelsehantering som separat system
- betalning och abonnemang
- marketplace
- avancerad organisationshantering
- avancerad e-signering
- BankID
- AI-genererade kontrollpunkter
- avancerad dokumenteditor
- realtidssamarbete
- chatt
- statistikplattform

Kunskap från dessa områden får endast användas som mönster för språk, ansvar, resultat och uppföljning när det stärker Egenkontroll App.

## Kvalitetsprinciper

Egenkontroll App ska:

- använda enkel svenska
- stödja mobil, surfplatta och dator
- göra nästa steg tydligt
- göra avvikelser synliga
- inte förlora pågående arbete
- visa status med både text och färg
- inte använda färg som enda informationsbärare
- kräva kommentar när spårbarhet behövs
- skilja arbetsläge från slutrapport
- bevara byggdokumentets professionalitet vid export
- undvika juridiska påståenden som inte är sakgranskade

## Sammanfattande Kunskapsmodell

Egenkontroll App består kunskapsmässigt av fem lager:

1. Mallkunskap: färdiga byggmallar och kontrollpunkter.
2. Projektkunskap: projekt, parter och referenser.
3. Kontrollkunskap: resultat, kommentar, datum och kontrollant.
4. Ansvarskunskap: utförare, granskare och bekräftelse.
5. Dokumentkunskap: sammanställning, rapport, utskrift och PDF.

Det användaren betalar för är inte en digital kopia av en Word-fil. Det användaren får värde av är att byggkunskapen i dokumenten blir lätt att välja, förstå, fylla i, följa upp, signera och lämna vidare.
