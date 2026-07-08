# DOMAIN_MODEL

## Syfte

Detta dokument beskriver den konceptuella domänmodellen för **Egenkontroll App**.

Dokumentet förklarar hur en egenkontroll fungerar i praktiken i ett byggprojekt: vilka begrepp som ingår, hur de hänger ihop och hur arbetet rör sig från projekt och mall till genomförd kontroll, avvikelsehantering, signering och slutförande.

Detta är inte en databasmodell, inte SQL och inte en teknisk implementation.

## Grundprincip

En egenkontroll är en praktisk dokumenterad kontroll av att ett arbete, ett material eller ett arbetsmoment uppfyller krav, ritningar, anvisningar eller andra handlingar.

I appen ska egenkontrollen förstås som ett arbetsflöde, inte bara som ett dokument. Användaren väljer en mall, anpassar den till ett projekt, bedömer kontrollpunkter, dokumenterar brister, signerar och skapar till slut en rapport som kan granskas och lämnas vidare.

Den konceptuella kedjan är:

```text
Projekt
→ Mall
→ Egenkontroll
→ Kontrollmoment
→ Kontrollpunkt
→ Resultat
→ Kommentar, bilaga, foto eller avvikelse
→ Åtgärd vid behov
→ Signering
→ Slutförande
→ Dokumenterad rapport
```

## Projekt

Ett projekt är sammanhanget där egenkontrollen utförs.

Projektet kan vara ett helt byggprojekt, en etapp, en arbetsplats, ett rum, ett hus, en installation eller ett avgränsat arbetsmoment. Det viktigaste är att egenkontrollen går att koppla till rätt plats, uppdrag och ansvariga parter.

Ett projekt innehåller normalt:

- projektnamn
- plats eller arbetsområde
- beställare eller byggherre
- entreprenör
- eventuellt underentreprenör
- relevanta krav, ritningar eller handlingar
- en eller flera egenkontroller

Projektet är inte själva kontrollen. Projektet är ramen som gör kontrollen begriplig.

### Praktisk betydelse

Utan projektinformation blir egenkontrollen svår att tolka i efterhand. En kontrollpunkt som är godkänd måste kunna kopplas till rätt projekt, rätt plats och rätt underlag.

Exempel:

- Ombyggnad kontor, plan 3
- Badrum, lägenhet 1204
- Takomläggning, etapp 1
- Installation VVS, hus B

## Mall

En mall är en förberedd struktur för en viss typ av egenkontroll.

Mallen innehåller kunskap från originalmaterialet: typiska kontrollmoment, kontrollpunkter, ordning och språk. Mallen är en startpunkt, inte ett färdigt facit för varje projekt.

En mall kan exempelvis avse:

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

### Praktisk betydelse

Användaren väljer den mall som bäst motsvarar arbetet och anpassar den innan kontrollen startar.

En mall ska hjälpa användaren att komma igång snabbt, men den får inte hindra projektspecifika justeringar. Det ska vara naturligt att ta bort irrelevanta punkter, lägga till egna punkter och ändra formuleringar så att kontrollen passar projektet.

### Relationer

- En mall kan användas många gånger.
- En mall kan skapa många egenkontroller.
- En skapad egenkontroll får en egen projektspecifik kopia av mallens innehåll.
- När en egenkontroll ändras ska det inte förändra originalmallen.

## Egenkontroll

En egenkontroll är den projektspecifika kontroll som faktiskt genomförs.

Den skapas från en mall eller som en tom egenkontroll. När den är skapad tillhör den ett projekt eller arbetsuppdrag och innehåller de kontrollmoment och kontrollpunkter som ska bedömas.

En egenkontroll innehåller i praktiken:

- namn på egenkontrollen
- projektuppgifter
- beställare eller byggherre
- entreprenör
- referenser till krav, ritningar eller handlingar
- kontrollmoment
- kontrollpunkter
- resultat per kontrollpunkt
- kommentarer
- avvikelser och åtgärder vid behov
- bilagor eller foton vid behov
- signering
- granskning
- slutförande
- exporterbar rapport

### Praktisk betydelse

Egenkontrollen är arbetsytan där kontrollen utförs. Den ska kunna vara pågående över tid. Alla punkter behöver inte bedömas vid samma tillfälle.

En egenkontroll kan vara:

- utkast när den förbereds
- pågående när kontrollen utförs
- klar för granskning när punkterna är behandlade
- granskad när ansvarig person har bekräftat den
- slutförd när den är färdig som dokumentation

## Kontrollmoment

Ett kontrollmoment är en logisk grupp av kontrollpunkter.

Kontrollmoment motsvarar ofta en del av arbetet, en fas, ett område eller en typ av kontroll. Det hjälper användaren att förstå kontrollen i mindre delar.

Exempel på kontrollmoment:

- Förberedelser
- Underlag
- Material
- Utförande
- Montering
- Täthet
- Funktion
- Säkerhet
- Dokumentation
- Slutkontroll

### Praktisk betydelse

Kontrollmoment gör egenkontrollen lättare att använda på byggplatsen. I stället för en lång osorterad lista får användaren kontrollpunkter i ett begripligt sammanhang.

### Relationer

- En egenkontroll kan ha flera kontrollmoment.
- Ett kontrollmoment innehåller en eller flera kontrollpunkter.
- En kontrollpunkt kan höra till ett kontrollmoment.
- Kontrollmomentet ger struktur, men det är kontrollpunkten som bedöms.

## Kontrollpunkt

En kontrollpunkt är den minsta praktiska saken som ska kontrolleras.

Den ska vara konkret nog för att användaren ska kunna bedöma den och välja ett resultat.

En kontrollpunkt bör normalt innehålla:

- en kort kontrollformulering
- eventuell koppling till kontrollmoment
- resultat
- kommentar vid behov
- kontrollant
- datum
- eventuella bilagor eller foton
- eventuell avvikelse

### Resultat

Varje kontrollpunkt har ett aktuellt resultat:

- Ej bedömd: punkten är inte behandlad ännu.
- Godkänd: punkten är kontrollerad och uppfyller krav eller underlag.
- Ej godkänd: punkten är kontrollerad men uppfyller inte krav eller underlag.
- Ej kontrollerad: punkten kunde eller skulle inte kontrolleras.

### Praktisk betydelse

Kontrollpunkten är där själva arbetet dokumenteras. Om punkten är godkänd räcker det ofta med resultat, datum och kontrollant. Om punkten är ej godkänd eller ej kontrollerad behövs en förklaring.

### Relationer

- En egenkontroll innehåller flera kontrollpunkter.
- En kontrollpunkt kan tillhöra ett kontrollmoment.
- En kontrollpunkt bedöms av en kontrollant.
- En kontrollpunkt kan ha kommentar, foto, bilaga, avvikelse eller åtgärd.
- En kontrollpunkt kan bara ha ett aktuellt resultat åt gången.

## Dokument

Dokument är underlag, bevis eller resultat som hör till egenkontrollen.

I praktiken finns två typer av dokument:

- underlag som kontrollen görs mot
- dokumentation som kontrollen skapar

Underlag kan vara:

- ritning
- teknisk beskrivning
- kontrollplan
- arbetsberedning
- monteringsanvisning
- produktblad
- materialintyg
- beställarkrav

Dokumentation som skapas kan vara:

- ifylld egenkontroll
- sammanställning
- avvikelseunderlag
- signeringsuppgift
- granskningsuppgift
- PDF eller utskrift
- slutrapport

### Praktisk betydelse

Dokument gör egenkontrollen spårbar. Det ska gå att förstå vad kontrollen avsåg och vilket underlag som användes.

### Relationer

- Ett projekt kan ha flera dokument som referenser.
- En egenkontroll kan hänvisa till flera dokument.
- En kontrollpunkt kan vid behov hänvisa till ett särskilt dokument.
- Slutförandet skapar ett nytt dokument i form av rapport eller export.

## Bilaga

En bilaga är kompletterande material som stödjer en kontroll, kommentar, avvikelse eller åtgärd.

Bilagan är inte alltid nödvändig, men den kan ge viktig spårbarhet när text inte räcker.

Exempel på bilagor:

- produktblad
- materialintyg
- ritningsutdrag
- leverantörsanvisning
- kontrollprotokoll
- intyg
- kompletterande dokument

### Praktisk betydelse

Bilagor ska användas när de tillför bevis, förklaring eller underlag. De ska inte göra appen till ett fullständigt dokumenthanteringssystem.

### Relationer

- En bilaga kan höra till en egenkontroll som helhet.
- En bilaga kan höra till en specifik kontrollpunkt.
- En bilaga kan stödja en avvikelse eller åtgärd.
- En bilaga kan ingå i eller refereras från slutrapporten.

## Foto

Foto är en särskild typ av bilaga som visar hur något såg ut vid kontrolltillfället.

Foto kan användas för att dokumentera:

- utfört arbete
- brist eller skada
- dold installation innan inbyggnad
- material eller märkning
- platsförhållande
- åtgärdat fel

### Praktisk betydelse

Foto ger ofta högt värde i byggsammanhang eftersom många saker blir svåra att kontrollera i efterhand. Samtidigt ska foto inte ersätta tydlig kontrolltext eller ansvarig bedömning.

Ett foto bör i praktiken förstås tillsammans med:

- vilken kontrollpunkt det hör till
- när det togs
- vad det visar
- vem som tog eller lade till det
- eventuell kommentar

### Relationer

- Ett foto kan höra till en kontrollpunkt.
- Ett foto kan höra till en avvikelse.
- Ett foto kan höra till en åtgärd som bevis på att något är rättat.
- Ett foto kan visas eller refereras i slutrapporten.

## Signering

Signering är en bekräftelse av ansvar och tidpunkt.

I Egenkontroll App ska signering förstås som dokumenterad bekräftelse, inte som avancerad elektronisk signering eller BankID.

Det finns två huvudsakliga signeringsnivåer:

- kontrollantens markering på kontrollpunkt
- slutlig signering eller granskning av egenkontrollen

### Kontrollpunktens signering

När en kontrollpunkt bedöms bör det framgå:

- vem som kontrollerade
- när kontrollen gjordes
- vilket resultat som sattes

Detta ersätter den manuella signaturen per rad i en pappersblankett.

### Slutlig signering

När egenkontrollen är färdig bekräftar utförare eller ansvarig person att uppgifterna är korrekta.

Slutlig signering bör innehålla:

- namn
- datum och tid
- bekräftelse
- eventuell kommentar

### Granskning

Kontrollansvarig eller annan ansvarig person kan granska sammanställningen.

Granskning betyder att personen har läst igenom egenkontrollen, kontrollerat brister och bekräftat granskningen.

### Relationer

- En kontrollpunkt kan ha kontrollant och kontrolldatum.
- En egenkontroll kan signeras av utförare.
- En egenkontroll kan granskas av kontrollansvarig eller annan ansvarig.
- Signering hör till ansvar och spårbarhet.
- Signering ska inte dölja ej bedömda eller ej åtgärdade punkter.

## Avvikelse

En avvikelse är en noterad brist, skillnad eller händelse där något inte uppfyller krav, ritning, anvisning eller förväntat utförande.

I Egenkontroll App uppstår avvikelse praktiskt när en kontrollpunkt markeras som ej godkänd, eller när användaren beskriver en brist som behöver följas upp.

En avvikelse bör beskriva:

- vad som är fel
- var felet finns
- vilket krav eller underlag det avviker från
- när det upptäcktes
- vem som noterade det
- eventuell bilaga eller foto
- vilken åtgärd som behövs

### Praktisk betydelse

Avvikelsen ska göra bristen synlig och möjlig att följa upp. Den ska inte gömmas i övergripande anteckningar.

En enkel egenkontroll behöver inte bli ett fullständigt avvikelsesystem, men den ska kunna visa vilka punkter som kräver åtgärd eller förklaring.

### Relationer

- En avvikelse kan skapas från en kontrollpunkt.
- En avvikelse kan ha en eller flera bilagor eller foton.
- En avvikelse kan leda till en åtgärd.
- En avvikelse påverkar sammanställningen och slutförandet.

## Åtgärd

En åtgärd är det som görs för att hantera en avvikelse eller brist.

Åtgärden kan vara enkel, till exempel att komplettera, rätta, byta material, kontrollera igen eller invänta beslut.

En åtgärd bör beskriva:

- vad som ska göras
- vem som ansvarar
- när det ska vara klart eller när det blev klart
- eventuell kommentar
- eventuell foto- eller bilagebevisning
- om punkten behöver kontrolleras igen

### Praktisk betydelse

Åtgärder gör att egenkontrollen inte bara konstaterar fel utan stödjer uppföljning. Första versionen behöver inte ha avancerad ärendehantering, men användaren bör kunna förstå vad som händer med en ej godkänd punkt.

### Relationer

- En åtgärd hör normalt till en avvikelse.
- En åtgärd kan kopplas till en kontrollpunkt.
- En åtgärd kan dokumenteras med kommentar, bilaga eller foto.
- En åtgärd kan leda till att kontrollpunkten bedöms på nytt.
- Slutförande bör uppmärksamma öppna eller oklara åtgärder.

## Slutförande

Slutförande är när egenkontrollen går från pågående arbetsdokument till färdig dokumentation.

Slutförandet ska inte bara vara en knapp. Det är en kontroll av att egenkontrollen är begriplig, komplett och spårbar.

Innan slutförande bör användaren se:

- antal godkända punkter
- antal ej godkända punkter
- antal ej kontrollerade punkter
- antal ej bedömda punkter
- punkter som saknar obligatorisk kommentar
- avvikelser och åtgärder
- övriga anteckningar
- signering
- granskning
- vilka dokument, bilagor eller foton som ingår

### Praktisk betydelse

Slutförande gör egenkontrollen redo att sparas, exporteras, granskas eller lämnas vidare. En slutförd egenkontroll bör inte ändras utan att den återöppnas eller hanteras som ny version.

### Relationer

- En egenkontroll kan slutföras när nödvändig information är behandlad.
- Slutförande sammanfattar kontrollpunkter, avvikelser, åtgärder och signering.
- Slutförande skapar eller möjliggör slutrapport.
- Slutförande ska varna om något fortfarande är ej bedömt eller saknar förklaring.

## Konceptuell Relationsöversikt

### Projekt Till Egenkontroll

Ett projekt kan ha en eller flera egenkontroller. Varje egenkontroll behöver tillräcklig projektinformation för att kunna förstås i efterhand.

```text
Projekt
→ innehåller eller samlar
Egenkontroller
```

### Mall Till Egenkontroll

En mall är återanvändbar kunskap. En egenkontroll är den projektspecifika användningen av den kunskapen.

```text
Mall
→ används för att skapa
Egenkontroll
```

När egenkontrollen är skapad kan den anpassas utan att originalmallen ändras.

### Egenkontroll Till Kontrollmoment Och Kontrollpunkt

Egenkontrollen består av kontrollmoment och kontrollpunkter. Kontrollmoment grupperar. Kontrollpunkter bedöms.

```text
Egenkontroll
→ består av
Kontrollmoment
→ innehåller
Kontrollpunkter
```

### Kontrollpunkt Till Resultat

Varje kontrollpunkt har ett aktuellt resultat.

```text
Kontrollpunkt
→ bedöms som
Ej bedömd | Godkänd | Ej godkänd | Ej kontrollerad
```

### Kontrollpunkt Till Avvikelse Och Åtgärd

När en kontrollpunkt inte är godkänd kan den leda till avvikelse och åtgärd.

```text
Kontrollpunkt
→ kan ge
Avvikelse
→ kan kräva
Åtgärd
```

### Dokument, Bilaga Och Foto

Dokument kan vara underlag eller resultat. Bilagor och foton stödjer kontrollen med bevis eller förklaring.

```text
Dokument
→ används som underlag för
Egenkontroll eller Kontrollpunkt

Bilaga / Foto
→ stödjer
Kontrollpunkt, Avvikelse eller Åtgärd
```

### Signering Och Slutförande

Signering bekräftar ansvar. Slutförande gör egenkontrollen till färdig dokumentation.

```text
Egenkontroll
→ signeras och granskas
→ slutförs
→ exporteras som rapport
```

## Praktiskt Scenario

1. En arbetsledare skapar en egenkontroll för ett badrum i ett projekt.
2. Arbetsledaren väljer mallen Badrum.
3. Kontrollpunkter som inte gäller tas bort och projektspecifika punkter läggs till.
4. Referenser anges, till exempel ritning, tätskiktsanvisning och beställarkrav.
5. Utföraren kontrollerar punkterna under arbetets gång.
6. En punkt markeras som ej godkänd eftersom tätning saknas vid en genomföring.
7. En kommentar skrivs och ett foto läggs till.
8. Bristen blir en avvikelse som kräver åtgärd.
9. Åtgärden dokumenteras när tätningen är kompletterad.
10. Punkten kontrolleras igen och markeras som godkänd om den uppfyller kraven.
11. Egenkontrollen sammanställs.
12. Utföraren signerar att uppgifterna är korrekta.
13. Kontrollansvarig eller ansvarig person granskar.
14. Egenkontrollen slutförs och exporteras som rapport.

## Avgränsning

Domänmodellen beskriver endast Egenkontroll App.

Den beskriver inte:

- databastabeller
- SQL
- API:er
- implementation
- filuppladdningsteknik
- behörighetssystem
- betalning
- abonnemang
- komplett dokumenthantering
- fullständigt avvikelsesystem
- avancerad e-signering

Dessa frågor kan beslutas senare. Domänmodellen ska först och främst hjälpa projektet att förstå vad en egenkontroll är, hur arbetet sker i praktiken och vilka begrepp som måste vara tydliga för användaren.
