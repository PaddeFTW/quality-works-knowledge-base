---
id: amp-roller-bas
title: Roller BAS-P, BAS-U och byggherre
typ: process
version: 1.0.0
datum: 2026-09-04
sprak: sv
regelverk: [AFS 2023:3, AML kap. 3]
---

# Roller i byggarbetsmiljön

En BAS-P och en BAS-U ska vara utsedda i taget. Samma person eller företag kan ha båda uppdragen, men det ska alltid vara tydligt vem som gäller.

## Byggherre

| Uppgift | Utförd | Datum |
|---------|--------|-------|
| Utser BAS-P och BAS-U | ☐ | |
| Ser till att AMP tas fram när den krävs | ☐ | |
| Ser till att förhandsanmälan görs när tröskel nås | ☐ | |
| Ger tid, mandat och underlag | ☐ | |
| Följer upp att BAS utför sina uppgifter | ☐ | |

Byggherre: {{byggherre}}

## BAS-P – planering och projektering

| Uppgift | Status | Kommentar |
|---------|--------|-----------|
| Samordnar projektörers arbetsmiljöarbete | ☐ | |
| Driver borttagning av risk redan i handlingarna | ☐ | |
| Tar fram AMP innan utförande startar | ☐ | |
| Överlämnar AMP och underlag till BAS-U | ☐ | |
| Informerar byggherren vid allvarliga brister | ☐ | |

BAS-P: {{bas_p}} · {{bas_p_foretag}}  
Period: __________ – __________

## BAS-U – utförande

| Uppgift | Status | Kommentar |
|---------|--------|-----------|
| Tar emot AMP och håller den aktuell | ☐ | |
| Ger klartecken före start efter riskinfo | ☐ | |
| Samordnar entreprenörer och samtidiga arbeten | ☐ | |
| Ser till att gemensamma regler efterlevs | ☐ | |
| Introducerar den som kommer till platsen | ☐ | |
| Organiserar skyddsverksamhet | ☐ | |
| Följer upp att åtgärder mot särskild risk fungerar | ☐ | |

BAS-U: {{bas_u}} · {{bas_u_foretag}}  
Period: __________ – __________

## Övriga nyckelroller

| Roll | Typiskt ansvar i detta paket | Namn |
|------|------------------------------|------|
| Platschef | Drift, arbetsberedning, daglig kontroll | {{platschef}} |
| Projektchef | Övergripande projekt | {{projektchef}} |
| Skyddsombud | Medverkan, rond, stopprätt enligt AML | {{skyddsombud}} |
| KMA | Dokumentstyrning, intern uppföljning | {{kma}} |
| Arbetsgivare (varje företag) | Eget SAM enligt AFS 2023:1, uppgifter till BAS-U | |

## Beslutsregel för appen

- Saknas BAS-U-namn: blockera status `gallande` på AMP.
- Byte av BAS: tvinga ny utgåva + ev. uppdaterad förhandsanmälan.
- UE utan kvitterad AMP: flagga före tillträde.
