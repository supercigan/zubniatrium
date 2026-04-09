# Zubní Atrium — Web Summary

## Projekt
Moderní jednostránkový web pro zubní ordinaci MUDr. Petry Matějíčkové.

## Zdroj dat
- Screenshot původního webu: `www.zubniatrium.cz_.png`
- WebFetch: https://www.zubniatrium.cz/

## Reálné informace zachované z originálu

| Položka | Hodnota |
|---|---|
| Lékař | MUDr. Petra Matějíčková |
| Specializace | Praktická zubní lékařka + dentální hygienistka |
| IČO | 48491756 |
| UH adresa | Masarykovo nám. 157 (Atrium), 686 01 |
| UH telefon | 739 064 328 |
| Boršice adresa | Hradišťská 170, 687 09 |
| Boršice telefon | 773 501 422 |
| Pohotovost | 155, 572 529 111 (nemuh.cz) |
| Aktuální stav | Nepřijímají nové pacienty (naplněná kapacita) |

### Ordinační hodiny — Uherské Hradiště
- Pondělí: 12:00–15:30
- Úterý: 7:30–12:00
- Středa: 12:00–15:30
- Čtvrtek: 7:30–12:00, 12:30–16:30
- Pátek: zavřeno

### Ordinační hodiny — Boršice
- Pondělí: 7:30–11:30
- Úterý: 12:30–17:30
- Středa: 7:30–11:30
- Čtvrtek–Pátek: zavřeno

## Design rozhodnutí

### Fonty
- **Cormorant Garamond** (nadpisy) — elegantní serif, evokuje preciznost a důvěru vhodnou pro lékařskou praxi
- **Inter** (body text) — čistý, moderní sans-serif, maximální čitelnost

### Barevná paleta
- `#0d2b45` — hluboká námořní modrá — autorita, důvěra
- `#1e7b6e` — střední teal — zdraví, čistota
- `#bee3df` — světlý mint — svěžest, vzduch
- `#f8fcfb` — téměř bílá — pozadí, čistota
- `#2d3748` — tmavý text — čitelnost

## Sekce webu
1. **Nav** — fixed, logo, links, hamburger pro mobil
2. **Hero** — jméno doktorky, badge, CTA tlačítka, scroll hint
3. **O nás** — notice (nepřijímají pacienty), features, vizuální karta s lokalitami
4. **Služby** — 6 karet (preventivní péče, ošetření, hygiena, RTG, děti, akutní)
5. **Ordinační hodiny** — dvě karty side by side (UH + Boršice)
6. **Kontakt** — dvě karty s adresami + emergency box
7. **Footer** — logo, links, info

## Responsivita
- Breakpointy: 900px, 768px, 640px, 428px, 375px, 320px
- Hamburger menu od 768px
- overflow-x: hidden na html i body
- Min font-size 16px zachován
- Min touch target 44px na všech CTA
- Hero actions → column na 640px

## Animace
- Hero: fadeUp keyframe animace při načtení
- Sekce: IntersectionObserver scroll reveal (.reveal class)
- Hover efekty na kartách, featurách, nav linkách
- Scroll indicator s bounce animací

## Soubory
- `index.html` — kompletní jednostránkový web
- `summary.md` — tento soubor
- `www.zubniatrium.cz_.png` — screenshot původního webu
