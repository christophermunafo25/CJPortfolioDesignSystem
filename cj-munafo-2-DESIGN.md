# CJ Munafo — Style Reference
> Creative strategy built to land

**Theme:** dark

CJ Munafo's portfolio is a high-voltage personal brand that pairs an electric chartreuse accent against near-black surfaces, communicating bold creative authority. The dark hero canvas gives way to a light inner-page system — white cards float over a warm off-white ground — creating a dual-mode aesthetic that feels both edgy and professional. Heavy condensed display type screams confidence while clean body copy invites genuine reading. Every interaction reinforces a singular message: this is a strategist who knows exactly what they are doing.

## Tokens — Colors

| Name | Value | Token | Role |
|------|-------|-------|------|
| Slate Mist | `#808080` | `--color-slate-mist` | Secondary body copy. Muted descriptive paragraphs and supporting text on both light and dark backgrounds. |
| Void Black | `#1a1a1a` | `--color-void-black` | Hero canvas & dark surface. The dominant background of the hero section and dark-mode surfaces throughout. |
| Warm Paper | `#f8f7f5` | `--color-warm-paper` | Page canvas & card ground. The lightest surface — used as the base page background in light sections and as a near-white body copy tone on dark backgrounds. |
| Cinder Dark | `#231f23` | `--color-cinder-dark` | Navigation bar & secondary dark surface. The slightly warm near-black used behind the nav pill and secondary dark components. |
| Ghost White | `#ffffff` | `--color-ghost-white` | Primary light text & headings. High-contrast type against dark backgrounds, used for all hero headlines and reversed copy. |
| Arctic Spark | `#00d4ff` | `--color-arctic-spark` | Secondary decorative accent. Social media icon highlights and rare secondary accent moments — never used for CTAs. |
| Charcoal Ink | `#4d4d4d` | `--color-charcoal-ink` | Body copy on light backgrounds. Main readable paragraph text within card and content sections. |
| Electric Lime | `#c4ff00` | `--color-electric-lime` | Primary CTA & brand accent. All interactive buttons, logo mark highlights, and hover states — the single saturated note in an otherwise dark palette. |
| Smoke Overlay | `#f8f7f5bf` | `--color-smoke-overlay` | Body copy on dark backgrounds. Semi-transparent warm white that softens long-form text against hero darkness. |

## Tokens — Typography

### Kurdis Text — Body and UI typeface. Clean humanist sans used for all paragraph copy, navigation links, card descriptions, and form labels. · `--font-kurdis`
- **Substitute:** Arial, sans-serif
- **Weights:** 300, 400, 500
- **Sizes:** 13px, 14px, 16px, 18px, 20px
- **Line height:** 1.40, 1.50, 1.60
- **Letter spacing:** 0em, 0.01em
- **Role:** Body and UI typeface. Clean humanist sans used for all paragraph copy, navigation links, card descriptions, and form labels.

### Helvena Bold — Primary display and heading typeface. Condensed, uppercase grotesque used for all hero headlines, section titles, and CTA labels — projects loud creative confidence. · `--font-helvena`
- **Substitute:** Arial, sans-serif
- **Weights:** 400, 700, 900
- **Sizes:** 12px, 14px, 24px, 32px, 48px, 64px, 80px
- **Line height:** 1.00, 1.05, 1.10
- **Letter spacing:** 0em, 0.02em, 0.05em
- **Role:** Primary display and heading typeface. Condensed, uppercase grotesque used for all hero headlines, section titles, and CTA labels — projects loud creative confidence.

### Fragment Mono — Eyebrow and detail labels. Used for small caps eyebrow tags, metadata, and subtle technical accents — adds a systematic, analytical texture. · `--font-fragment-mono`
- **Substitute:** monospace
- **Weights:** 400
- **Sizes:** 11px, 12px
- **Line height:** 1.20
- **Letter spacing:** 0.05em, 0.1em
- **Role:** Eyebrow and detail labels. Used for small caps eyebrow tags, metadata, and subtle technical accents — adds a systematic, analytical texture.

### Type Scale

| Role | Size | Line Height | Letter Spacing | Token |
|------|------|-------------|----------------|-------|
| caption | 11px | 1.2 | 0.08em | `--text-caption` |
| body-sm | 13px | 1.5 | 0em | `--text-body-sm` |
| body | 14px | 1.5 | 0em | `--text-body` |
| body-lg | 16px | 1.6 | 0em | `--text-body-lg` |
| heading-sm | 20px | 1.2 | 0.02em | `--text-heading-sm` |
| heading | 32px | 1.1 | 0.01em | `--text-heading` |
| heading-lg | 48px | 1.05 | 0em | `--text-heading-lg` |
| display-sm | 64px | 1 | -0.01em | `--text-display-sm` |
| display | 80px | 1 | -0.02em | `--text-display` |

## Tokens — Spacing & Shapes

**Base unit:** 8px

**Density:** comfortable

### Spacing Scale

| Name | Value | Token |
|------|-------|-------|
| 4 | 4px | `--spacing-4` |
| 8 | 8px | `--spacing-8` |
| 12 | 12px | `--spacing-12` |
| 16 | 16px | `--spacing-16` |
| 24 | 24px | `--spacing-24` |
| 32 | 32px | `--spacing-32` |
| 48 | 48px | `--spacing-48` |
| 64 | 64px | `--spacing-64` |
| 80 | 80px | `--spacing-80` |
| 96 | 96px | `--spacing-96` |
| 128 | 128px | `--spacing-128` |

### Border Radius

| Element | Value |
|---------|-------|
| pill | 9999px |
| cards | 16px |
| large | 32px |
| small | 8px |
| medium | 16px |
| buttons | 8px |
| nav-pill | 20px |
| cards-large | 24px |

### Layout

- **Page max-width:** 1140px
- **Section gap:** 80px
- **Card padding:** 24px
- **Element gap:** 16px

## Tokens — Shadows

| Name | Value | Role |
|------|-------|------|
| nav-glow | `0 4px 80px rgba(35,31,35,0.08)` | Soft drop shadow beneath the navigation bar pill — anchors the floating nav without creating visual noise. |
| card-float | `0 8px 50px rgba(0,0,0,0.05)` | Subtle lift for white cards on the warm-paper background — keeps surfaces feeling airy without heavy drama. |
| inset-border | `inset 0 0 0 1px rgba(244,243,234,0.08)` | Hairline inset border on dark surface cards — defines card edges on near-black backgrounds without a hard stroke. |

## Tokens — Motion

| Name | Duration | Easing | Role |
|------|----------|--------|------|
| micro | 200ms | `cubic-bezier(0.2, 0, 0, 1)` | Button hover states, color transitions — snappy, immediate feedback for interactive elements. |
| reveal | 300ms | `cubic-bezier(0.4, 0, 0.2, 1)` | Dropdown menus and panel reveals — smooth but never sluggish. |

## Tokens — Breakpoints

- **lg:** 1440px
- **md:** 991px
- **sm:** 767px
- **xl:** 1920px
- **xs:** 479px

## Do's and Don'ts

### Do
- Use Electric Lime (#c4ff00) exclusively for primary CTAs, button fills, and the logo bolt mark — it must remain the single saturated color on dark canvases.
- Set all hero and dark-section headlines in Helvena at weight 900, uppercase, with tight letter-spacing (-0.01em to -0.02em) to maintain the compressed power of the display type.
- Apply a 16px border-radius to work cards and service panels on the light inner-page sections, maintaining the soft-but-solid card aesthetic.
- Use the warm paper (#f8f7f5) as the base canvas for all inner-page light sections — never use pure #ffffff as a page background, only as a lifted card surface.
- Render the '+' plus-icon eyebrow pill (dark background, white text, rounded pill shape with fully rounded radius) before all section labels to retain the brand's signature tag motif.
- Keep body copy in Kurdis at weight 300–400 with 1.5–1.6 line-height; let breathing room carry the text, never tighten paragraphs.
- Maintain the dual-mode aesthetic: dark hero section at page top, light warm-paper body below — this contrast is central to the visual identity.

### Don't
- Never introduce additional saturated accent colors (red, orange, purple, blue) — the palette is intentionally monochrome with a single Electric Lime accent.
- Do not use Electric Lime (#c4ff00) for body text or decorative fills — it is reserved strictly for interactive CTAs and the brand mark.
- Avoid applying Helvena to body copy or UI labels — it belongs only at display and heading sizes where its condensed weight reads as power, not noise.
- Do not use pure #000000 black as a background — the brand's dark surfaces are always #1a1a1a or #231f23, preserving a warmth that keeps the aesthetic from feeling cold.
- Never add drop shadows to text on dark backgrounds — the hero headings must feel bold and flat, directly pressed against the void.
- Do not reduce card corner radii below 8px — the rounded rectangle language is a core system pattern that should never collapse to sharp corners.
- Avoid centering large blocks of body paragraph copy — all long-form text is left-aligned; centered alignment is reserved for short eyebrow labels and badge pills only.

## Surfaces

| Level | Name | Value | Purpose |
|-------|------|-------|---------|
| 1 | Warm Paper | `#f8f7f5` | Base page canvas for all light-section content areas — the warm off-white ground that all cards and sections float above. |
| 2 | Ghost White Card | `#ffffff` | Lifted card surface in the work and services grid — pure white panels that pop cleanly off the warm paper ground. |
| 3 | Void Black | `#1a1a1a` | Hero section dark canvas and depth inset surfaces — the dominant dark ground of the above-the-fold experience. |
| 4 | Cinder Dark | `#231f23` | Navigation bar pill and elevated dark surfaces — a slightly warmer near-black that sits above the void hero layer. |

## Dark Variant Overrides

### Colors

| Token | Light | Dark |
|-------|-------|------|
| `--color-accent` | `—` | `#c4ff00` |
| `--color-page-canvas` | `—` | `#1a1a1a` |
| `--color-primary-text` | `—` | `#ffffff` |
| `--color-secondary-text` | `—` | `#f8f7f5bf` |
| `--color-surface-raised` | `—` | `#231f23` |

### Surfaces

| Token | Light | Dark |
|-------|-------|------|
| `--surface-base` | `—` | `#1a1a1a` |
| `--surface-elevated` | `—` | `#231f23` |

## Imagery

Photography is cinematic and high-contrast — professional portraits of CJ in urban architectural settings (waterfronts, city skylines at dusk) shot with a cool, slightly desaturated grading that lets the Electric Lime accent breathe as the warmest element on screen. Work preview cards display brand identity mockups and UI screenshots presented in dark-framed containers with soft gradient fades, creating a gallery-within-a-gallery effect that keeps the focus on the work without visual competition.

## Layout

The page opens with a full-bleed dark hero featuring an asymmetric split: headline and copy occupy the left two-thirds while a cinematic portrait bleeds off the right edge. Below, the light inner sections use a generous three-column card grid at max-width 1140px with 24px gutters and 80px section gaps. The navigation floats as a contained pill-shaped bar centered in the viewport with a dark fill, hovering above the hero with a backdrop blur. Section transitions are clean horizontal cuts — no diagonal clips or overlapping layers — reinforcing the systematic, grid-native aesthetic.

## Agent Prompt Guide

### Quick reference
- Canvas (dark): #1a1a1a (Void Black)
- Canvas (light): #f8f7f5 (Warm Paper)
- Card surface: #ffffff (Ghost White)
- Nav surface: #231f23 (Cinder Dark)
- Primary accent / CTA: #c4ff00 (Electric Lime)
- Primary text (dark bg): #ffffff (Ghost White)
- Body text (dark bg): #f8f7f5bf (Smoke Overlay)
- Body text (light bg): #4d4d4d (Charcoal Ink)
- Secondary text: #808080 (Slate Mist)
- Secondary accent: #00d4ff (Arctic Spark)
- Display font: Helvena (900, uppercase, tight tracking)
- Body font: Kurdis (300–400, relaxed line-height)

### Voice
Direct, self-assured, and conversational without being casual — CJ writes like a strategist who has earned the right to be confident. Headlines are short punchy declarations. Body copy is first-person, slightly informal, and always grounded in a specific point of view. Avoid jargon and hollow buzzwords; every sentence should feel like something a real person with real opinions would say.

### Example prompts
- **Hero section copy:** Write a hero headline and two-sentence subhead for a marketing strategist portfolio. Tone: bold and first-person. Headline should be 4–7 words in all-caps, subhead should introduce the strategist's unique POV on why audience understanding drives brand success.
- **Service card:** Write a 60-word service description for a 'Brand & Positioning' card on a dark-themed portfolio site. Use the Helvena uppercase style for the card title and Kurdis body tone — direct, specific, no hollow adjectives.
- **CTA button label:** Suggest three Electric Lime CTA button labels (2–4 words each, uppercase) for a personal portfolio 'Let's Talk' action — energetic but professional, no exclamation marks.
- **About section paragraph:** Write a 3-sentence about-me paragraph for a marketing and design strategist. First-person, present tense, self-aware without being self-promotional. Should feel like the person notices the typeface on a restaurant menu.

## Quick Start

### CSS Custom Properties

```css
:root {
  /* Colors */
  --color-slate-mist: #808080;
  --color-void-black: #1a1a1a;
  --color-warm-paper: #f8f7f5;
  --color-cinder-dark: #231f23;
  --color-ghost-white: #ffffff;
  --color-arctic-spark: #00d4ff;
  --color-charcoal-ink: #4d4d4d;
  --color-electric-lime: #c4ff00;
  --color-smoke-overlay: #f8f7f5bf;

  /* Typography — Font Families */
  --font-kurdis: 'Kurdis', 'Arial, sans-serif', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-helvena: 'Helvena', 'Arial, sans-serif', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-fragment-mono: 'Fragment Mono', 'monospace', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;

  /* Typography — Scale */
  --text-caption: 11px;
  --leading-caption: 1.2;
  --tracking-caption: 0.08em;
  --text-body-sm: 13px;
  --leading-body-sm: 1.5;
  --tracking-body-sm: 0em;
  --text-body: 14px;
  --leading-body: 1.5;
  --tracking-body: 0em;
  --text-body-lg: 16px;
  --leading-body-lg: 1.6;
  --tracking-body-lg: 0em;
  --text-heading-sm: 20px;
  --leading-heading-sm: 1.2;
  --tracking-heading-sm: 0.02em;
  --text-heading: 32px;
  --leading-heading: 1.1;
  --tracking-heading: 0.01em;
  --text-heading-lg: 48px;
  --leading-heading-lg: 1.05;
  --tracking-heading-lg: 0em;
  --text-display-sm: 64px;
  --leading-display-sm: 1;
  --tracking-display-sm: -0.01em;
  --text-display: 80px;
  --leading-display: 1;
  --tracking-display: -0.02em;

  /* Typography — Weights */
  --font-weight-regular: 400;
  --font-weight-medium: 500;
  --font-weight-bold: 700;

  /* Spacing */
  --spacing-unit: 8px;
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-12: 12px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-48: 48px;
  --spacing-64: 64px;
  --spacing-80: 80px;
  --spacing-96: 96px;
  --spacing-128: 128px;

  /* Layout */
  --page-max-width: 1140px;
  --section-gap: 80px;
  --card-padding: 24px;
  --element-gap: 16px;

  /* Border Radius */
  --radius-pill: 9999px;
  --radius-cards: 16px;
  --radius-large: 32px;
  --radius-small: 8px;
  --radius-medium: 16px;
  --radius-buttons: 8px;
  --radius-nav-pill: 20px;
  --radius-cards-large: 24px;

  /* Surfaces */
  --surface-warm-paper: #f8f7f5;
  --surface-ghost-white: #ffffff;
  --surface-void-black: #1a1a1a;
  --surface-cinder-dark: #231f23;

  /* Shadows */
  --shadow-nav-glow: 0 4px 80px rgba(35,31,35,0.08);
  --shadow-card-float: 0 8px 50px rgba(0,0,0,0.05);
  --shadow-inset-border: inset 0 0 0 1px rgba(244,243,234,0.08);

  /* Motion */
  --duration-micro: 200ms;
  --easing-micro: cubic-bezier(0.2, 0, 0, 1);
  --duration-reveal: 300ms;
  --easing-reveal: cubic-bezier(0.4, 0, 0.2, 1);

  /* Breakpoints */
  --breakpoint-lg: 1440px;
  --breakpoint-md: 991px;
  --breakpoint-sm: 767px;
  --breakpoint-xl: 1920px;
  --breakpoint-xs: 479px;
}

@media (prefers-color-scheme: dark) {
  :root {
    --color-accent: #c4ff00;
    --color-page-canvas: #1a1a1a;
    --color-primary-text: #ffffff;
    --color-secondary-text: #f8f7f5bf;
    --color-surface-raised: #231f23;
    --surface-base: #1a1a1a;
    --surface-elevated: #231f23;
  }
}

[data-theme="dark"] {
  --color-accent: #c4ff00;
  --color-page-canvas: #1a1a1a;
  --color-primary-text: #ffffff;
  --color-secondary-text: #f8f7f5bf;
  --color-surface-raised: #231f23;
  --surface-base: #1a1a1a;
  --surface-elevated: #231f23;
}
```

### Tailwind v4

```css
@theme {
  /* Colors */
  --color-slate-mist: #808080;
  --color-void-black: #1a1a1a;
  --color-warm-paper: #f8f7f5;
  --color-cinder-dark: #231f23;
  --color-ghost-white: #ffffff;
  --color-arctic-spark: #00d4ff;
  --color-charcoal-ink: #4d4d4d;
  --color-electric-lime: #c4ff00;
  --color-smoke-overlay: #f8f7f5bf;

  /* Typography */
  --font-kurdis: 'Kurdis', 'Arial, sans-serif', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-helvena: 'Helvena', 'Arial, sans-serif', ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  --font-fragment-mono: 'Fragment Mono', 'monospace', ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace;

  /* Typography — Scale */
  --text-caption: 11px;
  --leading-caption: 1.2;
  --text-body-sm: 13px;
  --leading-body-sm: 1.5;
  --text-body: 14px;
  --leading-body: 1.5;
  --text-body-lg: 16px;
  --leading-body-lg: 1.6;
  --text-heading-sm: 20px;
  --leading-heading-sm: 1.2;
  --text-heading: 32px;
  --leading-heading: 1.1;
  --text-heading-lg: 48px;
  --leading-heading-lg: 1.05;
  --text-display-sm: 64px;
  --leading-display-sm: 1;
  --text-display: 80px;
  --leading-display: 1;

  /* Spacing */
  --spacing-4: 4px;
  --spacing-8: 8px;
  --spacing-12: 12px;
  --spacing-16: 16px;
  --spacing-24: 24px;
  --spacing-32: 32px;
  --spacing-48: 48px;
  --spacing-64: 64px;
  --spacing-80: 80px;
  --spacing-96: 96px;
  --spacing-128: 128px;

  /* Border Radius */
  --radius-pill: 9999px;
  --radius-cards: 16px;
  --radius-large: 32px;
  --radius-small: 8px;
  --radius-medium: 16px;
  --radius-buttons: 8px;
  --radius-nav-pill: 20px;
  --radius-cards-large: 24px;

  /* Shadows */
  --shadow-nav-glow: 0 4px 80px rgba(35,31,35,0.08);
  --shadow-card-float: 0 8px 50px rgba(0,0,0,0.05);
  --shadow-inset-border: inset 0 0 0 1px rgba(244,243,234,0.08);

  /* Breakpoints */
  --breakpoint-lg: 1440px;
  --breakpoint-md: 991px;
  --breakpoint-sm: 767px;
  --breakpoint-xl: 1920px;
  --breakpoint-xs: 479px;
}
```
