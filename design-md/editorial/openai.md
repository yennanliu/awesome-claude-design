# OpenAI — Editorial Minimalism (Dark)

Reference DESIGN.md for extreme, confident minimalism on a black canvas: monochrome, enormous whitespace, one geometric sans, a rounded conversational input as the hero, and near-zero decoration. A dark variant of editorial minimalism — restraint as the brand. Reference captured on the Traditional-Chinese homepage.

## 1. Visual Theme & Atmosphere

Quiet confidence. OpenAI's homepage says almost nothing on screen — a black field, one centered question, a rounded input, a few pill prompts. The absence of colour, ornament, and density *is* the statement: the product is powerful enough that the page doesn't have to shout.

Mood: calm, spacious, authoritative, neutral. Less "look at our features," more "ask, and it begins."

## 2. Color Palette & Roles

```
--bg:              #000000   /* canvas */
--bg-alt:          #0d0d0d   /* section lift */
--surface:         #1a1a1a   /* input, card */
--surface-2:       #242424   /* raised / hover */
--text:            #ffffff
--text-muted:      #a1a1a1
--text-dim:        #6e6e6e
--border:          #2e2e2e
--border-strong:   #3d3d3d

/* action — monochrome, not a saturated brand hue */
--action:          #ffffff   /* primary button: white fill, black text */
--action-text:     #000000
--focus:           #ffffff   /* focus ring (monochrome) */

/* used ONLY inside imagery tiles, never as UI accent */
--tile-warm:       #f5a623   /* e.g. a sun/space still */
--tile-cool:       #7c8cff
```

Rule: the UI is monochrome by design — no saturated accent on chrome. Colour appears only inside editorial/product imagery tiles, never on buttons, links, or focus states. Restraint is the identity; adding a brand accent breaks it.

## 3. Typography Rules

- **Display / hero:** `OpenAI Sans` (fallback `Söhne`, `Inter`, system-ui), weight 500–600, tight tracking. Centered, medium-large, calm — not oversized-shouting.
- **Body / UI:** same family, weight 400/500, generous line-height 1.6, `--text-muted` for secondary.
- **CJK:** `Noto Sans TC`, `Noto Sans SC`, `Noto Sans JP` — global brand; this reference is zh-TW. Keep CJK weight aligned with the light Latin.
- **Numerals:** tabular where numbers appear (usage, pricing).
- **Mono:** `SF Mono`, `JetBrains Mono` — code samples, API snippets only.

Scale: 13 / 14 / 15 / 16 / 18 / 22 / 28 / 36 / 48.

Note the restraint: the hero heading sits around 28–36px, not 80px. Whitespace does the work display size usually does.

## 4. Component Stylings

**Conversational input** (the hero)
- Wide rounded field, `--surface` fill, 1px `--border`, radius 16px, tall (multi-line), generous inner padding.
- Placeholder in `--text-dim`; a circular send button (white fill, black arrow) bottom-right.
- Centered under a single short heading; nothing else competes.

**Prompt / suggestion pills**
- Fully rounded, transparent fill, 1px `--border`, `--text-muted` label, hover → `--surface`/white text.
- A short row of 4–5 (e.g. 研究 · API 平台 · 品牌故事 · 更多).

**Buttons**
- Primary: `--action` white fill, black text, pill or 8px radius, weight 600 (e.g. "試用 ChatGPT ↗").
- Secondary/ghost: transparent, white text, 1px `--border-strong`.
- Links: white or `--text-muted`, underline on hover — never a coloured link.

**Editorial / product tiles**
- Large image-led cards (research stills, product screenshots, space imagery), radius 12–16px, minimal caption.
- Imagery carries all colour; captions stay monochrome. Generous gaps between tiles.

**Nav**
- Black, wordmark left, sparse text links, search glyph; a white pill CTA + subtle "登入" right. Hairline `--border` on scroll only.

**Inputs (general)**
- `--surface` fill, 1px `--border`, radius 12px. Focus: 2px white ring, 2px offset (monochrome).

## 5. Layout Principles

- Content centered in a narrow column for the hero (max ~760px), widening to 1200px for tile grids.
- Extreme vertical whitespace — the hero occupies a near-empty viewport on purpose.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96 / 128.
- Alternating: centered minimal hero → generous image-tile grids (2-up / asymmetric).
- Responsive, content-first; nothing fights the input.

## 6. Depth & Elevation

Black canvas — depth via near-black steps (`--bg` → `--bg-alt` → `--surface` → `--surface-2`) and 1px borders, essentially no shadow.

- Input/card: at most `0 1px 2px rgba(0,0,0,0.4)` or none.
- Menu/dialog: `0 8px 32px rgba(0,0,0,0.6)`.

No neumorphism, no glow, no gradients on chrome. Flatness + space is the aesthetic.

## 7. Do's and Don'ts

**Do**
- Keep the UI strictly monochrome; let imagery be the only colour.
- Make the rounded conversational input the single hero element.
- Use enormous whitespace; keep the hero heading modest in size.
- White-fill / black-text primary button; monochrome focus ring.
- Align CJK weight to the light Latin geometric sans.

**Don't**
- Introduce a saturated brand accent on buttons, links, or focus.
- Oversize or bold-shout the hero type — restraint is the point.
- Crowd the hero with more than one heading + input + a short pill row.
- Add gradients, glows, or decorative shapes.
- Use coloured links.

## 8. Responsive Behavior

- Hero input stays full-width within the narrow centered column; heading scales 36 → 22 on mobile.
- Pill row wraps or scrolls horizontally; nav collapses to a menu with the white CTA persisting.
- Tile grids collapse 2-up → single column; keep the generous gaps.
- Content-first everywhere; never sacrifice the whitespace that defines the brand.

## 9. Motion Notes

- Minimal, quiet motion: gentle fades and 200–300ms eases; the send button may have a subtle press state.
- No parallax circus; honour `prefers-reduced-motion`.
- Let stillness read as confidence — motion is punctuation, not decoration.

## 10. Agent Prompt Guide

Bias: pure black canvas (#000), strictly monochrome UI (white text, white-fill/black-text buttons, white focus ring), one geometric sans (OpenAI Sans → Söhne/Inter) + Noto Sans CJK, a wide rounded conversational input as the single hero, short row of outlined pill prompts, enormous whitespace, modest hero heading size (28–36px), colour only inside imagery tiles, flat borders-not-shadows depth, quiet motion.

Reject: saturated brand accent on chrome/links/focus, oversized shouting hero type, crowded hero, gradients/glows/decorative shapes, coloured links, cramped spacing, busy motion.
