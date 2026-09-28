# Quality WorX Knowledge Base

**Version:** 1.0  
**Status:** Förslag för godkännande  
**Syfte:** Gemensam, källspårbar kunskapsgrund för Quality WorX Apps Platform, fristående produktappar, konsulter och framtida AI-stöd.

---

## 1. Vad detta projekt är

Quality WorX Knowledge Base ska samla, bevara, analysera, strukturera, kvalitetssäkra och förädla KvalitetsDokuments och KvalitetsGruppens kunskap.

Kunskapsbanken ska kunna leverera:

- kvalitetssäkrat produktinnehåll
- källhänvisningar
- ordlistor och definitioner
- frågebanker och stegbanker
- innehållsblueprints
- branschanpassningar
- hjälptexter
- appunderlag
- underlag till Smart arbetsyta
- underlag till framtida AI-funktioner

Projektet ska **inte bygga applikationskod**.

---

## 2. Grundprinciper

- Originalfiler bevaras oförändrade.
- Varje original får ett stabilt `source_id`.
- Varje original får metadata och SHA-256-kontrollsumma.
- Bearbetad kunskap lagras separat.
- Bearbetad kunskap länkas tillbaka till ett eller flera `source_id`.
- Inga original skrivs över.
- Dubbletter, konflikter och versionsdrift dokumenteras.
- Kundmaterial och licensierade standarder hanteras restriktivt.
- Fulltext från licensierade standarder återges inte i onödan.
- Innehåll får inte hittas på när källunderlag saknas.
- Osäker information markeras tydligt.
- Källan ska alltid kunna identifieras i efterhand.

---

## 3. Vad Knowledge Base stödjer

Knowledge Base ska stödja:

1. Quality WorX Apps Platform
2. fristående Quality WorX-produktappar
3. Quality WorX App Template
4. Smart arbetsyta
5. konsulter och interna projekt
6. framtida AI-funktioner
7. produktutveckling och utbildning

Ingen enskild app ska äga den gemensamma kunskapen.

---

## 4. Rekommenderad struktur

Se avsnitt 11 för den spegling som gäller i detta repo.

---

## 5–10

Se styrpaketet i `standards/` och `source-briefs/`.

---

## 11. Denna repo-spegling (`PaddeFTW/quality-works-knowledge-base`)

```text
quality-works-knowledge-base/
├── README.md
├── originals/          # bara register, inga PDF/DOCX
├── processed/
│   ├── reports/
│   ├── hr-onboarding/
│   ├── arbetsmiljo/
│   ├── forbattring/
│   ├── ledning/        # tom tills MVP ledning
│   └── implementering/
├── products/
│   ├── _templates/
│   └── introduktion-nyanstalld/
├── standards/
├── source-briefs/
└── registry/
```

Inga original-PDF/DOCX i `processed/`. Inga licensierade standarder i fulltext.  
App-template ska peka på `processed/` + demo-fältkontrakt för **introduktion nyanställd**.
