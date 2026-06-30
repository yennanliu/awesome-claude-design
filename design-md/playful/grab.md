# Grab — Playful Superapp

Reference DESIGN.md for a Southeast-Asian consumer superapp: Grab green against bright white, bold rounded display type, full-bleed real-people photography, generous radii, friendly and human. Multi-market by default (SG / MY / ID / TH / VN / PH).

## 1. Visual Theme & Atmosphere

Warm, human, everyday. Grab is the app a whole region opens to get a ride, lunch, groceries, and to pay — so the brand reads optimistic and accessible, never corporate-cold. The playfulness comes not from illustration but from **bold rounded type, one confident green, and full-bleed photography of real drivers, riders, and merchants**. Green helmets and the double-bar mark are the recurring motifs.

Mood: friendly, community-minded, energetic, trustworthy. "Making every day better" — said plainly, over a photo of someone's actual day.

## 2. Color Palette & Roles

```
--bg:              #ffffff   /* canvas */
--bg-alt:          #f7f7f7
--surface:         #f2f2f2   /* gray section lift / cards */
--surface-green:   #e6f7ee   /* soft green wash for callouts */
--text:            #1a1a1a   /* near-ink headlines + body */
--text-muted:      #5c5c5c
--text-dim:        #8a8a8a
--border:          #e5e5e5
--border-strong:   #d4d4d4
--on-dark:         #ffffff   /* text over photos / dark-green bands */

--accent:          #00b14f   /* Grab green — primary action + brand */
--accent-hover:    #009a45
--accent-deep:     #00692e   /* footer band, pressed, dark sections */
--accent-soft:     #e6f7ee   /* tinted callouts, secondary button bg */

--success:         #00b14f   /* shares brand green — positive/confirmed */
--warning:         #ff8c00   /* amber, attention */
--danger:          #e02020   /* red, error / cancel */
```

Rule: Grab green is the only branded hue and the single action color. Status uses distinct amber/red — never introduce a second saturated brand color. The dark-green band `--accent-deep` anchors footers and full-width CTAs; the soft wash `--accent-soft` is the friendly softening move behind callouts.

## 3. Typography Rules

- **Headlines + display:** Grab's rounded brand sans (fallback `Poppins`, `Inter`, `-apple-system`, system-ui). Weight 700–800, tight tracking, **large** — hero headlines run huge over photography.
- **Body + UI:** Same family, weight 400/500, line-height 1.5–1.6.
- **CJK / Thai / Vietnamese:** always include regional fallbacks — `Noto Sans` (Thai, SC), `Noto Sans Vietnamese`; Grab ships across SEA scripts.
- **Numerals:** tabular figures on fares, prices, wallet balances, and order totals.
- **Mono:** `JetBrains Mono`, `SF Mono` — booking IDs, promo codes, OTPs only.

Scale: 12 / 14 / 16 / 18 / 20 / 24 / 32 / 40 / 56 / 72.

Hero display runs 56–72px on desktop over a photo; 14–16px dominates body and service cards.

## 4. Component Stylings

**Buttons**
- Primary: Grab green `--accent` fill, white text, radius 8px (soft rounded rect, not full pill), padding 14/24, weight 600. Hover: `--accent-hover`. Pressed: `--accent-deep` + scale(0.98) ~100ms.
- Secondary: `--surface-green` fill, `--accent-deep` text, radius 8px.
- On photos / dark-green bands: white fill, `--accent-deep` text, OR green fill with white text — keep AA contrast over imagery (add a scrim).
- Destructive: `--danger` fill, white text, confirm modals only.

**Service cards / tiles** (the superapp grid)
- White or `--surface` fill, radius 16px, padding 20. Each service (Rides / Food / Mart / Express / Finance) gets an icon in green + label.
- Soft shadow `0 2px 8px rgba(0,0,0,0.06)` only. Hover: lift to `0 6px 16px rgba(0,0,0,0.10)`.
- Icons: rounded, friendly line-or-filled, single green hue. Avoid photorealism in icons.

**Photography**
- Full-bleed, real people (drivers, riders, merchants, families). Warm, candid, on-location SEA settings.
- Headlines overlay with a left-anchored gradient scrim (`rgba(0,0,0,0.0 → 0.35)`) so white type stays legible.
- Never stretch or heavily filter; keep skin tones true. Photography is the brand's humanity — don't swap it for stock illustration.

**Cards / list items**
- White fill, 1px `--border`, radius 12–16px, padding 20. Generous tap targets (≥56px rows on mobile).

**Inputs**
- `--surface` fill, no border at rest, radius 12px, padding 14/16. Focus: 2px `--accent` ring.
- Currency/amount inputs right-aligned tabular numerals.

**Nav**
- Web top nav: white fill, 1px bottom `--border`, green active state, country switcher (SG/MY/ID/TH/VN/PH).
- Mobile: bottom-tab nav, green active icon.

## 5. Layout Principles

- Marketing: 1200px max shell, 24px gutter, generous vertical rhythm (48–80px between blocks).
- Full-bleed photo heroes break the shell to edge; content stays within the 1200px lane.
- App surfaces: mobile-first, 360–430px primary canvas; ≥56px tap-target rows.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 80.
- Service grid: 2-up on mobile, 3–4-up on desktop, equal-height rounded tiles.

## 6. Depth & Elevation

Bright white canvas — depth via soft shadows and the dark-green band, not borders.

- Cards: `0 2px 8px rgba(0,0,0,0.06)`; hover `0 6px 16px rgba(0,0,0,0.10)`.
- Modals / bottom sheets: `0 12px 32px rgba(0,0,0,0.14)`.
- No neumorphism, no stacked shadows, no gradients on flat surfaces (gradients only as photo scrims). Press feedback: scale(0.98), ~100ms ease-out.

## 7. Do's and Don'ts

**Do**
- Keep Grab green as the single confident brand + action color.
- Lead with full-bleed photography of real people; add a scrim under overlaid type.
- Use bold rounded display type, large, for hero statements.
- Render fares, prices, and balances in tabular numerals.
- Ship the superapp service grid as equal-height rounded tiles.
- Include regional script fallbacks (Thai, Vietnamese, SC) in every type stack.

**Don't**
- Introduce a second saturated brand hue, or reuse status amber/red decoratively.
- Replace photography with flat-vector illustration as the hero (that's the Toss lane, not Grab's).
- Use dark mode as the default marketing canvas.
- Let white type sit on a photo without a scrim (contrast failures).
- Over-round buttons into full pills, or stack heavy shadows.
- Assume one currency/locale — every market differs.

## 8. Responsive Behavior

- Mobile-first for app surfaces; marketing is responsive desktop-down.
- Hero display scales 72 → 32 on mobile; photo crops to keep the human subject in frame.
- Service grid: 3–4-up (desktop) → 2-up (mobile).
- Modals become full-screen bottom sheets below 640px.
- Country switcher persists across breakpoints.

## 9. Internationalisation & Multi-Market Notes

- Six+ markets (SG / MY / ID / TH / VN / PH) — locale drives language, currency, and content.
- Currency: render per market (S$, RM, Rp, ฿, ₫, ₱) with locale-correct separators; never hardcode SGD.
- Type stack must cover Latin, Thai, and Vietnamese diacritics without clipping line-height.
- Photography should reflect the local market where possible; avoid one-market-fits-all imagery.
- Keep layouts flex-direction reversible in case of future RTL needs.

## 10. Agent Prompt Guide

Bias: bright white `#ffffff` canvas, single Grab green `#00b14f` accent (+ dark-green `#00692e` band and soft `#e6f7ee` wash), bold rounded display sans (Poppins/Inter fallback) with Thai/Vietnamese/SC fallbacks, 8px button radius / 12–16px card radius, full-bleed real-people photography with gradient scrims under white type, superapp service grid of equal-height rounded tiles, tabular numerals on fares/prices, mobile-first ≥56px tap targets, multi-market currency/locale.

Reject: dark-mode marketing default, second saturated brand hue, flat-vector illustration as hero imagery, status colors used decoratively, full-pill or heavy-shadow buttons, unscrimmed white text over photos, hardcoded single currency/locale, non-tabular numerals on money.
