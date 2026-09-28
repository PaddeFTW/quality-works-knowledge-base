# Quiz-fält (så appen ska se ut)

## Varje fråga har dessa fält

| Fält | Vad det är | Exempel |
|------|------------|---------|
| id | Unikt id | A1, C3, G2 |
| standarder | Vilka ISO den gäller | 9001, 14001 |
| avsnitt | Kravavsnitt 4–10 | 6 Planering |
| fråga | Enkel fråga | Vad kan skada personalen? |
| tips | 1–2 rader hjälp | Tänk lyft, halka, kemikalier |
| status | Ja / Delvis / Nej | knappar |
| fritext | Hur ni gör det | textruta |
| placeholder | Grå exempeltext i rutan | "Tunga sopor, halka..." |
| bevis | Vad kan ni visa? | lista, foto, protokoll |
| vd_kan_svara_direkt | ja / delvis / nej (E1: ja i 1–5) | styr hjälptextens början |
| information_finns_hos | 2–4 roller från låst lista | visas även när VD kan svara |
| var_informationen_finns | var underlaget ligger i små företag | visas när användaren inte kan svara |
| vanliga_bevis | bevisnamn från kunskapsbanken | fyller “Vad kan ni visa?” |

Källa för de fyra sista fälten: `21_Information_och_Bevis.md`. Inget nytt ISO-krav.

## Knappar
`[ Ja ]  [ Delvis ]  [ Nej ]`

## Textrutor
1. Hur gör ni det hos er?  
   Placeholder: se frågan
2. Vad kan ni visa som bevis?  
   Placeholder: "Lista i pärmen / protokoll 2026-03-12"
3. Om Delvis eller Nej – vad saknas och vad gör ni?  
   Placeholder: "Saknar lista. Anna gör den senast 15 okt."

## Filter i programmet
Användaren väljer standarder först.
- Bara 9001 → visa frågor märkta 9001
- 9001+14001+45001 → visa alla KMA-frågor
- Alla fyra → visa även 27001-frågor
Frågor märkta med flera standarder visas en gång.
