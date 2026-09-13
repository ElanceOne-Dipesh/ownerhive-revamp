# OwnerHive Brand & UI Skills Guide

Visual system with cool off-white canvas, charcoal DM Sans typography, and a blue→magenta accent for CTAs, hover, and elevation.

---

## 1. Color System

### Core Brand Colors

| Token | Value | Role |
|-------|-------|------|
| **Theme blue** | #0F58B6 | Nav hover, icons, footer, selection |
| **Hive blue** | #126BDC | CTA start, forms, icon wells |
| **Magenta** | #CD5FFF | CTA end, table wash, shadows |
| **Bright blue** | #0089F7 | Feature-card hover border |

### Surface Colors

| Token | Value | Role |
|-------|-------|------|
| **Page** | #FCFCFC | HTML / wrapper / header background |
| **Ice** | #F4F9FF | Hero dividers, product panel |
| **Card fill** | #F3F4F4 | Benefit tiles, outline border |
| **Card stroke** | #E6E8EE | Feature cards 2px border |

### Text Colors

| Token | Value | Role |
|-------|-------|------|
| **Ink** | #2E2E2E | Body, headings, default links |
| **Input** | #576679 | Form field text |
| **Placeholder** | #929292 | Empty field hint |
| **Footer link** | #C9E1FF | Menus on blue footer |

### CSS Variables & Tokens

| Token | Value | Role |
|-------|-------|------|
| `--mfn-button-bg` | #126BDC | Solid fallback under CTA gradient |
| `--mfn-button-bg-hover` | #00B7FF | Solid hover fallback |
| **CTA gradient** | 90° #126BDC → #CD5FFF 70% | Primary buttons |
| **CTA hover gradient** | 90° #0F58B6 → #B114FA 70% | Primary :hover |
| **Section wash** | rgba(15,88,182,0.09) | Alternating bands |
| **Header hairline** | #0F58B617 | 80px header bottom border |
| **Magenta wash** | #CD5FFF24 | Comparison-table header |
| **Table border** | #DAE9FF | Comparison table lines |
| **Footer bar** | #0F58B6 | Main footer |
| **Footer copyright** | #05489E / #053571 | Bottom strip + overlay |
| **Side slide** | #0F2036 / #D6DDE4 | Mobile drawer |
| **Selection** | #0F58B6 on white | ::selection |

---

## 2. Typography

**Typeface:** DM Sans (Google Fonts)  
**Weights:** 100 / 300 / 400 / 400 italic / 500 / 700 / 700 italic / 900

**Rule:** Body tracking is open at 1px — keep that on paragraphs, not on display headings. Headings stay charcoal; blue is reserved for hover and UI chrome.

### Type Scale

| Level | Size / Line / Weight | Tracking | Sample |
|-------|----------------------|----------|--------|
| H1 | 64 / 77 / 900 | 0px | Streamlined management |
| H2 | 48 / 58 / 600 | 0px | Our Platform in Numbers |
| H3 | 26 / 38 / 600 | 0px | Social Media Management |
| H4 | 24 / 36 / 600 | 0px | Everything You Need |
| H5 / eyebrow | 16 / 25 / 600 | 0px | Manage Your Entire Business |
| H6 | 14 / 26 / 600 | 1px | From active users to scheduled posts |
| Body | 16 / 28 / 400 | 1px | Join thousands of businesses… |
| Lead | 17 / 29 / 400 | 1px | No credit card required. |
| Nav / button | 16 / 28 / 600 | 1px | Book A Demo |

### Responsive Type Scale

| Breakpoint | H1 | H2 | Body |
|------------|-----|-----|------|
| Desktop (≥960px) | 64 / 77 / 900 | 48 / 58 / 600 | 16 / 28 / 400 |
| Tablet (768–959px) | 54 / 65 / 900 | 41 / 49 / 600 | 14 / 24 / 400 |
| Small (480–767px) | 48 / 58 / 900 | 36 / 44 / 600 | 13 / 21 / 400 |
| Mobile (≤479px) | 38 / 46 / 900 | 29 / 35 / 600 | 13 / 19 / 400 |

---

## 3. Buttons

**Shared CSS variables on body.** Primary buttons are pills with a horizontal blue→magenta fill. Do not use a flat blue fill for the main CTA — the gradient is the brand mark.

### Button Styles

#### Primary CTA
- **Gradient:** #126BDC → #CD5FFF
- **Hover:** #0F58B6 → #B114FA
- **Shape:** Pill (50px radius)

#### Outline / Theme
- **Fill:** Transparent
- **Border:** 1px #F3F4F4
- **Usage:** On dark/blue bands

#### Action / Ghost
- **Fill:** #FCFCFC
- **Border:** Ink 1px
- **Hover:** Text/border #0F58B6

### Button Properties

| Property | Value |
|----------|-------|
| Font | DM Sans / 16px / 600 / 1px tracking |
| Padding | 16px 35px |
| Radius | 50px (full pill) |
| Border | 1px, transparent on primary |
| Icon gap | 10px |
| Transition | 0.3s |
| Box shadow | none |

---

## 4. Layout

### Page Frame

| Token | Value |
|-------|-------|
| **Wrapper max** | 1248px (≥1240px) |
| **Section / container** | 1228px |
| **Header height** | 80px, sticky |
| **Logo slot** | 178px desktop / 50px mobile |
| **Header border** | 1px #0F58B617 bottom |
| **Section padding** | 70px typical; hero 50px |
| **Footer padding** | 80px 0 40px, then 30px bars |

### Breakpoints

| Name | Width |
|------|-------|
| Mobile | ≤479px |
| Phablet | 480–767px |
| Tablet | 768–959px |
| Laptop | 960–1239px |
| Desktop | ≥1240px |
| Wide tweak | 960–1440 (section padding 0) |

**Content structure:** Full-bleed bands (ice, blue wash, page) with an inner 1228px column. Feature grids are 3 columns. Shape-divider SVGs transition between #F4F9FF and #FCFCFC.

---

## 5. Components

### Header
- Off-white bar, 80px, hairline blue border
- Nav links: ink / 600; hover and current item theme blue
- Logo left, menu right
- Sticky header keeps the same fill
- Mobile drawer: navy #0F2036 with #D6DDE4 links

### Feature Card
- **Border:** 2px #E6E8EE
- **Radius:** 20px
- **Padding:** 60px 12% 45px
- **Hover:** #0089F7 border
- **Shadow:** 0 10px 10px rgba(205,95,255,0.12)

### Icon Box (Product Tabs)
- **Icon well:** 50×60px, theme blue, 20px radius, 30px white glyph
- **Title:** 16px / 600 ink
- **Description:** 14px
- **Tile radius:** 20px
- **Tile padding:** 12px
- **Hover fill:** #0F58B617
- **Parent split:** White list vs ice #F4F9FF panel, 32px padding, 300px min height
- **Drop shadow:** 0 35px 36px rgba(15,88,182,0.12)

### Benefit Tile
- **Fill:** #F3F4F4
- **Radius:** 8px
- **Padding:** 50px 13% 35px
- **Shadow:** 0 10px 10px rgba(205,95,255,0.12)

### Comparison Table
- **Outer radius:** 20px
- **Border:** 1px #DAE9FF
- **Cell padding:** 24px
- **Header fill:** #CD5FFF24
- **Odd rows:** #FCFCFC
- **Even rows:** Blue wash
- **Headers:** 26px / 600

### Footer
- **Solid fill:** #0F58B6
- **Heading:** White / 500
- **Menu links:** #C9E1FF
- **CTA panel:** Blue fill, 15px radius, 32×40 padding
- **CTA shadow:** 0 16px 48px rgba(15,88,182,0.12)
- **Copyright strip:** #05489E over #053571
- **Back-to-top:** #0F58B6 with #FCFCFC icon

---

## 6. Elevation, Motion & Forms

### Shadow Effects

| Effect | Value | Where |
|--------|-------|-------|
| **Magenta lift** | 0 10px 10px rgba(205,95,255,0.12) | Feature cards, benefit tiles |
| **Magenta bloom** | 0 16px 48px rgba(205,95,255,0.12) | .video-tab |
| **Blue lift** | 0 35px 36px rgba(15,88,182,0.12) | Product-tab shell |
| **Blue bloom** | 0 16px 48px rgba(15,88,182,0.12) | CTA banner |

### Radius Scale

| Size | Value | Usage |
|------|-------|-------|
| S | 8px | Tiles |
| M | 15px | CTA |
| L | 20px | Cards |
| Pill | 50px | Buttons |

### Motion

| Property | Value | Where |
|----------|-------|-------|
| **Transition** | 0.3s | Buttons |

### Forms

- **Underline-only fields:** border-width 0 0 1px 0, no shadow, transparent fill
- **Border and focus color:** #126BDC
- **Value color:** #576679 → #126BDC on focus
- **Placeholder:** #929292
- **No resize:** Textareas

---

## 7. Do & Don't

### ✅ Do

- Use DM Sans only. Pair 900 display with 400 body.
- Keep primary actions as pills with the blue→magenta sweep.
- Alternate page white with 9% blue wash, not gray slabs.
- Tint shadows magenta on product UI, blue on chrome.
- Center section titles; left-align card copy.
- Number features 01–06 in 600 weight ink.

### ❌ Don't

- Don't introduce a second typeface or condensed tracking on body.
- Don't use sharp rectangles for CTAs — they are always pills.
- Don't set heading color to blue; ink stays charcoal until hover.
- Don't drop heavy black shadows; brand elevation is 12% tinted.
- Don't fill the page with #FFFFFF — the canvas is #FCFCFC.
- Don't use Gutenberg preset pinks/oranges; they are unused.

---

## Implementation Notes

**Stack:** WordPress on Betheme (Muffin Group) with a near-empty child theme

**Brand location:** Theme options + BeBuilder local CSS, not a design-token file

**To reimplement:** Copy the CSS variables on `body` and the homepage color / radius / shadow recipes from this guide.

---

*Extracted from https://ownerhive.com/ · August 2026*
