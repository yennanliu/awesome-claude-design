# Tesla — Cinematic (Daylight Minimal)

Reference DESIGN.md for a premium vehicle brand: full-bleed daylight car photography, tiny centered chrome, translucent rounded pill buttons, and near-total colour restraint. The vehicle photography is the design; UI floats over it. A bright, daylight variant of cinematic. Reference: tesla.com.

> Note: tesla.com is behind an Akamai bot wall, so this catalog ships the spec without a captured homepage still. Colours/type reflect the brand's well-known public design.

## 1. Visual Theme & Atmosphere

The product is the page. Tesla's homepage is a stack of full-bleed vehicle shots — clean, bright, aspirational — each with a small centered model name at the top and two pill buttons. There's no marketing chrome to speak of: the car, a name, "Order" / "Demo Drive." Minimalism as confidence.

Mood: clean, premium, aspirational, restrained. Less spec-sheet, more "look at the car."

## 2. Color Palette & Roles

```
/* text/UI colour flips per section to stay legible over the photo */
--ink:             #171a20   /* Tesla near-black — text/buttons on light shots */
--on-light:        #171a20
--on-dark:         #ffffff   /* text over darker shots */
--bg-light:        #ffffff   /* light sections / fallback */
--bg-grey:         #f4f4f4   /* section lift */
--muted:           #5c5e62
--btn-light:       rgba(244,244,244,0.85)  /* translucent light pill (dark text) */
--btn-dark:        rgba(23,26,32,0.70)     /* translucent dark pill (white text) */
--border:          #d0d1d2

/* the brand red — reserved, essentially logo/alert only */
--tesla-red:       #cc0000
```

Rule: the UI is monochrome and *adaptive* — text and pills flip between `--on-light`/`--on-dark` to stay legible over whatever the photo is. There is no decorative accent; Tesla red is logo/alert-only. Colour comes from the vehicle photography.

## 3. Typography Rules

- **UI / chrome / model names:** `Gotham SSm`, `Inter`, system sans. Section headings are the **model name** (e.g. "Model 3"), medium weight, centered, modest size.
- **Sub / tagline:** lighter weight, `--muted`, one short line ("Now supercharged…").
- **Body / legal:** small sentence-case sans.
- **Numerals:** tabular for range, 0–60, top speed, price.
- **Mono:** rarely — VIN, order IDs.

Scale: 12 / 13 / 14 / 16 / 20 / 28 / 40 / 56.

Restrained: hero model names sit ~40–56px and centered — Tesla never shouts with 120px type; the photo is the scale.

## 4. Component Stylings

**Full-bleed vehicle section** (the repeating unit)
- Edge-to-edge daylight car photo; centered top-anchored model name + one-line sub.
- Two pill CTAs below the text (primary + secondary); a downward chevron hint to the next section.
- Text/buttons adopt light or dark variant based on the photo's luminance.

**Buttons** (Tesla's signature pills)
- Primary: translucent light pill `--btn-light`, `--ink` text, UPPERCASE or title-case, fully rounded, ~44px tall, letter-spacing slight ("ORDER NOW").
- Secondary: translucent dark pill `--btn-dark`, white text ("DEMO DRIVE").
- Both sit side-by-side, equal width, generous horizontal padding.

**Nav**
- Transparent over photo, centered model links, small; wordmark "TESLA" letterspaced center or left; account/menu right. Solid white on scroll.

**Spec strip / cards**
- Minimal: big tabular number + tiny uppercase label (Range · 0–60 · Top Speed), separated by hairline `--border`. No heavy card chrome.

**Inputs (order flow)**
- White fill, 1px `--border`, small radius (4–8px). Focus: 2px `--ink` ring. Tabular for price/config numbers.

## 5. Layout Principles

- Vertical stack of full-bleed sections; each = one photo + centered name + two pills. Snap-scroll feel.
- Content centered, generous top margin; everything else is photo.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Softly rounded pills but otherwise near-flat, minimal geometry.
- Desktop-first cinematic; sections remain full-bleed on mobile.

## 6. Depth & Elevation

Photography-led — minimal shadow; pills use translucency + slight blur rather than drop shadow.

- Pill: backdrop-blur + translucent fill; no hard shadow.
- Cards/menus (rare): `0 8px 24px rgba(0,0,0,0.12)`.
- No neumorphism, no glow, no gradients on chrome; the only gradients are photographic.

## 7. Do's and Don'ts

**Do**
- Let full-bleed daylight car photos be the design; keep chrome tiny and centered.
- Flip text/pills between light/dark variants for legibility over each photo.
- Use translucent rounded pill buttons side-by-side (Order / Demo Drive).
- Tabular numerals for range, 0–60, top speed, price.
- Keep the palette monochrome; Tesla red is logo/alert-only.

**Don't**
- Add a decorative brand accent or coloured buttons.
- Oversize the hero type — the photo is the scale (~40–56px names).
- Use heavy drop shadows on pills (translucency + blur instead).
- Crowd sections with specs; one number + label, hairline-separated.
- Left-align the hero name/CTAs — Tesla centers them.

## 8. Responsive Behavior

- Photos crop to keep the vehicle framed; model name scales 56 → 26 on mobile.
- Nav collapses to a menu; pills stack or stay side-by-side depending on width.
- Full-bleed sections persist on mobile; spec strips wrap.
- Order flow is form-first and responsive.

## 9. Motion Notes

- Gentle section transitions and fades (250–400ms); a subtle scroll-snap between full-bleed sections.
- Honour `prefers-reduced-motion` (static photos, no autoplay).
- Motion is calm and premium — never flashy.

## 10. Agent Prompt Guide

Bias: full-bleed daylight vehicle photography as the design, tiny centered chrome, model name as the heading (~40–56px, centered), adaptive monochrome UI that flips light/dark for legibility over each photo, translucent rounded pill buttons side-by-side (primary light / secondary dark), tabular numerals for range/0–60/top-speed/price, near-flat minimal geometry, calm scroll-snap motion. Tesla red is logo/alert-only.

Reject: decorative brand accents or coloured buttons, oversized shouting hero type, heavy drop shadows on pills, spec-crowded sections, left-aligned hero, flashy motion, dark-only assumption (Tesla is daylight-bright).
