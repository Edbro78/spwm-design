# Söderberg & Partners Wealth Management — Design

Enhetlig designreferanse for SPWM-designsystemet, samlet fra filene i dette repoet (`SPWM mal/`, `Designsystem/`).

---

## Oversikt

| | |
|---|---|
| **Produkt** | Klientportal for formuesforvaltning (Wealth Management) |
| **Merkevare** | Söderberg & Partners Wealth Management |
| **Språk** | Norsk bokmål |
| **Uttrykk** | Eksklusivt, moderne, rent — nordisk institusjonell fintech |
| **Figma** | [Designsystem](https://www.figma.com/design/JZYh8Qbm5Ba8ddKREjpebv/Designsystem?node-id=51-513&m=dev) · [Prototype](https://www.figma.com/proto/JZYh8Qbm5Ba8ddKREjpebv/Designsystem?node-id=51-513) |
| **File key** | `JZYh8Qbm5Ba8ddKREjpebv` · node `51:513` |

**Ikke-forhandlingsbare regler**

- Navy `#002359` er blekk / merkevarefarge
- Blå `#0A5EDC` er den ene action-fargen
- Norsk bokmål, setningscase, tusenskille med mellomrom + `kr`, fortegn på %
- Ikoner via Boxicons (`bx bx-*`) — ingen emoji
- Flat bakgrunn — ingen gradienter på overflater
- Rolig, presis, rådgivende tone

---

## Produkt og skjermer

Klientportal med venstre sidebar (280px, hvit) og hovedflate på canvas `#F9FAFB` med 24px avrundet øvre venstre hjørne.

| Skjerm | Innhold |
|---|---|
| **Login** | Delt navy brand-panel + e-post/passord + BankID |
| **Hjem / Oversikt** | Hilsen, KPI-kort (Investeringer & Pensjon), allokering, nyheter |
| **Investeringer** | Performance-graf, periodevalg, allokering, beholdningstabell |
| **Pensjon** | Pensjonsgraf, avtaleliste, estimert pensjon |
| **Dokumenter** | Dokumentliste med type/dato/størrelse og nedlasting |
| **Rådgiver** | Rådgiverkort + «Book et møte» |
| **Tilbakemelding** | Feedback |
| **Mobil** | Topnavbar med logomark, klientvelger og hamburger (&lt; 900px) |

Page header: 30px navy-tittel + myk blå «Rapporteringsdato»-badge.

---

## Innhold og tone

| Norsk | Engelsk |
|---|---|
| Hjem / Oversikt | Home / Overview |
| Investeringer | Investments |
| Pensjon | Pension |
| Dokumenter | Documents |
| Beholdning | Holdings |
| Rådgiver / Rådgivere | Advisor / Advisors |
| Tilbakemelding | Feedback |
| Klientvelger | Client selector |
| Min side | My page |
| Logg ut | Log out |
| Totalverdi | Total value |
| Avkastning siden start | Return since inception |
| Markedsverdi | Market value |
| Fordeling / Aktivklasser | Allocation / Asset classes |
| Rapporteringsdato | Reporting date |
| Avbryt / Lagre / Slett | Cancel / Save / Delete |
| Se detaljer | See details |

- **Tone:** rolig, presis, rådgivende — aldri selgende eller leken
- **Person:** diskret «din/dine» («Dine rådgivere»)
- **Casing:** setningscase overalt (overskrifter, knapper, nav)
- **Tall:** `6 002 474 kr` · `+26,12 %` · `−14,51 %`
- **Eksempler:** «Totalverdi — 6 002 474 kr» · «Rapporteringsdato: 02.06.2024» · «Se detaljer om investeringer →»

---

## Farger

### Merkevare

| Token | Hex | Bruk |
|---|---|---|
| `--sp-navy` | `#002359` | Logo, overskrifter, brødtekst, ikoner, aktiv nav-tekst |
| `--sp-navy-ink` | `#12326E` | Logo-skille / dype aksenter |
| `--sp-navy-pressed` | `#074EB9` | Dyp interaktiv blå (hover/pressed) |
| `--blue-main` / `--blue-800` | `#0A5EDC` | Primærknapp, lenker, fokus, valgt, chart-linjer |

### Blå-skala (action)

| 25 | 50 | 100 | 200 | 300 | 400 | 500 | 600 | 700 | 800 |
|---|---|---|---|---|---|---|---|---|---|
| `#F9FBFE` | `#F3F7FD` | `#EEF5FF` | `#E6EFFB` | `#B5CFF5` | `#99BEF5` | `#84AEED` | `#6096E8` | `#3B7EE3` | `#0A5EDC` |

### Sekundær (navy-grå)

| 25 → 800 |
|---|
| `#F6F7F9` · `#F2F4F7` · `#ECEFF3` · `#E5E9EE` · `#CCD3DE` · `#A0AEC4` · `#8091AC` · `#597093` · `#405A82` · `#264472` |

### Nøytral grå

| 25 → 900 |
|---|
| `#FCFCFD` · `#F9FAFB` · `#F2F4F7` · `#EAECF0` · `#D0D5DD` · `#98A2B3` · `#667085` · `#475467` · `#344054` · `#1D2939` · `#101828` |

`--white` `#FFFFFF` · `--black` `#161616` · canvas `--gray-50` `#F9FAFB`

### Semantisk

| Rolle | Text | Action | Border | Background |
|---|---|---|---|---|
| Error | `#B42318` | `#D92D20` | `#FDA29B` | `#FEF3F2` |
| Warning | `#B54708` | `#DC6803` | `#FEC84B` | `#FFFAEB` |
| Success | `#067647` | `#079455` | `#A6F4C5` | `#ECFDF3` |

Positiv avkastning = grønn · negativ = rød.

### Diagram

| Token | Hex |
|---|---|
| `--chart-blue` | `#0A5EDC` (pensjon) |
| `--chart-violet` | `#9747FF` (investeringer) |
| `--chart-navy` | `#002359` |
| `--chart-positive` | `#079455` |
| `--chart-negative` | `#D92D20` |
| `--chart-grid` | `#EAECF0` |

### Semantiske roller

| Token | Verdi |
|---|---|
| `--fg` | navy (standard blekk) |
| `--fg-muted` / `--fg-subtle` | gray-600 / gray-500 |
| `--fg-link` | blue-main |
| `--bg` / `--bg-subtle` | white / gray-50 |
| `--bg-brand-soft` | blue-100 (aktiv nav) |
| `--border` / `--border-strong` | gray-200 / gray-300 |
| `--ring` | `rgba(10,94,220,0.24)` |

---

## Typografi

| Familie | Token | Merknad |
|---|---|---|
| **Whitney** (produkt) | — | Hoefler&Co — ikke fri |
| **Hanken Grotesk** | `--font-sans` / `--font-display` | Erstatning i dette systemet |
| **SoderbergSans** (kun italic) | `--font-italic` | Light/Regular/Medium/Bold/Black italic OTF |
| Inter | fallback | — |

**Vekter:** Book 400 · Medium 500 · Semibold 600 · Bold 700

### Display-skala

| Steg | Størrelse | Linjehøyde | Tracking |
|---|---|---|---|
| xl | 60px | 72px | −2% |
| lg | 48px | 60px | −2% |
| md | 36px | 44px | −2% |
| sm | 30px | 38px | 0 |
| xs | 24px | 32px | 0 |

### Text-skala

| Steg | Størrelse | Linjehøyde |
|---|---|---|
| xl | 20px | 30px |
| lg | 18px | 28px |
| md | 16px | 24px |
| sm | 14px | 20px |
| xs | 12px | 18px |

Overskrifter: Medium-vekt navy. Tall/totaler: Semibold.

---

## Spacing, radius, elevation

**Spacing (4px-grid):** 4 · 8 · 12 · 16 · 20 · 24 · 32 · 40 · 48 · 64 · 80  
Typisk: 24–40px page padding · 24px mellom kort · 12px mellom nav-items

| Radius | Verdi | Bruk |
|---|---|---|
| xs | 4px | — |
| sm | 5px | Button-group container |
| md | 8px | Knapper, inputs |
| lg | 12px | Kort |
| xl | 16px | — |
| 2xl | 24px | App main container (øvre venstre) |
| pill | 100px | Ikonknapper, badges, avatarer |

| Shadow | Bruk |
|---|---|
| xs / sm | Kort (ofte bare border + sm) |
| md | Mellomnivå |
| lg / xl | Popovers, menyer, modaler |

Struktur formidles med 1px border + whitespace mer enn skygge. Flat farge — ingen gradienter.

---

## Komponenter

### Knapper

| Variant | Stil |
|---|---|
| Primary | `#0A5EDC` → hover `#074EB9` · hvit tekst |
| Secondary | Hvit · navy tekst · gray-300 border |
| Tertiary | Transparent · blå tekst · soft blue hover |
| Destructive | `#B42318` · outline-variant med error-border |
| Størrelser | md (11×18 padding, 16px) · sm (9×14, 14px) |
| Radius | 8px · Semibold |

### Input

Høyde 44px · radius 8px · border gray-300 · fokus: blue border + 4px ring · feil: error-500

### Badge / chip

Pills (100px radius) · toner: brand, success, error, warning, neutral, secondary

### Kort

Hvit · 12px radius · gray-200 border · 16–24px padding  
KPI: label → stort Semibold-tall → fortegnsavkastning → sparkline

### Navigasjon

| Tilstand | Stil |
|---|---|
| Default | Navy/grå tekst |
| Hover | soft gray-50 / blue-100 |
| Selected | blue-100 bakgrunn + navy tekst/ikon |
| Fokus | 2px blue ring (`--ring`) |

### Diagrammer

Rene linjediagrammer (tynn stroke, soft area fill, minimal akser) · doughnut for allokering i blå-familien + tabell

### Interaksjon og motion

- Hover/active uten scale/bounce
- Motion: 150–250ms fade/slide, ease-out
- Respekter `prefers-reduced-motion`
- Ingen emoji, ingen dekorativ animasjon

---

## Ikonografi

Boxicons CDN: `https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css`  
Standard: `bx bx-*` (outline) · solid (`bxs-*`) kun der Figma gjør det

| Nav | Ikon |
|---|---|
| Hjem | `bx-home-alt-2` |
| Investeringer | `bx-pie-chart-alt-2` |
| Pensjon | `bx-wallet` |
| Dokumenter | `bx-file` |
| Tilbakemelding | `bx-edit-alt` |
| Klientvelger | `bx-group` |
| Min side | `bx-user` |
| Logg ut | `bx-log-out` |
| Rapporteringsdato | `bx-info-circle` |

---

## Visuelle assets

| Fil | Beskrivelse |
|---|---|
| `SPWM mal/assets/spwm-logo.svg` | Horisontal lockup (navy) |
| `SPWM mal/assets/spwm-logo-white.svg` | Hvit knockout |
| `SPWM mal/assets/spwm-mark.svg` | Logomark navy |
| `SPWM mal/assets/spwm-mark-white.svg` | Logomark hvit |
| `SPWM mal/fonts/SoderbergSans-*Italic.otf` | 5 italic-vekter |
| `Designsystem/cover.webp` | Figma cover/thumbnail |

Clear space = wordmark cap-height rundt logo. Min. høyde ~20px. Ikke omfarge eller forvrenge.

---

## Layout-skall

```
┌────────────┬──────────────────────────────────────┐
│ Sidebar    │ Main canvas #F9FAFB                  │
│ 280px hvit │ border-radius 24px (top-left)        │
│            │                                      │
│ Logo       │ Page header (tittel + dato-badge)    │
│ Nav items  │                                      │
│            │ Cards / charts / tables              │
│ ─────────  │                                      │
│ Klientvelger                                      │
│ Min side / Logg ut                                │
└────────────┴──────────────────────────────────────┘
```

---

## UI Kit — Wealth Portal

Sti: `SPWM mal/ui_kits/wealth-portal/`  
Åpne `index.html` → Login → Logg inn → sidebar-navigasjon.

| Fil | Innhold |
|---|---|
| `primitives.jsx` | Button, Badge, Avatar, Input, Card, Icon, `nok()` / `pct()` |
| `charts.jsx` | LineChart, Doughnut |
| `shell.jsx` | Sidebar, NavItem, ClientSelector, PageHeader, MobileTopbar |
| `cards.jsx` | KpiCard, NewsCard, AdvisorCard, SectionTitle, DetailLink |
| `tables.jsx` | AssetAllocation, HoldingsTable |
| `screens.jsx` | Hjem, Investeringer, Pensjon, Dokumenter, Rådgiver |
| `app.jsx` | Login, Portal, router |
| `data.jsx` | Sample data |

---

## Design tokens (kilde)

Importer alltid:

```text
SPWM mal/colors_and_type.css
```

CSS-klasser: `.sp-display-xl` … `.sp-display-xs` · `.sp-text-xl` … `.sp-text-xs` · `.sp-w-book|medium|semibold|bold`

---

## Repo-struktur

```text
spwm-design/
├── design.md                 ← denne filen
├── Designsystem/             ← Figma-referanse (lenker + cover)
│   ├── README.md
│   ├── figma.json
│   └── cover.webp
└── SPWM mal/                 ← designsystem + UI kit
    ├── README.md
    ├── SKILL.md
    ├── colors_and_type.css
    ├── assets/
    ├── fonts/
    ├── preview/              ← spec-kort (brand, farger, type, komponenter)
    └── ui_kits/wealth-portal/
```

### Preview-kort (`SPWM mal/preview/`)

Brand · Colors (brand, blue, gray, secondary, semantic) · Type (typeface, display, text, italic) · Spacing (scale, radius, elevation) · Components (buttons, badges, inputs, KPI, nav)

### Figma-sider (kilde)

Foundations · Colors · Spacing · Typography · Brand-assets · Buttons-and-links · Cards · Inputs · Navigation · Page-template · Page-header · Data-visualization · Tables · Badge · Banner · Modals · Tabs · Dropdown · Stepper · Switch-toggle · Radio-checkbox · Tooltip · Datepicker

---

## Caveats

1. **Whitney** er ikke inkludert — Hanken Grotesk er stand-in.
2. **SoderbergSans** har kun italic-vekter — ikke bruk til brødtekst.
3. UI-kitet er kosmetisk prototype (sample data), ikke produksjonskode.
4. Figma-filen er view-link; full canvas-eksport krever Figma-token eller manuelle eksporter.

---

*Samlet fra `SPWM mal/` (README, SKILL, colors_and_type.css, _ds_manifest.json, UI kit) og `Designsystem/` (figma.json).*
