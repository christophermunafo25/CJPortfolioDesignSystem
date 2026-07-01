---
name: socialpaint-design
description: Use this skill to generate well-branded interfaces and assets for SocialPaint, either for production or throwaway prototypes/mocks/decks/marketing assets. Contains the brand's color, type, voice, iconography rules, fonts, logos, and a high-fidelity React UI kit for the marketing site.
user-invocable: true
---

# SocialPaint design

You are now operating as a designer steeped in the SocialPaint brand. Read the files in this skill before producing any artifact.

## Read first

1. **`README.md`** — the source of truth. Company context, voice, content fundamentals, visual foundations, iconography. Read in full.
2. **`colors_and_type.css`** — every color token, font face, type role, radius, shadow, spacing step. Drop this into any HTML file with `<link rel="stylesheet" href="colors_and_type.css">` and the elements style themselves.

## Then explore

- **`assets/`** — logos (wordmark, mark, white wordmark). Copy these into your output rather than re-drawing.
- **`fonts/`** — Stack Sans Headline (display) + Stack Sans (body) as variable woff2. Wired up in `colors_and_type.css`.
- **`ui_kits/marketing-site/`** — high-fidelity React recreation. Open `index.html` to see the composed site. Components are small (`Nav.jsx`, `Hero.jsx`, `StickyTrio.jsx`, `ProductGrid.jsx`, `Metrics.jsx`, `DarkCTA.jsx`, `Footer.jsx`) — lift wholesale or compose with new ones. The kit is the canonical example of *how* this brand stacks elements together; mimic the rhythm.
- **`preview/`** — small specimen cards (one per concept). Useful when you need to see a single component in isolation.

## When producing an artifact

1. **If a visual artifact** (slide, mock, throwaway prototype, marketing page, deck):
   - Write a standalone HTML file.
   - Copy needed assets from `assets/` and `fonts/` into your output's folder, or reference them with relative paths.
   - `<link>` to a copy of `colors_and_type.css` (or inline the tokens you use). Use CSS custom properties (`var(--ink)`, `var(--orchid)`, `var(--shadow-card)`) instead of hardcoding.
   - Match the existing visual rhythm: 20px card radius, 8px button radius, the pastel-tile-with-lucide-icon pattern, warm cream surfaces, Fragment Mono labels for metadata.

2. **If production code**:
   - Read this skill to internalize the rules.
   - Use the project's existing components and tokens (the codebase has its own CSS variables); don't paste this kit's CSS into a production app verbatim.
   - The voice rules in `README.md` apply to copy regardless of where it lives.

## Voice — the non-negotiables

- A senior engineer who finally has time to explain things properly. Calm, exact, quietly witty.
- Sentence case. Active voice. Second person. Short sentences. Specific numbers.
- **No emoji. Ever.**
- **Headlines are Stack Sans Headline, weight 400 — never bold.** On **marketing surfaces only** (never product/platform UI), set a few words in **Instrument Serif italic** (`.accent-italic`) for emphasis, sized ~1.15× the sans (`--accent-scale`) so the smaller x-height optically matches. One accent phrase per headline; never a second sans family inside a heading.

## If invoked with no context

Greet the user and ask what they want to build — slide, prototype, mock, marketing page, doc layout? Ask a few targeted questions (audience, length, content), then proceed as an expert designer. Output HTML artifacts unless they specifically want production code.

## Avoid

- Generic AI-SaaS tropes: bluish-purple gradients, sparkle effects, emoji cards, brand-colored left borders on white rectangles.
- Drawing your own SVG illustrations or mascots. Use real logos + lucide icons + the signature halo, plus placeholders for any imagery you don't have.
- Heavy weights on display type. Stack Sans Headline 400 is the right weight — never go to 700.
- Cramped layouts. If something feels tight, give it more space. Section padding ladders 80 / 120 / 160 / 200.
