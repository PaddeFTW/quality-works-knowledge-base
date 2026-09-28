# Information och bevis per fråga

**Version:** 1.0  
**Syfte:** Underlag till fälten `information_finns_hos` och `vanliga_bevis` i ISO Quiz.  
**Källa:** Befintlig frågebank (`10`) plus beviskolumnen i `01`–`04`. Inga nya ISO-krav.  
**Målgrupp:** Små och medelstora företag.

---

## Så här fungerar det i verkligheten

I företag med 1–5 anställda sitter nästan all kunskap hos VD eller ägaren. Det betyder inte att VD har papper på allt. Det betyder att VD kan *börja* svaret.

I företag med 6–20 anställda börjar kunskapen delas: arbetsledare vet hur jobbet görs, administratör vet lön och avtal, den som säljer vet vad kunden klagar på.

I företag med 21–50 anställda finns ofta namngivna roller, men sällan en ISO-avdelning.

Revisorer frågar inte efter ISO-ord. De frågar:

- Hur gör ni det?
- Kan ni visa det?
- Gör ni så varje gång?

Därför är bevisen nedan vanliga saker som redan nämns i kunskapsbanken: listor, policy med underskrift, protokoll, rutiner, mätdata, avtal.

---

## Fält som ska in i varje fråga

```text
information_finns_hos: []
vanliga_bevis: []
vd_kan_svara_direkt: ja | delvis | nej
var_informationen_finns: []
```

**Betydelse**

- `vd_kan_svara_direkt: ja` – VD i ett småföretag kan normalt ge ett användbart svar utan att fråga någon annan.
- `delvis` – VD kan ge en grov bild, men någon annan behövs för att svaret ska bli revisionsbart.
- `nej` – någon annan har den praktiska kunskapen.

Även när VD kan svara ska fältet `information_finns_hos` visas. Det hjälper om VD är osäker.

---

## Roller som används i fälten

Använd dessa namn, inte ISO-titlar:

- VD / ägare
- Platschef / arbetsledare
- Administratör
- Ekonomi / lön
- Säljare / kundansvarig
- Projektledare
- Skyddsombud
- Den som gör jobbet
- IT-ansvarig eller IT-leverantör
- Inköpsansvarig
- HR (ofta samma person som administratör eller VD)

Visa 2–4 roller per fråga. Inte en lång lista.

---

## 1. Frågor som VD normalt kan svara på direkt

Gäller särskilt 1–20 anställda.

| ID | Fråga i korthet | Varför VD kan svara |
|----|-----------------|---------------------|
| A1 | Vad företaget gör och vad som ska ingå | Det är VD:s verksamhetsbeskrivning |
| A2 | Vad som påverkar utifrån | VD lever med kunder, priser, lagar och personalbrist |
| A3 | Vem som ställer krav | VD känner kund, personal, myndighet och ägare |
| B1 | Kvalitetslöfte | VD skriver under |
| B2 | Miljölöfte | VD skriver under |
| B3 | Säkerhetslöfte | VD skriver under |
| B4 | Informationslöfte | VD skriver under |
| B5 | Vem som gör vad | I små bolag är rollerna få och kända av VD |
| C6 | Enkla mål | VD sätter målen |
| F6 | Chefens årliga möte | Det är VD:s möte |

**Begränsning:** VD kan svara *att* något finns eller *hur det ungefär går till*. Beviset ligger ofta hos administratör eller i en pärm.

---

## 2. Frågor som normalt kräver information från andra

| ID | Fråga i korthet | Först fråga | VD:s roll |
|----|-----------------|-------------|-----------|
| A4 | Vilken information som ska skyddas | IT-ansvarig / administratör | Godkänner omfattningen |
| B6 | Personalens medverkan | Skyddsombud, arbetsledare | Vet om möten finns |
| C1 | Vad som kan gå fel i jobbet | Arbetsledare, säljare, den som gör jobbet | Känner de stora riskerna |
| C2 | Vad som påverkar miljön | Arbetsledare, den som kör / städar / producerar | Vet avfall och bilar på övergripande nivå |
| C3 | Faror för personalen | Skyddsombud, arbetsledare, den som gör jobbet | Vet allvarliga händelser |
| C4 | Informationsrisker | IT-ansvarig / IT-leverantör | Vet att “datorer och mejl finns” |
| C5 | Vilka lagar som gäller | Administratör, ekonomi, skyddsombud | Känner de stora lagarna |
| D1 | Vad varje person kan | Arbetsledare, administratör / HR | Känner personalen, inte kurslistan |
| D2 | Introduktion | Arbetsledare, handledare | Vet att “de går bredvid” |
| D3 | Om personalen sett löftena | Administratör, arbetsledare | Tror att alla sett policyn |
| D4 | Utrustning, skydd, IT | Arbetsledare, inköp, IT-leverantör | Vet att grejer finns |
| D5 | Rätt version av dokument | Administratör | Sällan VD som håller i mallarna |
| D6 | Konton och inloggning | IT-ansvarig / administratör | Godkänner att konton ska stängas |
| E1 | Hur en order tas emot | Säljare / kundansvarig | Ofta VD i 1–5 bolag |
| E2 | Hur jobbet utförs | Den som gör jobbet, arbetsledare | VD beskriver grovt |
| E3 | Inköp och leverantörer | Inköpsansvarig, administratör | VD godkänner stora köp |
| E4 | Avfall och kemikalier | Arbetsledare, den som gör jobbet | Vet att sortering “finns” |
| E5 | Plan när något går riktigt fel | Skyddsombud, arbetsledare, IT-leverantör | Godkänner planen |
| E6 | Information i vardagen | IT-ansvarig / administratör | Sätter reglerna |
| F1 | Vad kunderna tycker | Säljare, kundansvarig, projektledare | Pratar med några kunder |
| F2 | Betyg på leverantörer | Inköp, arbetsledare, administratör | Känner de stora leverantörerna |
| F3 | Uppföljning av mål | Administratör / ekonomi | Vill se siffrorna |
| F4 | Genomgång av lagar | Administratör, skyddsombud | Beställer genomgången |
| F5 | Intern genomgång av systemet | Den som utsetts, ofta administratör eller extern hjälp | Beställer genomgången |
| G1 | Att fel skrivs upp | Den som gör jobbet, arbetsledare | Ser de stora felen |
| G2 | Att orsaken åtgärdas | Arbetsledare, den som utreder | Beslutar åtgärd |
| G3 | Förbättringsförslag | Personalen, arbetsledare | Tar upp förslagen |

---

## 3–5. Fråga för fråga

Varje post är redo att kopieras in i frågebanken.

### A1. Vad gör företaget?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare
- **var_informationen_finns:** Huvudet på VD, hemsidan, anbud, Bolagsverket, kundavtal
- **vanliga_bevis:** Kort verksamhetsbeskrivning, manualens inledning, hemsida, offertmall
- **källa_bevis:** Q9/Q14/Q45/Q27-4.3, A1

### A2. Vad påverkar oss utifrån?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare, platschef / arbetsledare
- **var_informationen_finns:** Ledningsmöten, kundkrav i avtal, nyheter i branschen, priser från leverantör
- **vanliga_bevis:** Kort lista över yttre påverkan, SWOT om sådan finns, mötesanteckningar
- **källa_bevis:** Q9/Q14/Q45/Q27-4.1

### A3. Vem bryr sig om oss?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare, säljare / kundansvarig
- **var_informationen_finns:** Kundlista, anställningsavtal, myndighetspost, leverantörsavtal
- **vanliga_bevis:** Intressentlista, kundavtal, krav i upphandling
- **källa_bevis:** Q9/Q14/Q45/Q27-4.2

### A4. Vad ska skyddas (information)?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** VD / ägare, administratör, IT-ansvarig eller IT-leverantör
- **var_informationen_finns:** Affärssystem, mejl, lönesystem, kundregister, avtalsmapp
- **vanliga_bevis:** Lista över information och system som ska skyddas, beskrivning av vad systemet gäller
- **källa_bevis:** Q27-4.3, Q27-6.1.2, A4

### B1. Har chefen lovat kvalitet?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare
- **var_informationen_finns:** Policypärm, personalpärm, anslagstavla, introduktionsmapp
- **vanliga_bevis:** Underskrivet kvalitetslöfte, lista där personalen kvitterat att de sett det
- **källa_bevis:** Q9-5.2

### B2. Har chefen lovat miljö?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare
- **var_informationen_finns:** Policypärm, personalpärm, anslagstavla
- **vanliga_bevis:** Underskrivet miljölöfte, kvittens från personal
- **källa_bevis:** Q14-5.1, Q14-5.2

### B3. Har chefen lovat säkerhet?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare, skyddsombud
- **var_informationen_finns:** Policypärm, skyddsombudspärm, introduktion
- **vanliga_bevis:** Underskrivet arbetsmiljölöfte, kvittens från personal
- **källa_bevis:** Q45-5.1, Q45-5.2

### B4. Har chefen lovat att skydda information?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare, IT-ansvarig eller IT-leverantör
- **var_informationen_finns:** Policypärm, IT-instruktion, anställningsavtal
- **vanliga_bevis:** Underskrivet löfte om skydd av uppgifter och IT
- **källa_bevis:** Q27-5.1, Q27-5.2

### B5. Vet alla vem som gör vad?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare, administratör
- **var_informationen_finns:** Enkel rollista, anställningsavtal, organisation på en sida
- **vanliga_bevis:** Lista med namn och ansvar, befattningsbeskrivning om sådan finns
- **källa_bevis:** Q9-5.3, Q14-5.3, Q45-5.3, Q27-5.3

### B6. Får personalen vara med?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** VD / ägare, skyddsombud, platschef / arbetsledare, den som gör jobbet
- **var_informationen_finns:** Fredagsmöte, skyddsrond, förslagslåda, personalmöte
- **vanliga_bevis:** Mötesanteckningar, skyddsrondprotokoll, deltagarlista, förbättringsförslag
- **källa_bevis:** Q45-5.4, Q9-5.1

### C1. Vad kan gå fel i jobbet?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** VD / ägare, platschef / arbetsledare, säljare / kundansvarig, den som gör jobbet
- **var_informationen_finns:** Reklamationer, sena jobb, felmaterial, huvudbry i vardagen
- **vanliga_bevis:** Enkel risklista, SWOT om sådan finns, reklamationslista
- **källa_bevis:** Q9-6.1

### C2. Vad kan skada miljön?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** VD / ägare, platschef / arbetsledare, den som gör jobbet
- **var_informationen_finns:** Avfallskärl, kemikalier på hyllan, körjournal, elfaktura
- **vanliga_bevis:** Lista över det som påverkar miljön, kemikalielista, avfallsavtal
- **källa_bevis:** Q14-6.1.2, Q14-8.1

### C3. Vad kan skada personalen?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Skyddsombud, platschef / arbetsledare, den som gör jobbet, VD / ägare
- **var_informationen_finns:** Skyddsrond, tillbud, vardag på arbetsplatsen, SDB för kemikalier
- **vanliga_bevis:** Riskbedömning, skyddsrondprotokoll, tillbudslista
- **källa_bevis:** Q45-6.1.2, Q45-9.1b

### C4. Vad kan läcka eller stjälas?

- **vd_kan_svara_direkt:** nej
- **information_finns_hos:** IT-ansvarig eller IT-leverantör, administratör, VD / ägare
- **var_informationen_finns:** Datorer, mobiler, mejl, molntjänst, backup
- **vanliga_bevis:** Lista över informationstillgångar, enkel risklista för IT, backup-rutin
- **källa_bevis:** Q27-6.1.2, Q27-6.1.3

### C5. Vilka lagar måste ni följa?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** VD / ägare, administratör, skyddsombud, ekonomi / lön
- **var_informationen_finns:** Myndighetspost, branschorganisation, anställningsavtal, avfallsavtal, integritetspolicy
- **vanliga_bevis:** Kort laglista, anteckning att listan gåtts igenom
- **källa_bevis:** Q14-6.1.3, Q45-6.1.3, Q9-4.1, Q27-4.2

### C6. Finns enkla mål?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare
- **var_informationen_finns:** Ledningsmöte, budget, tavla på kontoret, årsplan
- **vanliga_bevis:** Målkort eller kort mål-lista, enkel handlingsplan
- **källa_bevis:** Q9-6.2, Q14-6.2, Q45-6.2, Q27-6.2

### D1. Kan alla sitt jobb?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Platschef / arbetsledare, administratör / HR, VD / ägare
- **var_informationen_finns:** Huvudet på arbetsledaren, utbildningsintyg, anställningsavtal, körkortspärm
- **vanliga_bevis:** En rad per person (namn, jobb, kan, nästa kurs), utbildningsplan, intyg
- **källa_bevis:** Q9-7.2, Q14-7.2, Q45-7.2

### D2. Får nya en introduktion?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Platschef / arbetsledare, handledare, administratör / HR, VD / ägare
- **var_informationen_finns:** Första arbetsdagen, checklista i personalpärm, genomgång med handledare
- **vanliga_bevis:** Introduktionschecklista, underskrift att genomgång skett
- **källa_bevis:** Q9-7.3, Q45-7.3, Q27-7.3, D2

### D3. Vet alla reglerna?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Administratör, platschef / arbetsledare, VD / ägare
- **var_informationen_finns:** Personalpärm, introduktion, personalmöte
- **vanliga_bevis:** Kvittenslista på policyer, mötesanteckning från genomgång
- **källa_bevis:** Q9-7.3, Q14-7.3, Q45-7.3, Q27-7.3

### D4. Finns rätt utrustning?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Platschef / arbetsledare, inköpsansvarig, IT-ansvarig eller IT-leverantör, VD / ägare
- **var_informationen_finns:** Bilar och förråd, skyddsutrustning, datorer, underhållsleverantör
- **vanliga_bevis:** Inventarielista, underhållskvitto, lista på skyddsutrustning, backup-uppgift
- **källa_bevis:** Q9-7.1, Q45-8.1.2, Q27-A.8

### D5. Sparas rätt version av dokument?

- **vd_kan_svara_direkt:** nej
- **information_finns_hos:** Administratör, VD / ägare
- **var_informationen_finns:** Gemensam mapp, pärm med flikar, utskrivna mallar i bilarna
- **vanliga_bevis:** Versionsdatum på dokument, mapp med enbart senaste versionen
- **källa_bevis:** Q9-7.5, Q14-7.5, Q45-7.5, Q27-7.5

### D6. Vem får logga in var?

- **vd_kan_svara_direkt:** nej
- **information_finns_hos:** IT-ansvarig eller IT-leverantör, administratör, VD / ägare
- **var_informationen_finns:** Användarlista i programmet, mejladministration, offboarding när någon slutar
- **vanliga_bevis:** Användarregister, anteckning att konto stängts, regel om egna konton
- **källa_bevis:** Q27-A.5

### E1. Hur tar ni emot en order?

- **vd_kan_svara_direkt:** ja i 1–5 anställda, delvis därefter
- **information_finns_hos:** Säljare / kundansvarig, VD / ägare, administratör
- **var_informationen_finns:** Mejl, telefon, offertmall, avtalsmapp, affärssystem
- **vanliga_bevis:** Offert, orderbekräftelse, avtal, enkel beskrivning av stegen
- **källa_bevis:** Q9-8.2, Q9-8.1

### E2. Hur utförs jobbet?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Den som gör jobbet, platschef / arbetsledare, projektledare
- **var_informationen_finns:** Arbetsorder, checklista i bilen, “så här gör vi”-lista, egenkontroll
- **vanliga_bevis:** Kort rutin för vanligaste jobben, ifylld checklista, arbetsorder
- **källa_bevis:** Q9-8.5, Q9-8.1

### E3. Hur köper ni in?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Inköpsansvarig, administratör, VD / ägare
- **var_informationen_finns:** Leverantörsfakturor, inköpsmejl, avtal, “vi brukar köpa av”
- **vanliga_bevis:** Lista över godkända leverantörer, inköpskrav, avtal, bedömning av ny leverantör
- **källa_bevis:** Q9-8.4, Q14-8.1b, Q27-A.5c

### E4. Hur hanteras avfall och kemikalier?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Platschef / arbetsledare, den som gör jobbet, administratör
- **var_informationen_finns:** Städskåp, förråd, avfallskärl, transportörsavtal, SDB-pärm
- **vanliga_bevis:** Kemikalielista, säkerhetsdatablad, avfallsavtal, sorteringsinstruktion
- **källa_bevis:** Q14-8.1, Q14-7.5, Q45-8.1.2

### E5. Finns plan om något går riktigt fel?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Skyddsombud, platschef / arbetsledare, IT-ansvarig eller IT-leverantör, VD / ägare
- **var_informationen_finns:** Första hjälpen-väska, utrymningsplan, larmlista i telefonen, IT-leverantörens support
- **vanliga_bevis:** Nödplan, övningsanteckning, lista med larmnummer, incidentrutin för IT
- **källa_bevis:** Q14-8.2, Q45-8.2, Q27-A.5b

### E6. Hur skyddas information i vardagen?

- **vd_kan_svara_direkt:** nej
- **information_finns_hos:** IT-ansvarig eller IT-leverantör, administratör, den som gör jobbet
- **var_informationen_finns:** Datorer, mobiler, skrivare, USB-minnen, papperskorg
- **vanliga_bevis:** Kort IT-instruktion, skärmlås, rutin för papper och USB, backup-rutin
- **källa_bevis:** Q27-7.3, Q27-A.8, Q27-A.5

### F1. Frågar ni kunderna?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Säljare / kundansvarig, projektledare, VD / ägare
- **var_informationen_finns:** Eftersamtal, mejl efter avslutat jobb, enkät, reklamationer
- **vanliga_bevis:** Kundfrågor och svar, sammanställning, klagomålslista
- **källa_bevis:** Q9-9.1, Q9-5.1

### F2. Bedömer ni leverantörer?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Inköpsansvarig, platschef / arbetsledare, administratör
- **var_informationen_finns:** Fakturahistorik, sena leveranser, fel i material, samtal med leverantör
- **vanliga_bevis:** Enkel betygslista på huvudleverantörer, inköpsuppföljning
- **källa_bevis:** Q9-8.4, Q14-8.1b

### F3. Mäter ni det ni lovat?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Administratör / ekonomi, VD / ägare, skyddsombud
- **var_informationen_finns:** Reklamationslista, avfallsfaktura, tillbudslista, sjukfrånvaro, IT-ärenden
- **vanliga_bevis:** Enkel tabell med mål och utfall, mätdata för avfall eller energi, tillbudsstatistik
- **källa_bevis:** Q9-9.1, Q14-9.1.1, Q45-9.1, Q27-9.1

### F4. Kollar ni lagarna?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Administratör, skyddsombud, VD / ägare
- **var_informationen_finns:** Laglista, myndighetsmejl, branschinfo, årsgenomgång
- **vanliga_bevis:** Laglista med datum för senaste genomgång, anteckning om avvikelse
- **källa_bevis:** Q14-9.1.2, Q45-6.1.3

### F5. Gör ni internrevision?

- **vd_kan_svara_direkt:** nej
- **information_finns_hos:** Den som utsetts att gå igenom systemet, administratör, VD / ägare
- **var_informationen_finns:** Kalender, revisionsanteckningar, åtgärdslista
- **vanliga_bevis:** Enkel plan för genomgång, protokoll, åtgärdslista
- **källa_bevis:** Q9-9.2, Q14-9.2, Q45-9.2, Q27-9.2

### F6. Har chefen ett årligt möte om systemet?

- **vd_kan_svara_direkt:** ja
- **information_finns_hos:** VD / ägare, administratör
- **var_informationen_finns:** Kalender, ledningsmöte, årsavslut
- **vanliga_bevis:** Protokoll från ledningens genomgång, dagordning
- **källa_bevis:** Q9-9.3, Q14-9.3, Q45-9.3, Q27-9.3

### G1. Skrivs fel upp?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Den som gör jobbet, platschef / arbetsledare, administratör, VD / ägare
- **var_informationen_finns:** Mejl från kund, anteckning i bok, tillbudsblankett, reklamationsmapp
- **vanliga_bevis:** Avvikelserapport, reklamationslista, tillbudsrapport, incidentrapport
- **källa_bevis:** Q9-10.2, Q9-8.7, Q14-10.2, Q45-10.2, Q27-10.1

### G2. Fixas orsaken, inte bara felet?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Platschef / arbetsledare, VD / ägare, den som utreder
- **var_informationen_finns:** Åtgärd efter reklamation, ändrad checklista, samtal efter tillbud
- **vanliga_bevis:** Avvikelserapport med orsak och åtgärd, uppföljningsdatum
- **källa_bevis:** Q9-10.2, Q45-10.2, Q14-10.2

### G3. Tas idéer emot?

- **vd_kan_svara_direkt:** delvis
- **information_finns_hos:** Den som gör jobbet, platschef / arbetsledare, VD / ägare
- **var_informationen_finns:** Personalmöte, förslagslåda, chatt, skyddsrond
- **vanliga_bevis:** Förbättringsförslag, åtgärdslista, mötesanteckning
- **källa_bevis:** Q9-10.3, Q14-10.3, Q45-10.3, Q27-10.2

---

## Kravområden i `01`–`04` som saknas som egna frågor i `10`

Dessa ska få samma två fält den dag de lyfts in. Inga nya krav, bara källbank som inte har egen A–G-fråga.

| Källa | Vad det handlar om | information_finns_hos | vanliga_bevis |
|-------|--------------------|------------------------|---------------|
| Q9-6.3 | Ändringar planeras innan de görs | VD / ägare, platschef / arbetsledare | Ändringsanteckning, mötesbeslut |
| Q9-8.6 | Kontroll innan leverans till kund | Den som gör jobbet, arbetsledare | Slutchecklista, kundgodkännande |
| Q9-8.7 | Felaktigt arbete släpps inte vidare | Arbetsledare, den som gör jobbet | Avvikelse, stopp av leverans |
| Q14-8.1c | Inköp, användning och avfall hänger ihop | Arbetsledare, inköp, VD | Miljöutredning, inköpskrav, avfallsavtal |
| Q14-9.1.2 | Lagefterlevnad följs upp | Administratör, VD | Lagefterlevnadskontroll med datum |
| Q45-8.1.3 | Riskbedömning när arbetet ändras | Skyddsombud, arbetsledare | Riskbedömning vid ändring |
| Q45-8.1.4 | Inhyrda och entreprenörer får riskinfo | Arbetsledare, skyddsombud | Introduktion för UE, deltagarlista |
| Q45-9.1b | Skyddsrond enligt plan | Skyddsombud, arbetsledare | Skyddsrondprotokoll |
| Q27-6.1.3 | Valda skyddsåtgärder finns nedskrivna | IT-ansvarig eller IT-leverantör, VD | Lista över valda skyddsåtgärder |
| Q27-8.1 | Skyddsåtgärder genomförs | IT-ansvarig eller IT-leverantör | Åtgärdsplan med status |
| Q27-A.8 | Backup, enheter, radering | IT-ansvarig eller IT-leverantör, administratör | Backup-rutin, test av backup |

---

## Vad revisorn normalt tittar på

Samma saker som redan står som bevis i `01`–`04`, översatta till vardag:

**Alltid vanligt hos små företag**
- Underskrivna löften (policyer)
- En lista över ansvar
- Någon form av risk- eller farolista
- Introduktion av nyanställda
- Avtal och offerter
- Reklamationer eller tillbud
- Ett årligt möte med anteckningar

**Vanligt när miljö är vald**
- Kemikalielista och säkerhetsdatablad
- Avfallsavtal
- Kort lista över det som påverkar miljön

**Vanligt när arbetsmiljö är vald**
- Riskbedömning
- Skyddsrondprotokoll
- Tillbud
- Nödplan / första hjälpen

**Vanligt när information är vald**
- Lista över system och uppgifter
- Egna konton
- Backup
- Incidentanteckning
- Lista över valda skyddsåtgärder

Revisorer i små bolag accepterar enkla listor. De accepterar inte tomma mallar som ingen använder.

---

## Regel för quizet

När användaren inte kan svara ska systemet visa, i denna ordning:

1. Förklaring av frågan
2. Vem som oftast har svaret
3. Var informationen normalt finns
4. Vilket bevis som räcker

Inte en föreläsning om standarden.

För 1–5 anställda: visa VD först, sedan “den som gör jobbet”.  
För 21–50 anställda: visa den namngivna rollen först.

---

## Koppling till schema

Lägg till i `13_Question_JSON_Schema.md`:

```json
"vd_kan_svara_direkt": "ja",
"information_finns_hos": ["VD / ägare"],
"var_informationen_finns": ["hemsidan", "kundavtal"],
"vanliga_bevis": ["kort verksamhetsbeskrivning", "manualens inledning"]
```
