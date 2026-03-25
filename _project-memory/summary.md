# Projekt: Autoslužby UH s.r.o.
**Datum zahájení:** 2026-03-25
**Datum dokončení:** 2026-03-25

---

## Co je hotovo
- [x] Inicializace projektu, _project-memory/summary.md
- [x] Přečteny všechny DNA soubory (6 projektů) — zaznamenáno co NEpoužívat
- [x] Scraping reálného webu autosluzbyuh.cz — získány všechny info
- [x] Navržena vizuální identita (fonty, paleta, archetype)
- [x] Vytvořen kompletní index.html — jednostránkový web
- [x] Opravy po screenshotu (ikony, grid, centrování, kontrast)
- [x] Stats sekce smazána (na žádost klienta)
- [x] Vozidla box ikony — sedan, dodávka, G-Wagon se zásobní pneumatikou
- [x] Font nadpisů změněn: Syne → Oswald
- [x] Nav logo: text zvětšen na 1.65rem, ikona 40px
- [x] GitHub push → Vercel deploy
- [x] DNA soubor vytvořen

---

## Reálné info ze starého webu
- **Firma:** Autoslužby UH s.r.o., IČO: 29363306
- **Provozovna:** Třída M. Malinovského 473, 686 01 Uherské Hradiště
- **Sídlo:** Nová 604, 687 22 Ostrožská Nová Ves
- **Tel. servis:** +420 572 503 230
- **František Klas:** +420 608 851 012 (příjem oprav, technik)
- **Pavel Klas:** +420 603 323 929 (příjem oprav, fakturace)
- **Email:** servis@autosluzbyuh.cz, info@autosluzbyuh.cz
- **OT. doba:** Po–Čt 8:00–12:00, 12:30–17:00 / Pá 8:00–12:00, 12:30–15:00
- **Vozidla:** osobní, dodávkové, SUV a terénní
- **Firma od:** 2012

---

## Vizuální identita
### Fonty (finální)
- **Oswald** (nadpisy, 400–700) — kondenzovaný, razantní, automotive charakter
- **Manrope** (tělo, 300–700) — přesný, čitelný, moderní

### Paleta — "Precision & Trust"
| Proměnná | Hex | Role |
|----------|-----|------|
| `--dark` | #141B22 | Hero, nav, footer |
| `--dark-mid` | #1A2738 | Sekce kontakt, why |
| `--teal` | #14B8A6 | Primární akcent |
| `--teal-d` | #0D9488 | Hover |
| `--teal-l` | #CCFBF1 | Světlé teal plochy |
| `--concrete` | #F8FAFC | Světlé sekce |
| `--white` | #FFFFFF | Čistá bílá |
| `--text-dark` | #0F172A | Hlavní text |
| `--text-mid` | #475569 | Sekundární text |

### Archetype
**Precision & Trust** — moderní autoservis jako technologická firma

---

## Struktura webu (finální)
1. NAV — fixed, průhledný → dark on scroll, hamburger
2. HERO — teal glow dekorace (radial gradient), info panel vpravo
3. SLUŽBY — 6 karet v gridu (3×2), teal left border na hover
4. PROČ MY — dark sekce, 4 číslované benefity (01–04)
5. O NÁS — split: text + tým (František, Pavel Klas) + vozidla box
6. KONTAKT + HODINY — dark sekce, split layout
7. FORMULÁŘ — světlá sekce, intro vlevo + form vpravo
8. FOOTER — 3 sloupce, teal border-top

---

## Příští kroky
- [ ] Napojit formulář na Formspree (ID doplnit dle klienta)
- [ ] Ověřit OT. dobu s klientem

---

## Log změn
| Datum | Změna |
|-------|-------|
| 2026-03-25 | Inicializace projektu |
| 2026-03-25 | Scraping webu, analýza DNA souborů |
| 2026-03-25 | Kompletní index.html vytvořen |
| 2026-03-25 | Opravy po screenshotu: ikony, stats flex, grid 3×2, centrování karet, kontrast |
| 2026-03-25 | Stats sekce smazána, logo ikona → auto silueta |
| 2026-03-25 | Vozidla box ikony opraveny (sedan, dodávka, G-Wagon+rezerva) |
| 2026-03-25 | Font Syne → Oswald, nav logo text 1.65rem |
| 2026-03-25 | GitHub push, DNA soubor vytvořen |
