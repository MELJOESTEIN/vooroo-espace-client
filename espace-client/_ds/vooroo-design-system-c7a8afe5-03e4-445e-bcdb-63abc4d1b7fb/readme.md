# Vooroo Design System

## About Vooroo

Vooroo est une plateforme technologique nouvelle génération, conçue pour connecter partenaires, professionnels et utilisateurs autour d'une expérience commune de performance et de valeur partagée.

**Sources provided:**
- `uploads/Charte Graphique Vooroo_Juillet 2026.pdf` — Official brand guide (8 pages, Édition 2026)
- `uploads/Logo Vooroo-01.png` through `uploads/Logo Vooroo-08.jpg` — Full logo kit (8 variants)

No codebase, Figma link, or product screenshots were provided. UI kit and components are informed by the brand guide's aesthetic only.

---

## Brand Pillars

| Pillar | Description |
|---|---|
| **Performance** | Des résultats mesurables au service de nos partenaires |
| **Innovation** | Des solutions technologiques en constante évolution |
| **Partenariat** | La co-construction comme moteur de croissance |
| **Confiance** | Une relation de transparence et d'engagement durable |

**Brand signature:** *"Connectez. Performez. Grandissez."*

---

## CONTENT FUNDAMENTALS

**Language:** French-first brand. All official communications are in French; digital product may be multilingual.

**Tone:** Direct, confident, professional. Performance-oriented without being cold. The brand speaks to results and growth.

**Voice characteristics:**
- Assertive, action-forward: "Connectez. Performez. Grandissez." — three imperative verbs, no filler
- Short declarative sentences over long explanations
- No fluff, no excessive hedging
- Occasional warmth when addressing partnerships ("co-construction", "relation de transparence")

**Casing:** Display type (Bebas Neue) renders visually in uppercase due to the font. UI labels and body copy use sentence case. CTA buttons: uppercase or title case (consistent within context).

**Emoji:** Not used — brand is professional, tech-focused, and document-formal.

**Numbers:** Use figures (1, 2, 3), not words. Metric separators follow French convention (space as thousands separator).

**Examples of brand copy:**
- "L'identité visuelle officielle de la marque Vooroo — guide complet à l'usage des équipes et partenaires."
- "Connectez. Performez. Grandissez."
- "Une marque pensée pour inspirer la confiance, stimuler la croissance et incarner l'excellence technologique."

---

## VISUAL FOUNDATIONS

### Colors
- **Vert Vooroo #35AA47** — Primary brand green (brand guide value). Note: the real product UI uses **#27A36A** for active states (nav highlights, CTA buttons in the CRM) — both tokens are in `colors.css`.
- **Icon rail #1A1B5C** — Dark indigo used for the left icon navigation rail in the product (sampled from real screenshot). Not mentioned in the brand guide; added as `--color-rail`.

### Colors Used for primary actions, highlights, logo, backgrounds on hero/cover surfaces. Vibrant, mid-spectrum green evoking growth and tech vitality.
- **Noir Vooroo #111111** — Secondary. Used for dark backgrounds, text, premium contexts.
- **Blanc #FFFFFF** — Neutral. Primary background for light surfaces, inverse text on dark.
- **Gris Moyen #8A8A8A** — Neutral. Muted text, borders, secondary content. CMYK 0·0·0·46.
- **Gris Léger #F2F2F2** — Not in spec but inferred for subtle surface tinting.

### Typography
- **Display font: Bebas Neue Bold** — Used for all section titles, headings, display text. Renders as uppercase. Sizes: H1 48–72px, H2 32–48px, H3/Label 20–28px. Letter-spacing 0.02em.
- **Body font: Roboto Regular** — Used for body copy, UI text, navigation, subtitles. Sizes: body 16px, small 14px, xs 12px.
- No serif fonts. No handwritten or decorative type.

### Backgrounds
- Primary light surface: pure white `#FFFFFF`
- Dark/premium surface: `#111111` (Noir Vooroo)
- Brand accent surface: `#35AA47` (Vert Vooroo) — used full-bleed for covers and section starters
- No gradients — the brand uses flat, solid color surfaces
- No textures or patterns (beyond the subtle V-mark watermark used in the brand guide itself)

### Shapes & Geometry
- The logo mark is angular and geometric — diagonal cuts, sharp angles, no curves
- UI elements use minimal border radius (2–4px). Not rounded-pill style.
- Strong use of negative space

### Animations
- Not defined in the brand guide
- Inferred: clean, quick transitions (150–200ms ease). No bounces or spring physics — the brand is precise and performant.
- Hover states: slight color darkening on primary, no opacity tricks

### Hover / Press States
- **Primary button hover:** darken green to `#2A8C39`
- **Dark button hover:** `#1A1A1A`
- **Ghost/outline hover:** fill with green at low opacity or invert
- **Press states:** slightly deeper color shift, no shrink/scale effect (not a playful brand)

### Cards
- White background, `--shadow-sm` or 1px `#E0E0E0` border
- Border radius: 4–6px (minimal)
- Padding: 24px
- No colored left-border accent

### Borders & Dividers
- `1px solid #E0E0E0` for standard borders
- `2px solid #35AA47` for focus/active states
- Horizontal rules: thin, light grey

### Shadows
- Subtle, neutral-tone shadows (no colored shadows except green glow on special CTAs)
- `shadow-sm` for cards, `shadow-md` for elevated panels/modals

### Corner Radii
- Brand is angular — default radius is 2–4px
- No pill buttons unless used for tags/chips

### Iconography
See ICONOGRAPHY section below.

### Imagery
- Not shown in brand guide; no photography guidelines provided
- Inferred from brand context: clean product/tech imagery, possibly with cool-to-neutral color grading
- No hand-drawn illustrations visible in the brand guide

### Layout
- Brand guide uses a strong split-panel layout: 1/3 dark/green panel (left) + 2/3 white content (right)
- Generous whitespace
- Left-aligned content with consistent margins

### Transparency & Blur
- Not used in the brand guide; the aesthetic is clean and flat
- Avoid frosted glass / backdrop-blur effects (not on-brand)

---

## ICONOGRAPHY

No proprietary icon set is defined in the brand guide. The system uses **Lucide Icons** (CDN) as the recommended icon library — it matches the brand's clean, geometric, thin-stroke aesthetic.

CDN: `https://unpkg.com/lucide@latest`

Usage: `<i data-lucide="arrow-right"></i>` with `lucide.createIcons()`.

**Substitution note:** Lucide is an inferred addition — no official icon set was specified in the brand guide. If Vooroo has a proprietary icon set, provide it and it will replace this.

Emoji: Not used.
Unicode chars as icons: Not used.

---

## LOGO SYSTEM

### Logo variants (in `assets/`)

| File | Description |
|---|---|
| `logo-mark-green.png` | Symbol only, green on transparent |
| `logo-full-green.png` | Full wordmark, green on transparent |
| `logo-mark-white.png` | Symbol only, white on transparent |
| `logo-full-white.png` | Full wordmark, white on transparent |
| `logo-mark-on-black.jpg` | Symbol only, green on black |
| `logo-full-on-black.jpg` | Full wordmark, green on black |
| `logo-mark-bw.jpg` | Symbol only, white on black |
| `logo-full-bw.jpg` | Full wordmark, white on black |

### Usage rules
- **On white/light backgrounds:** green logo (logo-full-green.png)
- **On green backgrounds:** white logo (logo-full-white.png)
- **On dark/black backgrounds:** white or green logo (logo-full-white.png or logo-full-on-black.jpg)
- **Never:** grayscale, rotated, skewed, deformed, stretched, with borders/shadows/effects, on non-approved background colors
- **Min digital size:** 200px wide (full logotype), 80px (symbol only)
- **Min print size:** 40mm wide (full logotype), 15mm (symbol only)
- **Clear space:** X = height of the symbol; no element may enter this zone

---

## Components

| Component | File | Description |
|---|---|---|
| **Avatar** | `components/core/Avatar.jsx` | Initials avatar with deterministic color hash, sizes, online indicator |
| **Badge** | `components/core/Badge.jsx` | Status badge pill (success/warning/error/info/primary/dark) |
| **Button** | `components/core/Button.jsx` | CTA button (primary/secondary/ghost/ghost-dark/link, sm/md/lg) |
| **Card** | `components/core/Card.jsx` | Content surface (default/dark/green variants) |
| **Input** | `components/core/Input.jsx` | Text input with label, error, hint, prefix/suffix |
| **Tag** | `components/core/Tag.jsx` | Filter chip / label (active, removable, clickable) |



The following components were added because they are standard UI primitives required for building interfaces, not defined in the brand guide which covers only visual identity:

- **Button** — Core interactive primitive
- **Input** — Form text entry
- **Card** — Content container surface
- **Badge** — Inline status indicator
- **Tag** — Label/chip primitive
- **Lucide Icons** — Icon library (substitution; see ICONOGRAPHY)

---

## File Manifest

```
styles.css                  ← Entry point; @imports all token files
tokens/
  colors.css                ← Color tokens (base + semantic)
  typography.css            ← Font imports, type tokens
  spacing.css               ← Spacing scale
  effects.css               ← Shadows, radii, transitions
assets/
  logo-*.png / .jpg         ← 8 logo variants
components/core/
  Button.jsx + .d.ts        ← Button (primary/secondary/ghost, sm/md/lg)
  Input.jsx + .d.ts         ← Text input
  Card.jsx + .d.ts          ← Content card container
  Badge.jsx + .d.ts         ← Status badge
  Tag.jsx + .d.ts           ← Label chip
  Avatar.jsx + .d.ts        ← Initials avatar with deterministic color
  core.card.html            ← Component specimen card
  avatar.card.html          ← Avatar specimen card
guidelines/
  colors-primary.card.html  ← Vert Vooroo swatch
  colors-neutrals.card.html ← Neutral palette
  colors-semantic.card.html ← Semantic color aliases
  type-display.card.html    ← Bebas Neue display type
  type-body.card.html       ← Roboto body type
  type-scale.card.html      ← Full type scale
  spacing.card.html         ← Spacing scale
  effects.card.html         ← Shadows & radii
  brand-logo.card.html      ← Logo variants
  brand-signature.card.html ← Brand mark & tagline
  brand-voice.card.html     ← Voice & tone specimen
ui_kits/platform/
  index.html                ← Interactive platform dashboard (partner management)
ui_kits/crm/
  index.html                ← CRM contacts view (matches real product — Personnes screen)
thumbnail.html              ← Design system tile
readme.md                   ← This file
SKILL.md                    ← Agent skill descriptor
```
