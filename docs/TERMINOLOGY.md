# TERMINOLOGY

## Syfte

Detta är byggbranschens ordlista för **Egenkontroll App**.

Ordlistan ska hjälpa appen att använda samma språk överallt: i knappar, hjälptexter, tooltips, felmeddelanden, rapporter och framtida översättningar.

Språket ska vara vardagssvenska för små och medelstora byggföretag. Undvik ISO-jargong, myndighetssvenska och onödigt svåra systemord.

## Språkprinciper

- Skriv kort och konkret.
- Använd ord som byggföretag redan känner igen.
- Förklara svårare ord nära där de används.
- Använd hellre "kontroll" än "verifiering".
- Använd hellre "klar" än "färdigställd" när det passar i appflödet.
- Använd hellre "skriv kommentar" än "ange avvikelseorsak".
- Säg inte mer juridiskt än appen faktiskt stödjer.

## Termlista

### Projekt

**Rekommenderad term:** Projekt

**Enkel förklaring:** Det jobb, bygge, arbetsplats eller uppdrag som egenkontrollen hör till.

**Undvik detta:** Objekt, ärende, case, uppdragsenhet, verksamhetskontext.

**Exempel på apptext:** "Välj projekt" eller "Ange vilket projekt egenkontrollen gäller."

**När används:** När användaren ska koppla egenkontrollen till rätt jobb, plats eller kund.

**När används inte:** Använd inte om det bara handlar om själva kontrollmallen eller en enskild kontrollpunkt.

**Kommentar:** Projekt kan vara stort eller litet. Det kan vara ett helt bygge, ett rum, en etapp eller ett avgränsat arbete.

**Framtida översättning:** EN: Project.

### Arbetsplats

**Rekommenderad term:** Arbetsplats

**Enkel förklaring:** Den fysiska plats där arbetet utförs.

**Undvik detta:** Lokalisering, site location, produktionsställe.

**Exempel på apptext:** "Arbetsplats: Hus B, plan 2"

**När används:** När platsen behöver vara tydlig i rapporten eller vid flera platser i samma projekt.

**När används inte:** Använd inte som ersättning för projekt om projektet även behöver kund, beställare och referenser.

**Kommentar:** Arbetsplats är ofta enklare än projektplats i apptext.

**Framtida översättning:** EN: Work site.

### Mall

**Rekommenderad term:** Mall

**Enkel förklaring:** En färdig startlista med kontrollpunkter för en viss typ av arbete.

**Undvik detta:** Template i svensk text, formulärmall, datamall, standardiserad kontrollstruktur.

**Exempel på apptext:** "Välj mall" eller "Utgå från mallen Badrum."

**När används:** När användaren ska skapa en ny egenkontroll från färdigt innehåll.

**När används inte:** Använd inte om den redan skapade, projektspecifika egenkontrollen.

**Kommentar:** En mall är inte låst. Användaren ska kunna anpassa den till projektet.

**Framtida översättning:** EN: Template.

### Tom mall

**Rekommenderad term:** Tom mall

**Enkel förklaring:** En egenkontroll utan färdiga kontrollpunkter, där användaren bygger listan själv.

**Undvik detta:** Blankett, tomt schema, custom template, fri kontroll.

**Exempel på apptext:** "Skapa från tom mall"

**När används:** När ingen färdig mall passar arbetet.

**När används inte:** Använd inte för vanliga mallar som redan innehåller kontrollpunkter.

**Kommentar:** Tom mall ska kännas enkel, inte teknisk.

**Framtida översättning:** EN: Blank template.

### Egenkontroll

**Rekommenderad term:** Egenkontroll

**Enkel förklaring:** En dokumenterad kontroll av att arbetet är utfört enligt krav, ritning eller annan handling.

**Undvik detta:** Inspektion om svensk byggterm räcker, audit, verifieringsaktivitet, kontrollärende.

**Exempel på apptext:** "Skapa ny egenkontroll" eller "Fortsätt egenkontroll."

**När används:** Som huvudnamn för det arbete användaren skapar, fyller i, signerar och exporterar.

**När används inte:** Använd inte för en enskild kontrollpunkt. En egenkontroll innehåller flera delar.

**Kommentar:** Detta är appens viktigaste ord. Använd konsekvent.

**Framtida översättning:** EN: Self-check eller Self-inspection. Välj senare efter målmarknad.

### Kontroll

**Rekommenderad term:** Kontroll

**Enkel förklaring:** Själva handlingen att titta, mäta, jämföra eller bedöma något.

**Undvik detta:** Verifiering, validering, revision, assessment.

**Exempel på apptext:** "Starta kontroll" eller "Kontrollen är inte klar."

**När används:** När appen beskriver att användaren ska utföra eller fortsätta kontrollarbetet.

**När används inte:** Använd inte om hela dokumentet när "egenkontroll" är tydligare.

**Kommentar:** Kontroll är vardagligt och fungerar bra i knappar och korta texter.

**Framtida översättning:** EN: Check eller Inspection.

### Kontrollmoment

**Rekommenderad term:** Kontrollmoment

**Enkel förklaring:** En grupp av kontrollpunkter som hör till samma del av arbetet.

**Undvik detta:** Sektion om byggord behövs, kategori, processdel, kontrollområde.

**Exempel på apptext:** "Kontrollmoment: Underlag"

**När används:** När kontrollpunkter behöver grupperas, till exempel Underlag, Material, Utförande eller Slutkontroll.

**När används inte:** Använd inte för den enskilda punkten som ska bedömas.

**Kommentar:** I mycket enkla vyer kan "Grupp" vara tydligare än "Kontrollmoment".

**Framtida översättning:** EN: Check section eller Inspection section.

### Kontrollpunkt

**Rekommenderad term:** Kontrollpunkt

**Enkel förklaring:** En sak i egenkontrollen som ska kontrolleras och få ett resultat.

**Undvik detta:** Fråga, rad, post, objekt, requirement item.

**Exempel på apptext:** "Lägg till kontrollpunkt" eller "Kommentar krävs för denna kontrollpunkt."

**När används:** När användaren bedömer, ändrar, lägger till eller tar bort en punkt.

**När används inte:** Använd inte för hela egenkontrollen eller för ett kontrollmoment.

**Kommentar:** Kontrollpunkt ska vara konkret och kort formulerad.

**Framtida översättning:** EN: Checkpoint.

### Resultat

**Rekommenderad term:** Resultat

**Enkel förklaring:** Det användaren väljer efter att en kontrollpunkt har bedömts.

**Undvik detta:** Status om det gäller själva bedömningen, utfall, klassning, bedömningsvärde.

**Exempel på apptext:** "Välj resultat" eller "Resultat saknas."

**När används:** För valen Godkänd, Ej godkänd, Ej kontrollerad och Ej bedömd.

**När används inte:** Använd inte för sammanställningar, diagram eller rapportresultat om det kan missförstås.

**Kommentar:** Status kan användas för hela egenkontrollen. Resultat passar bäst per kontrollpunkt.

**Framtida översättning:** EN: Result.

### Ej bedömd

**Rekommenderad term:** Ej bedömd

**Enkel förklaring:** Punkten är inte kontrollerad än.

**Undvik detta:** Obesvarad, ej hanterad, pending, okänd.

**Exempel på apptext:** "3 kontrollpunkter är ej bedömda."

**När används:** För punkter som återstår under pågående arbete.

**När används inte:** Använd inte som slutresultat utan att varna användaren.

**Kommentar:** Ej bedömd är ett arbetsläge. Det betyder inte att punkten är fel.

**Framtida översättning:** EN: Not assessed.

### Godkänd

**Rekommenderad term:** Godkänd

**Enkel förklaring:** Punkten är kontrollerad och ser rätt ut mot krav eller underlag.

**Undvik detta:** OK som huvudterm, passerad, accepterad, compliant.

**Exempel på apptext:** "Markera som godkänd"

**När används:** När kontrollpunkten uppfyller det den ska kontrolleras mot.

**När används inte:** Använd inte innan punkten faktiskt är kontrollerad.

**Kommentar:** Det går bra att använda grön färg, men texten Godkänd måste alltid synas.

**Framtida översättning:** EN: Approved eller Passed.

### Ej godkänd

**Rekommenderad term:** Ej godkänd

**Enkel förklaring:** Punkten är kontrollerad men något stämmer inte.

**Undvik detta:** Underkänd om tonen blir för hård, non-conformity, fail, avvikande kravuppfyllnad.

**Exempel på apptext:** "Kommentar krävs när en punkt är ej godkänd."

**När används:** När brist, fel eller avvikelse har upptäckts.

**När används inte:** Använd inte när punkten inte har kunnat kontrolleras. Då används Ej kontrollerad.

**Kommentar:** Ej godkänd ska alltid leda till kommentar och ofta till åtgärd.

**Framtida översättning:** EN: Not approved eller Failed.

### Ej kontrollerad

**Rekommenderad term:** Ej kontrollerad

**Enkel förklaring:** Punkten har inte kontrollerats, eller kunde inte kontrolleras.

**Undvik detta:** Ej tillämplig om det inte är säkert, okontrollerad, skipped, not applicable som standard.

**Exempel på apptext:** "Skriv varför punkten inte har kontrollerats."

**När används:** När kontrollen inte kan göras, inte ingår eller måste skjutas upp.

**När används inte:** Använd inte för fel som faktiskt har upptäckts. Då används Ej godkänd.

**Kommentar:** Orsak ska alltid anges så att rapporten går att förstå i efterhand.

**Framtida översättning:** EN: Not checked.

### Kommentar

**Rekommenderad term:** Kommentar

**Enkel förklaring:** En kort förklaring till resultatet eller något användaren vill notera.

**Undvik detta:** Notering om det skapar otydlighet, fritextfält, avvikelsebeskrivning i alla lägen.

**Exempel på apptext:** "Skriv kommentar"

**När används:** När en punkt är ej godkänd, ej kontrollerad eller när användaren vill förklara något.

**När används inte:** Använd inte som ersättning för tydliga resultatval.

**Kommentar:** Kommentarer ska helst ligga på rätt kontrollpunkt, inte bara i övriga anteckningar.

**Framtida översättning:** EN: Comment.

### Övriga anteckningar

**Rekommenderad term:** Övriga anteckningar

**Enkel förklaring:** Samlad text som gäller hela egenkontrollen.

**Undvik detta:** Generella kommentarer, fri text, sammanfattande avvikelseinformation.

**Exempel på apptext:** "Lägg till övriga anteckningar"

**När används:** För information som gäller hela kontrollen, till exempel etapp, omfattning eller övergripande förklaring.

**När används inte:** Använd inte för brister som hör till en specifik kontrollpunkt.

**Kommentar:** Appen bör hjälpa användaren att skriva punktkommentarer på rätt plats.

**Framtida översättning:** EN: Additional notes.

### Referens

**Rekommenderad term:** Referens

**Enkel förklaring:** Det underlag kontrollen görs mot, till exempel ritning, krav eller anvisning.

**Undvik detta:** Hänvisning om det blir tungt, dokumentrelation, styrande dokument.

**Exempel på apptext:** "Lägg till referens" eller "Ritning A-40.1-101, rev B"

**När används:** När användaren ska ange vilket underlag som gäller för kontrollen.

**När används inte:** Använd inte för bilagor som bara är bevis eller foton efter utfört arbete.

**Kommentar:** Referens kan vara en ritning, teknisk beskrivning, monteringsanvisning eller beställarkrav.

**Framtida översättning:** EN: Reference.

### Dokument

**Rekommenderad term:** Dokument

**Enkel förklaring:** En fil eller handling som hör till projektet, kontrollen eller rapporten.

**Undvik detta:** Artefakt, resurs, filobjekt, document entity.

**Exempel på apptext:** "Lägg till dokument" eller "Dokument som kontrollen gäller"

**När används:** För ritningar, beskrivningar, produktblad, materialintyg, rapporter och liknande.

**När används inte:** Använd inte när det egentligen handlar om ett foto eller en enkel kommentar.

**Kommentar:** Dokument kan vara både underlag och slutresultat. Förtydliga vid behov.

**Framtida översättning:** EN: Document.

### Bilaga

**Rekommenderad term:** Bilaga

**Enkel förklaring:** Extra material som stödjer en kontrollpunkt, avvikelse eller åtgärd.

**Undvik detta:** Attachment i svensk text, filbilaga om "bilaga" räcker, bevismaterial som standardterm.

**Exempel på apptext:** "Lägg till bilaga"

**När används:** När användaren vill lägga till produktblad, intyg, ritningsutdrag eller annat stödmaterial.

**När används inte:** Använd inte som huvudterm för alla dokument i projektet.

**Kommentar:** Bilagor ska ge stöd, inte göra appen till ett stort dokumentarkiv.

**Framtida översättning:** EN: Attachment.

### Foto

**Rekommenderad term:** Foto

**Enkel förklaring:** En bild som visar arbetet, en brist eller en åtgärd.

**Undvik detta:** Bildbevis, fotodokumentationsobjekt, mediafil.

**Exempel på apptext:** "Lägg till foto"

**När används:** När en bild gör kontrollen tydligare, till exempel före inbyggnad eller vid brist.

**När används inte:** Använd inte som ersättning för resultat, kommentar eller ansvarig bedömning.

**Kommentar:** Foto är en typ av bilaga, men ordet Foto är enklare i appen.

**Framtida översättning:** EN: Photo.

### Avvikelse

**Rekommenderad term:** Avvikelse

**Enkel förklaring:** Något som inte stämmer med krav, ritning, anvisning eller förväntat utförande.

**Undvik detta:** Non-conformity, NCR, bristärende, kvalitetsavvikelse om det blir för tungt.

**Exempel på apptext:** "Avvikelse skapad från ej godkänd punkt"

**När används:** När en kontrollpunkt är ej godkänd och behöver följas upp.

**När används inte:** Använd inte för punkter som bara inte har kontrollerats. Där räcker ofta kommentar om orsaken.

**Kommentar:** I enklare flöden kan appen prata om "brist" i hjälptext, men Avvikelse är rätt term i rapport och sammanställning.

**Framtida översättning:** EN: Deviation eller Issue. Välj senare efter produktens ton.

### Brist

**Rekommenderad term:** Brist

**Enkel förklaring:** Något som saknas, är fel eller behöver rättas.

**Undvik detta:** Defekt, felaktighet, non-conformance.

**Exempel på apptext:** "Beskriv bristen"

**När används:** I enkel apptext när användaren ska beskriva vad som är fel.

**När används inte:** Använd inte som ersättning för Avvikelse i rapportdelar där spårbarhet behövs.

**Kommentar:** Brist är ofta mer vardagligt än Avvikelse och passar bra nära kommentarfält.

**Framtida översättning:** EN: Defect eller Issue.

### Åtgärd

**Rekommenderad term:** Åtgärd

**Enkel förklaring:** Det som ska göras, eller har gjorts, för att rätta en brist.

**Undvik detta:** Korrigerande åtgärd, corrective action, aktivitetspost, remedy.

**Exempel på apptext:** "Lägg till åtgärd" eller "Beskriv vad som ska åtgärdas."

**När används:** När en ej godkänd punkt eller avvikelse behöver följas upp.

**När används inte:** Använd inte för vanliga kommentarer som inte kräver något arbete.

**Kommentar:** Håll åtgärd enkel i första versionen. Det behöver inte bli ett avancerat ärendesystem.

**Framtida översättning:** EN: Action.

### Kontrollant

**Rekommenderad term:** Kontrollant

**Enkel förklaring:** Personen som har kontrollerat en punkt.

**Undvik detta:** Inspektör om det låter för formellt, verifierare, utförare om det är oklart.

**Exempel på apptext:** "Kontrollerad av"

**När används:** Vid kontrollpunktens resultat, datum och spårbarhet.

**När används inte:** Använd inte automatiskt för den som signerar hela egenkontrollen om det är en annan roll.

**Kommentar:** I fältetiketter kan "Kontrollerad av" vara tydligare än "Kontrollant".

**Framtida översättning:** EN: Checked by eller Inspector.

### Utförare

**Rekommenderad term:** Utförare

**Enkel förklaring:** Personen eller företaget som har gjort arbetet.

**Undvik detta:** Resurs, operatör, producerande part.

**Exempel på apptext:** "Utfört av"

**När används:** Vid slutlig bekräftelse av vem som står bakom utfört arbete eller ifylld egenkontroll.

**När används inte:** Använd inte om beställare, byggherre eller granskare.

**Kommentar:** Utförare och kontrollant kan vara samma person, men behöver inte vara det.

**Framtida översättning:** EN: Performed by.

### Granskare

**Rekommenderad term:** Granskare

**Enkel förklaring:** Personen som läser igenom och bekräftar egenkontrollen.

**Undvik detta:** Reviewer i svensk text, godkännare om appen inte formellt godkänner, revisor.

**Exempel på apptext:** "Granskad av"

**När används:** När någon kontrollerar sammanställningen efter att egenkontrollen är ifylld.

**När används inte:** Använd inte för personen som bedömer varje kontrollpunkt under arbetet.

**Kommentar:** Granskare är enklare än kontrollansvarig i många små byggföretag.

**Framtida översättning:** EN: Reviewer.

### Kontrollansvarig

**Rekommenderad term:** Kontrollansvarig

**Enkel förklaring:** En ansvarig person som granskar eller följer upp egenkontrollen.

**Undvik detta:** KA som enda term, certifierad roll om appen inte faktiskt hanterar den rollen, myndighetsgodkännare.

**Exempel på apptext:** "Kontrollansvarig / granskare"

**När används:** När kunden eller projektet uttryckligen använder rollen kontrollansvarig.

**När används inte:** Använd inte om alla användare. Många små jobb har bara en ansvarig granskare.

**Kommentar:** Var tydlig med att appens granskning inte är avancerad e-signering eller myndighetsbeslut.

**Framtida översättning:** EN: Quality controller eller Responsible inspector. Kräver senare språkbeslut.

### Beställare

**Rekommenderad term:** Beställare

**Enkel förklaring:** Den som beställt arbetet.

**Undvik detta:** Kund om avtalsrollen behöver vara tydlig, uppdragsgivare om det blir för formellt.

**Exempel på apptext:** "Beställare"

**När används:** När egenkontrollen ska visa vem arbetet görs åt.

**När används inte:** Använd inte när projektet kräver ordet Byggherre.

**Kommentar:** För många småföretag är Beställare det mest begripliga ordet.

**Framtida översättning:** EN: Client.

### Byggherre

**Rekommenderad term:** Byggherre

**Enkel förklaring:** Den som låter utföra byggarbetet.

**Undvik detta:** Byggkund, projektägare, developer utan förklaring.

**Exempel på apptext:** "Beställare / byggherre"

**När används:** När byggprojektet eller dokumentationen behöver den byggbranschspecifika rollen.

**När används inte:** Använd inte om Beställare är tillräckligt och användaren inte behöver den särskilda rollen.

**Kommentar:** Byggherre är korrekt byggterm men kan behöva kort hjälptext i appen.

**Framtida översättning:** EN: Client eller Developer, beroende på sammanhang.

### Entreprenör

**Rekommenderad term:** Entreprenör

**Enkel förklaring:** Företaget som utför eller ansvarar för arbetet.

**Undvik detta:** Leverantör om det gäller utförande, contractor i svensk text, utförande part.

**Exempel på apptext:** "Ange entreprenör"

**När används:** För företaget eller parten som står för arbetet i egenkontrollen.

**När används inte:** Använd inte för beställare eller ren materialleverantör.

**Kommentar:** Entreprenör kan vara huvudentreprenör eller underentreprenör beroende på projekt.

**Framtida översättning:** EN: Contractor.

### Underentreprenör

**Rekommenderad term:** Underentreprenör

**Enkel förklaring:** Ett företag som gör en del av arbetet åt en annan entreprenör.

**Undvik detta:** UE som enda term, subcontractor i svensk text.

**Exempel på apptext:** "Underentreprenör, om det gäller"

**När används:** När det är viktigt att visa vem som faktiskt utfört ett visst moment.

**När används inte:** Använd inte om det bara finns en entreprenör i uppdraget.

**Kommentar:** Kan vara frivilligt fält i enkel version.

**Framtida översättning:** EN: Subcontractor.

### Signering

**Rekommenderad term:** Signering

**Enkel förklaring:** En bekräftelse med namn och tidpunkt.

**Undvik detta:** Elektronisk signatur, BankID-signering, kvalificerad signatur, digital legal signering.

**Exempel på apptext:** "Signera egenkontroll"

**När används:** När användaren bekräftar att uppgifterna är korrekta eller att granskning är gjord.

**När används inte:** Använd inte om appen bara sparar ett utkast eller en kommentar.

**Kommentar:** Appen ska vara tydlig med att signering här betyder enkel bekräftelse, inte avancerad e-signering.

**Framtida översättning:** EN: Sign-off.

### Bekräfta

**Rekommenderad term:** Bekräfta

**Enkel förklaring:** Att säga att uppgiften stämmer eller är genomförd.

**Undvik detta:** Attestera, certifiera, validera, verifiera.

**Exempel på apptext:** "Jag bekräftar att uppgifterna är korrekta."

**När används:** Vid signering, granskning eller avslutande steg.

**När används inte:** Använd inte när användaren bara navigerar vidare utan ansvar.

**Kommentar:** Bekräfta är ofta mjukare och tydligare än signera i hjälptexter.

**Framtida översättning:** EN: Confirm.

### Granskning

**Rekommenderad term:** Granskning

**Enkel förklaring:** Att läsa igenom egenkontrollen och kontrollera att den är rimlig och komplett.

**Undvik detta:** Revision, audit, formellt godkännande, myndighetsgranskning.

**Exempel på apptext:** "Skicka till granskning" eller "Markera som granskad"

**När används:** När någon ansvarig kontrollerar sammanställningen efter utförd egenkontroll.

**När används inte:** Använd inte för varje vanlig kontrollpunkt om "kontroll" räcker.

**Kommentar:** Granskning ska inte låta större än den är.

**Framtida översättning:** EN: Review.

### Slutförande

**Rekommenderad term:** Slutförande

**Enkel förklaring:** När egenkontrollen görs klar som färdig dokumentation.

**Undvik detta:** Stängning, arkivering, finalisering om det låter tekniskt, färdigställande om enklare ord räcker.

**Exempel på apptext:** "Slutför egenkontroll"

**När används:** När användaren går från pågående arbete till färdig rapport.

**När används inte:** Använd inte när användaren bara sparar ett utkast.

**Kommentar:** Innan slutförande ska appen varna om punkter saknar bedömning eller kommentar.

**Framtida översättning:** EN: Completion.

### Slutrapport

**Rekommenderad term:** Slutrapport

**Enkel förklaring:** Den färdiga rapporten av egenkontrollen.

**Undvik detta:** Exportartefakt, slutdokumentation om enklare ord räcker, rapportpaket.

**Exempel på apptext:** "Skapa slutrapport"

**När används:** När egenkontrollen är slutförd och ska sparas, skrivas ut eller skickas vidare.

**När används inte:** Använd inte för själva arbetsvyn där kontrollen fylls i.

**Kommentar:** Slutrapport ska kännas som ett professionellt byggdokument.

**Framtida översättning:** EN: Final report.

### PDF

**Rekommenderad term:** PDF

**Enkel förklaring:** En fil som går att spara, skriva ut eller skicka vidare.

**Undvik detta:** Exportformat som huvudtext, dokumentrendering, utskriftsartefakt.

**Exempel på apptext:** "Exportera PDF"

**När används:** När användaren vill skapa en delbar rapport.

**När används inte:** Använd inte som namn på hela egenkontrollen.

**Kommentar:** PDF är välkänt och behöver normalt ingen förklaring.

**Framtida översättning:** EN: PDF.

### Utkast

**Rekommenderad term:** Utkast

**Enkel förklaring:** En egenkontroll som är påbörjad men inte startad eller klar.

**Undvik detta:** Draft i svensk text, preliminär status, förberedelseläge.

**Exempel på apptext:** "Spara som utkast"

**När används:** När projektuppgifter eller kontrollpunkter förbereds.

**När används inte:** Använd inte för kontroller som redan är aktivt under genomförande om "Pågående" är tydligare.

**Kommentar:** Utkast ska kännas tryggt: användaren kan fortsätta senare.

**Framtida översättning:** EN: Draft.

### Pågående

**Rekommenderad term:** Pågående

**Enkel förklaring:** Egenkontrollen är startad men inte klar.

**Undvik detta:** Aktiv, öppen, in progress i svensk text.

**Exempel på apptext:** "Pågående egenkontroller"

**När används:** För egenkontroller som användaren håller på att fylla i.

**När används inte:** Använd inte för mallar eller slutförda rapporter.

**Kommentar:** Pågående är tydligt på startsidan.

**Framtida översättning:** EN: In progress.

### Klar för granskning

**Rekommenderad term:** Klar för granskning

**Enkel förklaring:** Egenkontrollen är ifylld och kan läsas igenom av ansvarig person.

**Undvik detta:** Ready for review i svensk text, granskningsbar, godkännandeklar.

**Exempel på apptext:** "Markera som klar för granskning"

**När används:** När kontrollpunkterna är behandlade men slutlig granskning återstår.

**När används inte:** Använd inte om egenkontrollen fortfarande har punkter utan bedömning och utan förklaring.

**Kommentar:** Detta steg kan vara valfritt i enkel version.

**Framtida översättning:** EN: Ready for review.

### Granskad

**Rekommenderad term:** Granskad

**Enkel förklaring:** En ansvarig person har läst igenom och bekräftat egenkontrollen.

**Undvik detta:** Godkänd om det kan misstolkas juridiskt, approved by authority, reviderad.

**Exempel på apptext:** "Granskad av Anna Andersson"

**När används:** Efter att granskare eller kontrollansvarig har bekräftat sammanställningen.

**När används inte:** Använd inte för en kontrollpunkt som bara är godkänd.

**Kommentar:** Skilj på kontrollpunktens resultat Godkänd och egenkontrollens status Granskad.

**Framtida översättning:** EN: Reviewed.

### Slutförd

**Rekommenderad term:** Slutförd

**Enkel förklaring:** Egenkontrollen är klar och bör inte ändras utan särskilt beslut.

**Undvik detta:** Stängd, låst, arkiverad om de orden inte exakt stämmer.

**Exempel på apptext:** "Slutförd egenkontroll"

**När används:** När kontrollen är klar, signerad eller redo som rapport.

**När används inte:** Använd inte medan punkter fortfarande ska kontrolleras.

**Kommentar:** Slutförd är statusen. Slutförande är handlingen.

**Framtida översättning:** EN: Completed.

### Arkiverad

**Rekommenderad term:** Arkiverad

**Enkel förklaring:** Egenkontrollen är sparad för historik och används inte aktivt.

**Undvik detta:** Borttagen, stängd, inaktiv om det kan misstolkas.

**Exempel på apptext:** "Visa arkiverade egenkontroller"

**När används:** När gamla egenkontroller ska finnas kvar men inte ligga bland pågående arbete.

**När används inte:** Använd inte som samma sak som slutförd. En slutförd kontroll behöver inte vara arkiverad.

**Kommentar:** Kan vänta till senare version om appen hålls enkel.

**Framtida översättning:** EN: Archived.

## Rekommenderade Ordval I Appen

Använd:

- Skapa ny egenkontroll
- Välj mall
- Fyll i projektinformation
- Anpassa kontrollpunkter
- Starta kontroll
- Lägg till kontrollpunkt
- Markera som godkänd
- Skriv kommentar
- Lägg till foto
- Lägg till bilaga
- Beskriv bristen
- Lägg till åtgärd
- Granska sammanställning
- Signera egenkontroll
- Markera som granskad
- Slutför egenkontroll
- Exportera PDF
- Skriv ut rapport

Undvik:

- Initiera kontrollprocess
- Validera kontrollobjekt
- Hantera non-conformity
- Exekvera åtgärdsflöde
- Finalisera dokumentartefakt
- Utför compliance review
- Administrera kvalitetsmodul

## Översättningsförberedelse

Framtida översättning ska inte göras ord för ord utan utifrån hur byggföretag i målmarknaden faktiskt pratar.

Särskilt viktiga termer att besluta separat vid översättning:

- Egenkontroll
- Kontrollpunkt
- Kontrollmoment
- Kontrollansvarig
- Avvikelse
- Signering
- Slutrapport

Svenska originaltermer ska vara styrande tills en målmarknad och engelsk produktton är beslutad.
