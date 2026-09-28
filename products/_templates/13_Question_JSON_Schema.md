# ISO Quiz - Question Schema

## Syfte

Alla frågor i ISO Quiz ska följa samma struktur.

Frågor ska kunna användas för:

- Quiz
- Manualgenerator
- Word-export
- PDF-export
- Internrevision
- GAP-analys
- Certifieringsförberedelse

---

## Fält

id

standarder

bransch

foretagsstorlek

avsnitt

prioritet

fraga

forklaring

exempel

tips

placeholder

mallsvar

manualtext

vd_kan_svara_direkt

information_finns_hos

var_informationen_finns

vanliga_bevis

Källa för de fyra sista: `21_Information_och_Bevis.md`.

---

## Exempel

{
  "id": "A1",
  "standarder": ["9001","14001","45001","27001"],
  "bransch": ["alla"],
  "foretagsstorlek": ["alla"],
  "avsnitt": "Organisation",
  "prioritet": "hog",

  "fraga": "Vad gör ert företag och vilka delar ska ledningssystemet gälla för?",

  "forklaring": "Beskriv verksamheten och vad systemet ska omfatta.",

  "exempel": "Vi är ett städföretag med 8 anställda som arbetar i Göteborg.",

  "tips": [
    "Beskriv verksamheten",
    "Beskriv kunderna",
    "Beskriv geografiskt område"
  ],

  "placeholder": "Vi är...",

  "mallsvar": "Vi är [företagsnamn]...",

  "manualtext": "Företaget bedriver verksamhet inom..."
}