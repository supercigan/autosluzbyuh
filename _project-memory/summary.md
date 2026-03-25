# Projekt: Autoslužby UH s.r.o.
**Datum zahájení:** 2026-03-25

---

## Co je hotovo
- [x] Inicializace projektu, _project-memory/summary.md
- [x] Přečteny všechny DNA soubory (6 projektů) — zaznamenáno co NEpoužívat
- [x] Scraping reálného webu autosluzbyuh.cz — získány všechny info
- [x] Navržena vizuální identita (fonty, paleta, archetype)
- [x] Vytvořen kompletní index.html — jednostránkový web

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
### Fonty
- **Syne** (nadpisy, 800/700/600) — geometrický, technický, moderní. Dosud nepoužitý v žádném projektu.
- **Manrope** (tělo, 300–700) — přesný, čitelný, moderní. Dosud nepoužitý.

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

**Odlišení od DNA:**
- NE amber (M-autoservis), NE červená (O.K. autoservis), NE bronz (Zámečnictví)
- Teal = svěží, technologický, důvěryhodný → automotive přesnost, ne agresivita

### Archetype
**Precision & Trust** — moderní autoservis jako technologická firma

---

## Struktura webu
1. NAV — fixed, průhledný → dark on scroll, hamburger
2. HERO — teal glow dekorace (radial gradient), info panel vpravo
3. STATS — teal pruh, 4 statistiky
4. SLUŽBY — 5 karet v gridu (3+2), teal left border na hover
5. PROČ MY — dark sekce, 4 číslované benefity (01–04)
6. O NÁS — split: text + tým (František, Pavel Klas) + vozidla box
7. KONTAKT + HODINY — dark sekce, split layout
8. FORMULÁŘ — světlá sekce, intro vlevo + form vpravo
9. FOOTER — 3 sloupce, teal border-top

---

## Odlišující prvky od DNA projektů
- **Hero efekt:** radial teal glow (ne canvas dots jako M-auto, ne grid texture jako O.K.)
- **Hero info panel:** vpravo s kontakty (jinak strukturovaný než O.K.)
- **Stats pruh:** teal bar (nové, žádný předchozí projekt tohle neměl)
- **Tým sekce:** František a Pavel Klas s avatary (unikátní, žádný předchozí projekt)
- **Vozidla box:** vizuální ikonky typů vozidel (unikátní)
- **Service grid s border separátory:** jiný než karty M-autoservisu
- **Teal border-top footer** (vs. červená u O.K.)

---

## Technický stack
- HTML/CSS/JS — jeden soubor index.html
- Google Fonts: Syne + Manrope
- Formulář: lokální simulace (Formspree lze napojit)
- IntersectionObserver fade-up animace
- ScrollSpy pro nav highlight

---

## Co se řeší
- GitHub push — repo vytvořit a pushnut

---

## Důležitá rozhodnutí
- Teal jako primární akcent — unikátní v kontextu všech DNA projektů (autoservisy i wellness)
- Syne + Manrope — nová kombinace, neobjevená v žádném předchozím projektu
- Team sekce (František + Pavel Klas) — humanizuje firmu, unikátní prvek
- Stat pruh za hero — dává firmě váhu bez velkých textů

---

## Příští kroky
- [x] GitHub push → Vercel deploy
- [ ] Napojit formulář na Formspree (ID doplnit dle klienta)
- [ ] Ověřit OT. dobu s klientem
- [ ] DNA soubor po dokončení projektu

---

## Log změn
| Datum | Změna |
|-------|-------|
| 2026-03-25 | Inicializace projektu |
| 2026-03-25 | Scraping webu, analýza DNA souborů |
| 2026-03-25 | Kompletní index.html vytvořen (hero, stats, služby, proč my, o nás, kontakt, formulář, footer) |
