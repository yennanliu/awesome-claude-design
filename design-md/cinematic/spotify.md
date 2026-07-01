# Spotify — Cinematic (Vibrant Dark)

Reference DESIGN.md for a bold consumer-music brand: black canvas, Spotify green, a promo-pink CTA, oversized Circular type, and a mosaic of vibrant album art as the hero. A vibrant-dark cinematic variant — media-heavy and energetic. Reference captured on the Traditional-Chinese Premium page.

## 1. Visual Theme & Atmosphere

Sound, loud and visual. Spotify sells feeling, so the page is black to let saturated album art pop, type is big and confident, and a single green carries the brand while campaign pink pushes the offer. It's cinematic in its media density and scale, but energetic and pop rather than moody.

Mood: bold, vivid, youthful, музыка-forward. Less corporate, more "turn it up."

## 2. Color Palette & Roles

```
--bg:              #000000   /* canvas — lets album art glow */
--bg-alt:          #121212   /* section lift / cards */
--surface:         #1a1a1a   /* raised card, input */
--surface-2:       #242424
--text:            #ffffff
--text-muted:      #b3b3b3   /* Spotify's canonical secondary grey */
--text-dim:        #7a7a7a
--border:          #2a2a2a

--accent:          #1ed760   /* Spotify green — brand, primary action, active */
--accent-hover:    #1fdf64
--accent-deep:     #169c46

--promo:           #ffc9d4   /* campaign pink — offer/trial CTA */
--promo-text:      #111111   /* dark text on pink/green pills */

/* gradient wash behind hero (subtle, brand-tinted) */
--wash-a:          #3d2b4f
--wash-b:          #000000
```

Rule: green is the permanent brand + primary action; promo pink is campaign-scoped (trials/offers) and temporary. Album art supplies all the other colour — never invent decorative hues; let the artwork be the palette.

## 3. Typography Rules

- **Display / hero:** `Spotify Circular` (fallback `Montserrat`, `Inter`), weight 700–900, tight tracking, **big**. Bold black-weight headlines are the signature.
- **Body / UI:** Circular / `Inter`, weight 400/500, `--text-muted` for secondary copy.
- **CJK:** `Noto Sans TC`, `Noto Sans SC`, `Noto Sans JP` — Spotify is global; this reference is zh-TW. Match CJK weight to the bold Latin display.
- **Numerals:** tabular for prices, durations, plan tiers.
- **Mono:** rarely — only for codes/receipts.

Scale: 12 / 14 / 16 / 18 / 24 / 32 / 44 / 60 / 80.

44–80px black-weight display for the hero; 14–16px body. Prices sit inline in bold display.

## 4. Component Stylings

**Album-art mosaic hero** (the centrepiece)
- A tilted/overlapping grid of saturated cover art bleeding off the right edge.
- Left: black-weight headline (with the price inline, e.g. "只要 $0") + muted subline + CTAs.
- Subtle brand-tinted gradient wash (`--wash-a → --wash-b`) behind the type for legibility.

**Buttons**
- Primary (offer): `--promo` pink fill, `--promo-text` dark text, fully rounded pill, weight 700, slight scale(1.04) on hover — Spotify's signature grow.
- Primary (evergreen): `--accent` green fill, dark text, pill.
- Secondary: transparent, white text, 1px `--text-muted` outline, pill.

**Plan / pricing cards**
- `--bg-alt` fill, radius 8px, generous padding. Plan name (bold) + big tabular price + feature list with green checks.
- Highlighted plan: 1px `--accent` border or a subtle gradient top-edge.

**Now-playing / list rows (app)**
- 56px rows, cover thumb + title/artist, green active state, `--text-muted` metadata, tabular durations right-aligned.

**Nav**
- Black bar, Spotify logo left, sparse links, a divider, then `註冊 / 登入`. Green or pink pill CTA right.

**Badges / tags**
- Pill, 20px, uppercase or title-case. Plan tier, "Premium", campaign labels; green or pink fills.

**Inputs**
- `--surface` fill, no border at rest, radius 8px (large tap targets). Focus: 2px `--accent` ring.

## 5. Layout Principles

- 1200px max content shell, 24px gutter; hero art mosaic breaks full-bleed to the right edge.
- Generous vertical rhythm; sections alternate black and near-black with occasional gradient washes.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Mobile-first for the app; marketing is responsive desktop-down with tap-target sizing.

## 6. Depth & Elevation

Black canvas — depth from album-art layering, gradient washes, and subtle steps (`--bg` → `--bg-alt` → `--surface`), not hard shadow.

- Card: `0 4px 16px rgba(0,0,0,0.5)`
- Hover lift + scale on primary pills (Spotify's tactile grow, ~120ms).

No neumorphism. Gradients are brand-tinted and subtle; album art provides the visual energy.

## 7. Do's and Don'ts

**Do**
- Keep black canvas so album art glows; let artwork be the palette.
- Green = brand/evergreen action; pink = campaign/offer only.
- Big black-weight Circular display, with price set inline.
- Fully rounded pills with a subtle grow-on-hover.
- Tabular numerals for prices, durations, tiers; match CJK weight to Latin.

**Don't**
- Invent decorative colours beyond green/pink + album art.
- Use light canvas or thin display weights.
- Make promo pink permanent (it's campaign-scoped).
- Square off the pills or drop the hover grow.
- Let white text sit on busy album art without a wash/scrim.

## 8. Responsive Behavior

- Hero art mosaic reflows/crops; headline scales 80 → 32 on mobile, price stays inline.
- Nav collapses to a menu; the green/pink CTA persists.
- Pricing cards stack single-column; feature lists remain scannable.
- App surfaces are mobile-first with bottom nav and 56px rows.

## 9. Motion Notes

- Primary pills grow slightly on hover/press (Spotify's tactile feedback), ~120ms.
- Album mosaic may drift/parallax subtly; honour `prefers-reduced-motion`.
- Keep motion playful but brief — energy, not distraction.

## 10. Agent Prompt Guide

Bias: black canvas (#000), Spotify green brand/action (#1ed760), campaign pink for offers only (#ffc9d4 on dark text), oversized black-weight Circular display (with price inline) + Noto Sans CJK, album-art mosaic as the hero and the palette source, fully rounded pills with subtle grow-on-hover, tabular numerals for prices/durations, subtle brand-tinted gradient washes.

Reject: light canvas, thin display weights, invented decorative colours beyond green/pink + artwork, permanent promo pink, squared pills, unscrimmed white text over busy art, non-tabular prices.
