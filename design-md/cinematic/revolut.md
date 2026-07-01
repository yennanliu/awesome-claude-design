# Revolut — Cinematic (Premium Fintech Dark)

Reference DESIGN.md for premium fintech marketing: a near-black stage, a hero rendered around the physical card, bold grotesque type, pill buttons, and Revolut's vibrant gradient used as a scarce jewel. A dark, product-render variant of cinematic. Reference captured on the Business page.

## 1. Visual Theme & Atmosphere

"This is business banking." Revolut sells premium capability, so the page is a dark cinematic stage: dramatic lighting, a metal card floating on geometric podiums, confident bold type, and a single vibrant gradient that flashes on brand moments. Restraint on the Business surface; the gradient is the reward, not the wallpaper.

Mood: premium, sleek, engineered, aspirational. Less playful-consumer, more "the card that means business."

## 2. Color Palette & Roles

```
--bg:              #000000   /* stage canvas */
--bg-alt:          #0a0b0f   /* section lift */
--surface:         #14161c   /* card / panel */
--surface-raised:  #1c1f27
--text:            #ffffff
--text-muted:      #a7adba
--text-dim:        #6b7180
--border:          #23262f
--border-strong:   #333844
--metal:           #c9ccd3   /* metallic card / silver pill */

/* Revolut vibrant gradient — scarce jewel accent */
--grad-a:          #4b6bff   /* electric blue */
--grad-b:          #a248ff   /* violet */
--grad-c:          #ff5ea1   /* pink */
--accent:          #6d7cff   /* solid fallback for links/focus */
--accent-hover:    #8a95ff

/* status (product) */
--pos:             #2ecf80   /* credit / positive */
--neg:             #ff5a5f   /* debit / decline */
```

Rule: the blue→violet→pink gradient is a scarce jewel — use it on one hero element, a key CTA, or a highlighted number, never as a full-section wash on the Business surface. Keep the stage black and let lighting + the metal card carry drama. Status green/red is for transactions only.

## 3. Typography Rules

- **Display / hero:** a bold grotesque (`Aeonik`, `Neue Haas Grotesk`, `Inter`), weight 600–700, tight tracking. Big, confident, sentence-case ("This is business banking").
- **Body / UI:** same grotesque or `Inter`, weight 400/500, `--text-muted` for secondary.
- **Numerals:** tabular everywhere money appears — balances, FX rates, fees, limits.
- **Mono:** `JetBrains Mono`, `SF Mono` — IBANs, card numbers, transaction IDs, API keys.

Scale: 12 / 14 / 16 / 18 / 22 / 28 / 40 / 56 / 72.

56–72px bold display over the dark stage; 14–16px body; tabular figures for all amounts.

## 4. Component Stylings

**Product-render hero** (the centrepiece)
- Near-black stage with soft directional lighting and subtle geometric podiums/planes.
- The physical card (metal, embossed) rendered at an angle, catching a rim of the vibrant gradient.
- Left-anchored bold headline + muted subline + one pill CTA.

**Buttons**
- Primary: `--metal` silver pill (or gradient-filled on a brand moment), dark text, fully rounded, weight 600 ("Open a bank account").
- Secondary: transparent, white text, 1px `--border-strong`, pill.
- Nav "Sign up": metallic/white pill.

**Cards / feature tiles**
- `--surface` fill, 1px `--border`, radius 16px. Product screenshots or metal-card renders inside; minimal chrome.
- A highlighted metric may use a gradient underline or gradient number — sparingly.

**Balance / FX rows (product)**
- 56px rows, currency flag + code (mono) + big tabular amount right-aligned; +/− coloured by `--pos`/`--neg` with sign, never colour alone.

**Nav**
- Transparent-over-stage, solid `--bg` on scroll. Wordmark left, sparse links, metallic "Sign up" pill right.

**Badges / tags**
- Pill, 20px, 12px. Plan tier, "Business", region. Mono for account/IBAN identifiers.

**Inputs**
- `--surface` fill, 1px `--border`, radius 12px. Focus: 2px `--accent` ring.
- Mono for IBAN / card / amount fields; amounts right-aligned tabular.

## 5. Layout Principles

- 1200px max content shell, 24px gutter; hero/product stages break full-bleed.
- Generous vertical rhythm (48–80px); alternate black stage sections with near-black feature bands.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80.
- Mobile-first for the app; marketing responsive desktop-down with pill tap targets.

## 6. Depth & Elevation

Black stage — depth via lighting, product renders, and background steps (`--bg` → `--bg-alt` → `--surface`), not flat shadow.

- Card: `0 8px 28px rgba(0,0,0,0.5)`
- Overlay/menu: `0 16px 48px rgba(0,0,0,0.6)`
- The gradient may cast a soft coloured glow behind the hero card only.

No neumorphism. Gradient is a jewel, not a texture; keep flat surfaces flat.

## 7. Do's and Don'ts

**Do**
- Keep the stage black; let lighting + the metal card render carry drama.
- Use the blue→violet→pink gradient scarcely — one hero moment or CTA.
- Bold grotesque display; tabular numerals for every amount, mono for IBAN/card IDs.
- Fully rounded pill buttons; metallic silver for the primary on the Business surface.
- Sign + colour for +/− amounts, never colour alone.

**Don't**
- Wash whole sections in the gradient (that's the consumer-marketing register, not Business).
- Use light canvas or thin display weights.
- Center-align monetary columns.
- Reuse transaction green/red as decoration.
- Over-round or over-chrome feature cards.

## 8. Responsive Behavior

- Hero render crops to keep the card in frame; display scales 72 → 30 on mobile.
- Nav collapses to a menu; the metallic CTA persists.
- Full-bleed stages stack; feature tiles go single-column.
- Product/app surfaces mobile-first with 56px rows and bottom sheets.

## 9. Motion Notes

- Slow, premium motion (300–500ms ease): the card render may rotate subtly, the gradient rim may drift.
- Honour `prefers-reduced-motion` (static render, no drift).
- Motion signals quality — never bouncy or fast.

## 10. Agent Prompt Guide

Bias: black stage canvas (#000), near-black cinematic product-render hero built around a metal card, bold grotesque display (Aeonik/Inter) at 56–72px, Revolut blue→violet→pink gradient used scarcely as a jewel (on one hero element/CTA), metallic silver pill primary buttons, tabular numerals for all amounts, mono for IBAN/card/transaction IDs, sign+colour for +/−, slow premium motion.

Reject: full-section gradient washes on the Business surface, light canvas, thin display weights, centered monetary columns, transaction colours as decoration, bouncy/fast motion.
