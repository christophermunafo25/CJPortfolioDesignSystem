# SocialPaint Design System

> SocialPaint is a brand intelligence layer for marketing and design teams. It sits inside the design platforms a team already works in — Figma, Canva, Adobe — and turns institutional creative knowledge into structured, reusable data. The result: anyone in a company can generate content that looks like the design team made it, because in a sense, they did.

This repo is the **single source of truth** for how SocialPaint looks, sounds, and feels — and a tool for any AI/design agent to produce on-brand artifacts (decks, mocks, prototypes, throwaway pages) without re-deriving the system.

---

## Source materials

Provided by the user and used to derive this system:

| Source | Path | Notes |
|---|---|---|
| Marketing site codebase | `Socialpaint website (1)/` (read-only mount) | React Router + Tailwind + Motion. The product itself is pre-launch — this is the waitlist site. |
| Internal UX guidelines | `Socialpaint website (1)/src/SOCIALPAINT_UI_UX_GUIDELINES.md` | The most authoritative doc the team has. |
| Business overview | `Socialpaint website (1)/src/SOCIALPAINT_BUSINESS_OVERVIEW.md` | Company background + product features + ICP. |
| Brand brief (uploaded) | The "SocialPaint — Brand Brief" pasted in chat | Voice, palette, type, shape, shadow, halo. |
| Fonts (uploaded) | `uploads/StackSans*.{otf,ttf,woff2}` | Stack Sans (Pangram Pangram). See [Type substitution note](#type-substitution-note). |
| Logos (uploaded) | `uploads/Group 25 (3).png`, `Group 50 (2).png`, `Group 28.png` | Wordmark, mark, dark-mode wordmark. |

---

## The product, in one breath

Most tools ask teams to document their brand in templates and style guides that go stale the moment they're written. SocialPaint **learns from the work itself, and keeps learning.** Five surfaces:

1. **StyleDNA** — the brand intelligence engine. Connects to design tools and extracts colors, type, spacing, voice, imagery, components. A living profile that updates as the team designs.
2. **Generate Designs** — natural-language prompt → on-brand visual + copy, sized for every platform.
3. **Connectors** — hooks into design tools and social accounts. The feeds StyleDNA learns from, and the destinations Generate Designs pushes to.
4. **Brand Templates** — repeatable, on-brand starting points the team can lean on.
5. **Insights & Analytics** — what's being generated, by whom, for which platforms, and which sources feed StyleDNA.

The pitch is **"correct by construction"**: the model has actually learned how the team thinks, so its outputs don't need to be policed.

---

## Content fundamentals

### Voice

> *A senior engineer who finally has time to explain things properly.*
>
> Calm. Exact. Quietly witty. Documentation-clean, never marketing-loud.

### Principles

- **Confident, not aggressive.** Statements, not exclamations. Periods, not bangs.
- **Concise.** Short sentences. No filler words. If a sentence can be cut, cut it.
- **Specific.** "60% of production hours" not "lots of time." "Tuesday 9AM posts see 3.2× more engagement" not "great results."
- **Active voice.** "SocialPaint learns your brand" — not "your brand is learned."
- **Second person.** *Your* brand, *your* team. Speak directly to the reader.
- **Plain language.** "Brand consistency checks." Never "multi-dimensional brand alignment protocols."

### Casing

- **Sentence case** for headings, buttons, nav links, and section titles. *"Join the waitlist"*, not *"Join The Waitlist"*.
- **Uppercase + tracked** only for the Fragment Mono labels (eyebrows, taxonomy chips, table headers, metadata).
- The brand name is `SocialPaint` (one word, two capitals). The codebase sometimes uses `Socialpaint`; match whichever the user uses in a given artifact. Prefer `SocialPaint`.

### Punctuation & details

- Em-dashes for asides and rhythm: *"SocialPaint observes how on-brand content actually gets made — every action, decision, and creative pattern."*
- Real curly quotes (`"…"`, `'`), not straight.
- No exclamation marks in product copy. Reserved for the rare moment of warmth in onboarding.
- Numerals over spelled-out numbers from 10 onward; `10×`, not `10x`.
- Oxford comma. Yes.

### Emoji & glyphs

**Emoji are not used.** Anywhere. Not in headers, not in social copy, not in onboarding, not even ironically. The brand earns its warmth through type, color, and shape — not graphical glyphs grafted onto sentences.

Unicode symbols are used sparingly and only when they read as typography: `×` for multiplication, `→` (preferred via the lucide `ArrowRight` icon, not the character), `&` inside Fragment Mono labels.

### Examples (from the wild)

| ✅ Use | ❌ Avoid |
|---|---|
| "Replicate your marketing team straight from the source." | "🚀 Supercharge your team with AI!" |
| "Your brand, down to the pixel." | "Brand Consistency, Reinvented." |
| "Tell me what it's for." | "Tell us your goals and we'll handle the rest 😊" |
| "Tuesday 9AM posts see 3.2× more engagement than average." | "Performance has been great recently." |
| "Join the waitlist" | "Sign Up Now!" |

### Headlines

Headings are set in **Stack Sans Headline, weight 400** — never bold. On **marketing surfaces only** (never product/platform UI), a few words may be set in **Instrument Serif italic** (the `.accent-italic` utility) for emphasis, e.g. "Replicate your team *straight from the source.*" Because Instrument Serif has a smaller x-height, accent words are sized **~1.15× the sans** (`--accent-scale`) so they optically match — e.g. Stack Sans Headline 100px pairs with Instrument Serif italic 115px. Use the accent sparingly: one phrase per headline, and never a second sans family inside a heading.

> Tell me what it's for.
>
> Your brand, generated at scale.
>
> Correct by construction.

---

## Visual foundations

### The mood

A warm, paper-cream document. Generous whitespace. A single bloom of coral-orange light behind the headline. Crisp dark text. Pastel pills earning their tiny corners of color. It should feel like reading a beautifully-typeset spec sheet at a quiet desk.

### Color

The palette has **four surfaces, two inks, five pastels, two semantics**. Pastels are *never* used as large flat fields — only as small icon tiles, category chips, and inside the signature halo gradient. The halo and warm emphasis come from the warm spectrum (`--solar`, `--amber`, `--blush`), not from a pastel.ent.

| Token | Hex | Role |
|---|---|---|
| Linen Base | `#faf8f5` | Outer page wash |
| Paper Cream | `#f7f6f5` | Primary canvas |
| Light Gray | `#ececec` | Secondary surfaces, dividers, resting cards |
| Lift White | `#ffffff` | Elevated cards, inputs |
| Midnight Ink | `#231f23` | Text, primary CTAs, dark surfaces in light mode |
| Obsidian Depth | `#1a171a` | Full dark sections |
| Orchid | `#CDBCFF` | StyleDNA (purple pastel) |
| Mint | `#A7FFAC` | Generate Designs (green pastel) |
| Sky | `#A6CEFF` | Connectors (blue pastel) |
| Sand | `#FFED8C` | Insights & Analytics (warm yellow pastel) |
| Peach | `#FFC5B0` | Brand Templates (peach pastel) |
| Success | `#4a7c59` | Positive trend |
| Danger | `#e94560` | Negative trend |

**Opacity scale on light**: 0.64 (secondary), 0.48 (tertiary/labels), 0.32 (placeholder), 0.08 (borders, disabled). On dark, the same opacities but on `#f7f6f5`. These five steps cover essentially every state.

### Typography

- **Display**: Stack Sans Headline, weight **400** (not bold), tracking `-0.5` to `-2px` based on size.
- **Body**: Stack Sans, weight **300**, 16px / 1.5.
- **Labels / metadata**: Fragment Mono, 10–12px, **uppercase**, tracking `0.75px`.

> #### Type substitution note
> The brief originally specified **Instrument Sans** for display and body. The fonts the user uploaded are **Stack Sans** (Pangram Pangram) — a similar geometric humanist sans that the team appears to have settled on. The system is built on Stack Sans, with Instrument Sans listed as the named fallback. If the user wants to revert to Instrument Sans, swap the family in `colors_and_type.css` — no other change needed.

### Shape

| Element | Radius |
|---|---|
| Cards, sections, hero containers | `20px` |
| Smaller cards (testimonial cells, data cards) | `16px` |
| Icon tiles | `10–12px` |
| Buttons, inputs, tags | `8px` |
| Pills, badges | `999px` |
| Tiny color dots inside labels | `2px` (almost square) |

Never mix radius scales on a single component. A 20px card never contains a 12px button; it contains an 8px button.

### Shadow

There are exactly **two real shadows**, both warm and very wide:

- **Card** — `0 4px 80px rgba(35,31,35,0.08)` — floating panels, nav (scrolled), the hero analyzer frame.
- **Dropdown** — `0 4px 40px rgba(35,31,35,0.08)` — menus and popovers.

Resting cards have **no** shadow. They're flat on the canvas. Shadow appears when an element lifts — scroll-pinning the nav, opening a dropdown, hovering an interactive tile.

### Borders

Almost always `1px solid rgba(35,31,35,0.08)`. On dark sections, `1px solid rgba(247,246,245,0.08)`. Borders are *hairlines* — barely visible, doing structural rather than decorative work.

### Layout

- **Max content width**: `1440px` for full pages, `1100px` for the editorial hero column, `800px` for prose, `520px` for forms.
- **Section padding (vertical)**: a 4-step scale — `80 / 120 / 160 / 200px`. Use the larger steps as you go up the page (hero gets `200`, mid-page sections `120`).
- **Section padding (horizontal)**: `32px` desktop, `16px` mobile.
- **Card grid gap**: `16px`. **Section header → body**: `48–64px`.
- **Generous breathing room.** Cramped layouts break the brand. If something feels tight, give it more space — that's almost always the answer.

### Backgrounds & imagery

- **The signature halo** — a 600–700px blurred radial gradient (`Coral → Sand → Peach`, fading to transparent), sitting behind hero headlines. This is the brand's signature visual move. Don't overuse — usually one per page, just behind the H1.
- **No full-bleed photography** as section backgrounds. Imagery lives *inside* cards with `20px` radius, never as a wash behind text.
- **Dark sections** use a faint SVG noise overlay (`feTurbulence`, very low opacity) for tactile grain — never gradients, never neon.
- **No stock illustrations.** No hand-drawn glyphs. No bluish-purple gradients. No "AI" sparkle effects.

### Motion

- **Library**: Motion (`motion/react`) on the production site. Use the same easing curve for hand-rolled CSS: `cubic-bezier(0.25, 0.1, 0.25, 1)`.
- **Entrance**: `opacity 0→1`, `y 40px→0`, `duration: 0.6s`, triggered once on scroll-in with an `-80px` margin.
- **Stagger**: `0.08s` between siblings.
- **Hover lift**: `y -4px` + shadow appears. `duration: 0.25s`.
- **Dropdown**: height + opacity, `0.3s`.
- **Smooth scroll**: Lenis on the marketing site, `duration: 1.2`, exponential ease-out.
- **No bounces. No springs. No spin.** The brand doesn't celebrate — it informs.

### Hover & press

- **Links**: `opacity: 1` → `0.7`. That's it.
- **Nav links** (inactive state): rest at `opacity: 0.48`, hover at `1`. Active also at `1`.
- **Buttons (primary, dark)**: background darkens negligibly — really just a `0.2s` color transition. No scale.
- **Cards**: rest flat. Hover gains a `0 4px 40px rgba(0,0,0,0.06)` shadow and lifts `4px`. Used only for interactive cards (links, clickable feature tiles), never decorative ones.
- **Press**: no shrink animation. The brand reads as paper, not a button game.

### Transparency & blur

Used sparingly. Two production patterns:
- **Backdrop-blur ghost buttons**: `backdrop-blur(8px)` over `rgba(35,31,35,0.08)`. Lets the canvas show through.
- **Marquee fade edges**: a 80px gradient from `#f7f6f5` to transparent, masking the infinite scroller.

That's it. No frosted glass panels, no overlapping translucent layers.

### Imagery color vibe

Warm. Cream-and-paper backgrounds. When photos appear (product UI shots, case studies), they're shot or composited so they sit naturally on the cream — never cold, never high-contrast blue. Coral, peach, sand pop against the cream and read as *the same world*. Black-and-white is fine for portraits but rare.

### Cards (at a glance)

```
.card {
  background: #ffffff;            /* or var(--paper-warm) for resting */
  border-radius: 20px;
  border: 1px solid rgba(35,31,35,0.08);
  padding: 24px;                  /* sm */  →  32px (md)  →  48px (lg)
  box-shadow: none;               /* shadow appears on hover OR for hero panels */
  transition: transform .25s var(--ease-brand), box-shadow .25s var(--ease-brand);
}
```

---

## Iconography

### Library

**Lucide React** (`lucide-react`). Used everywhere in the codebase. Default stroke weight `1.5`, no fill.

### Sizing & color

| Context | Size | Stroke |
|---|---|---|
| Inline with text / nav buttons | `14–16px` | 1.5 |
| Icon tile badges (cards, nav dropdowns) | `18–20px` (icon) inside `40px` tile (`p-3 rounded-[12px]`) | 1.5 |
| Feature icons (hero feature cards) | `24px` inside icon tile | 1.5 |
| Decorative / hero | `32px` | 1 |

Default icon color: `#231f23` on light surfaces, `#f7f6f5` on dark. Secondary: `rgba(35,31,35,0.48)`.

### The icon tile pattern

Every feature icon in the system sits inside a **pastel rounded square**. The pastel matches the feature:

```
<div class="icon-tile" style="background: var(--orchid)">  /* StyleDNA */
  <Fingerprint size=20 color="#231f23" />
</div>
```

This is the most repeated decorative element in the entire system. The pastel-tile-with-lucide-icon is, in some ways, the brand's iconography.

### Feature-to-icon-to-color mapping

| Feature | Lucide icon | Pastel |
|---|---|---|
| StyleDNA | `Fingerprint` | Orchid `#CDBCFF` |
| Generate Designs | `Wand2` | Mint `#A7FFAC` |
| Connectors | `Workflow` | Sky `#A6CEFF` |
| Insights & Analytics | `BarChart3` | Sand `#FFED8C` |
| Brand Templates | `LayoutTemplate` | Peach `#FFC5B0` |

### No emoji. No custom illustrations.

The brand does not draw. No mascots, no custom SVG illustrations of "AI brains" or "design systems flowing." Imagery is either:
1. A pastel tile + lucide icon, or
2. A real product UI screenshot inside a `20px`-radius card, or
3. The signature warm halo behind a headline.

If a slot calls for an illustration, leave it as a placeholder and ask for real art rather than inventing.

### Logo files (in `assets/`)

Socialpaint ships in two lockup families — a **horizontal** lockup (icon + “SocialPaint” wordmark, side by side) and a **stacked** lockup (icon above the wordmark) — each in three background variants. Pick the variant that matches the background — never recolor, redraw, or substitute. Files are transparent PNGs.

| File | Use |
|---|---|
| `socialpaint-dark.png` | **Primary (horizontal).** Midnight Ink wordmark + flame-gradient icon — for light neutrals (Paper Cream, Linen, Lift White, Ash). |
| `socialpaint-light-color.png` | Horizontal — white wordmark + flame-gradient icon — for clean solid dark surfaces (Obsidian, Graphite, Midnight Ink). Avoid on photography or busy dark imagery; reach for the all-white variant instead. |
| `socialpaint-light.png` | **Safety variant (horizontal).** Fully monochrome white — for color/gradient fills, mesh halos, photography, or anything that isn't a clean light or clean dark surface. When in doubt, this one. |
| `socialpaint-stacked-dark.png` | Stacked — icon above dark wordmark — for light neutrals where vertical space is available. |
| `socialpaint-stacked-light-color.png` | Stacked — icon above white wordmark — for clean solid dark surfaces. |
| `socialpaint-stacked-light.png` | Stacked — all-white safety variant — for color/gradient/photo. |
| `socialpaint-mark-color.png` | Mark alone, flame gradient — for favicons, avatars, social handles, anywhere a wordmark won't fit. |
| `socialpaint-mark-white.png` | Mark alone, monochrome white — pair with `light` lockup contexts. |

**Decision rule (apply in order):**

1. Light neutral background (cream / white / pale gray)? → `socialpaint-dark.png`
2. Clean solid dark (near-black, deep ink, charcoal)? → `socialpaint-light-color.png`
3. Anything else — color, gradient, photo, busy texture? → `socialpaint-light.png`

Borderline (mid-tone teal, saturated pastel, photo with a light patch)? Default to `socialpaint-light.png` — monochrome white reads cleanly almost anywhere; the gradient does not.

**Clear space:** maintain padding around the lockup equal to the icon height, scaled proportionally. **Minimum width:** 120px on screen / 1 inch in print. **Lockup integrity:** the icon and wordmark are one unit — never separate them, resize them independently, or re-space them (use `socialpaint-mark-*.png` if you need the icon alone).

**Never** recolor the gradient, apply the dark wordmark to a colored background, add drop shadows / outlines / glows / strokes, tilt / skew / stretch / crop, or place the logo over a face or product hero. Nav uses the lockup at ~26px tall; footer at ~42px.

---

## Index — what's in this repo

| Path | What it is |
|---|---|
| `README.md` | You are here. The narrative + content fundamentals + visual foundations + iconography. |
| `colors_and_type.css` | The CSS source-of-truth — tokens, font-faces, semantic element defaults. Drop in `<link>`. |
| `SKILL.md` | Agent-readable skill manifest for Claude / Claude Code. |
| `fonts/` | Stack Sans Headline + Stack Sans Text (variable + weighted woff2). |
| `assets/` | Logo PNGs — horizontal lockups (`dark`, `light-color`, `light`), stacked lockups (`stacked-dark`, `stacked-light-color`, `stacked-light`), plus standalone marks (`mark-color`, `mark-white`). |
| `preview/` | Small HTML cards used to populate the Design System tab — colors, type, components, etc. |
| `ui_kits/marketing-site/` | High-fidelity recreation of the SocialPaint marketing site: nav, hero, sticky scroll, products, dark CTA, footer, plus an interactive `index.html`. |

---

## Product surface — what was added in 2026-05

The original brief covered the marketing site. The system was extended to cover the **platform** with the following preview cards (all in `preview/`, grouped by section in the Design System tab):

### Foundations

| Card | Tokens it documents |
|---|---|
| `foundations-icons.html` | Icon library — 40 Lucide line icons, 24px grid, 1.75 stroke. |
| `foundations-motion.html` | `--ease-brand` / `entrance` / `exit` / `emphasized` / `spring` × `--dur-instant` / `fast` / `base` / `slow` / `deliberate`. |
| `foundations-elevation.html` | `--shadow-e1..e5` paired with `--z-base..tooltip`. Use them in lockstep. |
| `foundations-focus.html` | `--focus-ring`, `--focus-ring-dark`. 44px hit targets, 4.5:1 contrast baseline. |
| `foundations-density.html` | `--row-h-compact / cozy / comfy` for tables and lists. |

### Forms

| Card | What it covers |
|---|---|
| `form-text-inputs.html` | Text, search, textarea — all states (rest / hover / focus / filled / error / success / disabled / read-only). |
| `form-select.html` | Single select, multi-select with chips, combobox, grouped. |
| `form-pickers.html` | Date-range calendar, file upload + drag-drop, slider, range slider. |
| `form-toggles.html` | Checkbox (+ indeterminate), radio, switch, segmented. |
| `form-layouts.html` | Two-column form pattern, inline edit, field-level error, footer actions. |

### Overlays

| Card | Pattern |
|---|---|
| `overlay-modal.html` | Destructive confirm with scrim. |
| `overlay-drawer.html` | Right-anchored inspector / sheet drawer. |
| `overlay-toast.html` | Toast (transient, dark) + banner (persistent, tinted). |
| `overlay-tooltip-popover.html` | Tooltip (small, fast) vs popover (rich, clickable). |
| `overlay-menu.html` | Dropdown, grouped, context menu with keyboard shortcuts. |
| `overlay-command-palette.html` | ⌘K — global search + verb-first actions. |

### Data display

| Card | Pattern |
|---|---|
| `data-table.html` | Sortable, selectable, sticky header, pagination. |
| `data-list.html` | Single-line, two-line, with thumbnail or avatar. |
| `data-empty.html` | First-time, filtered-to-zero, success, error, locked, pending. |
| `data-loading.html` | Skeleton shimmer (preferred), spinners, linear + indeterminate + circular progress. |
| `data-tabs.html` | Underline tabs, pill tabs, breadcrumbs, multi-step stepper. |
| `data-avatars-chips.html` | Avatars (5 sizes + status), stack, chips, status badges. |

### AI-native patterns (SocialPaint-specific)

| Card | Pattern |
|---|---|
| `ai-prompt-input.html` | Prompt input with grounding chips, attachments, slash menu, model picker. |
| `ai-streaming.html` | Stage pipeline, token-by-token stream, image shimmer placeholder, "thinking" state. |
| `ai-review.html` | 4-variant pick → accept · model reasoning · keyboard 1–4 to compare. |
| `ai-brand-picker.html` | The design system surfaced as a product feature — lock colors, type, logo, voice for one generation. |
| `ai-run-history.html` | Version timeline, side-by-side diff (content + metadata), restore & branch. |

### App shell & page templates

| Card | What it shows |
|---|---|
| `app-shell.html` | The full assembled product surface — sidebar, topbar, dashboard. |
| `app-page-templates.html` | The 4 layouts every screen falls under: list, detail, settings, editor. |

### Voice & imagery

| Card | What it covers |
|---|---|
| `voice-microcopy.html` | Buttons, errors, confirmations, formatting (dates / numbers / currency / plurals) with do / don't pairs. |
| `imagery-direction.html` | Photography moodboard, do / don't for sourcing & commissioning. |
| `imagery-avatars.html` | Initial-avatar gradients, project tile palettes, image-slot placeholders. |

### Logo system

The logo system uses transparent-PNG lockups in two families — horizontal (`socialpaint-dark.png`, `socialpaint-light-color.png`, `socialpaint-light.png`) and stacked (`socialpaint-stacked-dark.png`, `socialpaint-stacked-light-color.png`, `socialpaint-stacked-light.png`) — plus standalone marks (`socialpaint-mark-color.png`, `socialpaint-mark-white.png`). See the **Logo files** section above for the decision rule and clear-space requirements.

The marketing-site sections (`Nav`, `Hero`, `StickyTrio`, `ProductGrid`, `Metrics`, `DarkCTA`, `Footer`) are exported design-system components on `window.SocialPaintDesignSystem_019df3`.

---

## Caveats

- The brief specified **Instrument Sans**; the uploaded fonts were **Stack Sans**. The system uses Stack Sans with Instrument Sans listed as a fallback. Flag to confirm.
- The provided codebase contains a legacy `theme.css` with a *different* palette (navy/blue/orange/lime) — this is older draft work and is **not** used by the actual site. The `SOCIALPAINT_UI_UX_GUIDELINES.md` doc and the rendered site components are the real source of truth and they match the brief.
- No mobile-app screenshots were provided, so the responsive product patterns are extrapolated from the marketing site's responsive behaviour. Real device captures from beta users would refine this.
