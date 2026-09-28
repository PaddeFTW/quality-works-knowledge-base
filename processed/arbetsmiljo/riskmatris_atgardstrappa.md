---
id: amp-riskmatris
title: Riskmatris 5×5 och åtgärdstrappa
typ: instruktion
version: 1.0.0
datum: 2026-09-04
sprak: sv
regelverk: [AFS 2023:1, AFS 2023:3]
---

# Riskmatris 5×5

Poäng = sannolikhet × konsekvens. Använd samma skala i hela projektet.

## Sannolikhet (S)

| Värde | Benämning | Tumregel |
|-------|-----------|----------|
| 1 | Mycket osannolik | Kan inträffa i branschen, inte förväntat här |
| 2 | Osannolik | Har hänt i liknande projekt |
| 3 | Möjlig | Kan hända under projektet utan extra skydd |
| 4 | Sannolik | Förväntas utan åtgärd |
| 5 | Mycket sannolik | Inträffar ofta vid liknande moment |

## Konsekvens (K)

| Värde | Benämning | Tumregel |
|-------|-----------|----------|
| 1 | Försumbar | Första hjälpen, ingen sjukfrånvaro |
| 2 | Lindrig | Kort sjukfrånvaro, lätt skada |
| 3 | Allvarlig | Längre sjukfrånvaro, bruten kroppsdel |
| 4 | Mycket allvarlig | Bestående men, flera skadade |
| 5 | Katastrofal | Dödsfall eller många svårt skadade |

## Matris

| S \ K | 1 | 2 | 3 | 4 | 5 |
|-------|---|---|---|---|---|
| 5 | 5 | 10 | 15 | 20 | 25 |
| 4 | 4 | 8 | 12 | 16 | 20 |
| 3 | 3 | 6 | 9 | 12 | 15 |
| 2 | 2 | 4 | 6 | 8 | 10 |
| 1 | 1 | 2 | 3 | 4 | 5 |

| Poäng | Klass | Färgkod i app | Beslut |
|-------|-------|---------------|--------|
| 1–4 | Låg | grön | Dokumentera, bevaka |
| 5–9 | Medel | gul | Åtgärd inom plan, uppföljning |
| 10–16 | Hög | orange | Åtgärd före start av moment |
| 17–25 | Mycket hög | röd | Stopp. Ny metod eller skydd innan start. BAS-U godkänner |

Särskild risk enligt 11 kap. 12 § får inte lämnas utan beskriven åtgärd även om poängen blir låg.

## Åtgärdstrappa

Välj högsta möjliga nivå som är rimlig. Personlig skyddsutrustning är sista steget, inte första.

| Nivå | Princip | Exempel bygg |
|------|---------|--------------|
| 1 | Eliminera | Prefab i fabrik i stället för arbete på hög höjd |
| 2 | Ersätt | Mindre farligt ämne, annan metod |
| 3 | Teknisk / kollektiv | Ställning med skyddsräcke, schaktstöd, trafikavstängning |
| 4 | Organisatorisk | Tidsseparation, behörighet, arbetsberedning, bevakning |
| 5 | Personlig skyddsutrustning | Sele, andningsskydd, hörselskydd |

Dokumentera vald nivå och varför lägre nivå inte räcker.

## Residualrisk

Efter åtgärd skattas S och K på nytt.  
Moment får starta när residualklass är acceptabel enligt projektets regel **och** särskild-risk-åtgärd finns i AMP.
