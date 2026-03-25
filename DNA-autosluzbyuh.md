# DNA — Autoslužby UH s.r.o.

**Typ projektu:** Jednostránkový web autoservisu (landing page)
**Klient:** Autoslužby UH s.r.o., Uherské Hradiště
**Datum dokončení:** 2026-03-25

---

## Vizuální archetype

**Precision & Trust** — Teal + dark navy. Moderní autoservis jako technologická firma. Žádná agresivita, žádná červená ani amber. Čistý, důvěryhodný, precizní dojem — automotive přesnost bez garáže.

---

## Barevná paleta

| Proměnná | Hex | Role |
|----------|-----|------|
| `--dark` | `#141B22` | Hero, nav, footer |
| `--dark-mid` | `#1A2738` | Kontakt, why sekce |
| `--teal` | `#14B8A6` | Primární akcent |
| `--teal-d` | `#0D9488` | Hover |
| `--teal-l` | `#CCFBF1` | Světlé teal plochy |
| `--concrete` | `#F8FAFC` | Světlé sekce |
| `--white` | `#FFFFFF` | Čistá bílá |
| `--text-dark` | `#0F172A` | Hlavní text |
| `--text-mid` | `#475569` | Sekundární text |

**Charakter palety:** Teal jako automotive precisnost — ne agresivní (červená), ne průmyslový (navy+amber). Svěží, moderní, důvěryhodný.

---

## Typografie

| Řez | Font | Použití |
|-----|------|---------|
| Nadpisy | Oswald 400–700 | H1–H4, nav, labely, stat čísla |
| Tělo | Manrope 300–700 | Odstavce, popisky, formulář |

- H1: `clamp(3rem, 6vw, 5rem)`, weight 800, letter-spacing 0.01em, line-height 1.0
- H2: `clamp(1.8rem, 3.5vw, 2.8rem)`, weight 700, letter-spacing 0.01em
- Section label: 0.72rem, letter-spacing 0.2em, uppercase, teal linka vlevo
- **Nav logo text: 1.65rem / 800** — osvědčená velikost pro čitelné logo v liště
- **Nav logo ikona: 40×40px, SVG 22×22px** — kompaktní, nekonkuruje textu

---

## Layout a struktura sekcí

```
1. NAV          — Fixed, průhledný → dark při scrollu, hamburger na mobilu
2. HERO         — Radial teal glow dekorace, velký H1 vlevo,
                  info panel vpravo (tel, email, adresa, hodiny, tagy)
3. SLUŽBY       — 6 karet v gridu 3×2, teal left-border na hover + translateY
4. PROČ MY      — Dark-mid sekce, 4 benefity číslované 01–04
5. O NÁS        — Split layout: text+seznam vlevo / tým+adresa vpravo
                  Vozidla box dole (sedan, dodávka, G-Wagon+rezerva)
6. KONTAKT      — Dark sekce, split: hodiny tabulka vlevo / kontakty vpravo
7. FORMULÁŘ     — Světlá sekce, intro vlevo + form vpravo
8. FOOTER       — 3 sloupce, teal border-top
```

---

## Klíčové UI vzory

- **Hero radial glow:** `radial-gradient` teal na tmavém pozadí (ne canvas dots, ne grid textura)
- **Hero info panel:** poloprůhledný rámeček vpravo s real kontakty — vyplní dead space
- **Section label:** teal linka 32px vlevo + Manrope uppercase 0.72rem 0.2em tracking
- **Service karty:** teal `left-border` scaleY(0→1) na hover + translateY(-4px)
- **Tým karty:** avatar s iniciálami (FK/PK), jméno, role, telefon — humanizuje firmu
- **Vozidla box:** 3 SVG ikony (sedan / dodávka / G-Wagon se zásobní pneumatikou) + popisek
- **Čísla benefitů:** 01–04 v teal, Oswald, velké — vizuální kotva dark sekce
- **Fade-up:** IntersectionObserver, delay třídy d1–d4
- **Tlačítka:** border-radius 6px, teal primary + ghost varianta

---

## Technický stack

- Čistý HTML/CSS/JS — jeden soubor `index.html`
- Google Fonts (Oswald + Manrope)
- Formulář: lokální simulace — Formspree ID nutno doplnit
- Deploy: GitHub → supercigan/autosluzbyuh → Vercel

---

## Co se osvědčilo

- **Teal akcent** — v kontextu všech DNA projektů zcela unikátní, svěží a důvěryhodný
- **Oswald pro nadpisy** — kondenzovaný, razantní, automotive charakter bez agresivity
- **Tým sekce (FK + PK)** — humanizuje firmu, žádný předchozí projekt tohle neměl
- **Hero info panel vpravo** — okamžitě viditelné kontakty, vyplní prázdný prostor
- **Vozidla box se zásobní pneumatikou** — G-Wagon ikonka s rezervou vzadu je okamžitě rozpoznatelná
- **Nav logo: ikona 40px + text 1.65rem** — správné proporce, text dominuje ale ikona drží identitu

## Co se nepovedlo / co příště udělat jinak

- **Syne jako první volba nadpisového fontu** — geometrický/kulatý Syne nevypadal dost razantně pro autoservis, nahrazen Osweldem; příště začít rovnou kondenzovaným fontem
- **Stats sekce** — na žádost klienta smazána; před přidáváním dalších sekcí ověřit záměr
- **SVG ikony ve vehicles-box** — první iterace ikon (sedan, dodávka, SUV) vypadaly jako crosshair/hodinky/dolar při malé velikosti; viewBox musí být větší než 24×24 a ikony stroke-based s jednoduchými tvary
- **Ikony v service kartách** — první návrh byl nerozpoznatelný; přejít systematicky přes každou ikonu před prvním commitem (poučení z O.K. projektu ale znovu se stalo)
