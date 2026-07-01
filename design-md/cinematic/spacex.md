# SpaceX — Cinematic Dark

Reference DESIGN.md for aerospace at its most austere: pure black, full-bleed rocket & orbital footage, tiny letterspaced uppercase chrome, and almost no colour. The imagery is the entire design; type gets out of the way. Reference: spacex.com.

> Note: spacex.com is behind an Akamai bot wall, so this catalog ships the spec without a captured homepage still. Colours/type are from the brand's well-known public design.

## 1. Visual Theme & Atmosphere

The mission is the message. SpaceX pages are full-bleed film of vehicles and launches on pure black, with minimal white letterspaced-uppercase labels floating over them. Restraint is total — no accent colours, no decoration, no gradients beyond the footage's own light. The result reads as documentary and monumental.

Mood: austere, monumental, engineered, quiet. Less "marketing," more "flight footage with captions."

## 2. Color Palette & Roles

```
--bg:              #000000   /* pure black canvas */
--surface:         #0c0c0e   /* rare card / panel */
--surface-raised:  #16161a
--text:            #ffffff
--text-muted:      #b7b9bd
--text-dim:        #6f7176
--border:          #ffffff26 /* hairline white @ ~15% */
--border-strong:   #ffffff4d /* white @ ~30% */
--on-film:         #ffffff

/* the only near-accent: mission live/alert red, used almost never */
--alert:           #e33   /* abort / critical only */
```

Rule: the palette is monochrome by mandate. There is no brand accent — white on black over film. The single red is reserved for genuine alert/abort states and appears essentially never on marketing. Colour comes exclusively from the footage.

## 3. Typography Rules

- **Chrome / labels / nav:** letterspaced UPPERCASE, `D-DIN`, `Gotham`, `Inter` (tight, wide tracking `.12–.2em`), small (11–13px). This is the SpaceX signature.
- **Display / hero:** same family, uppercase, weight 500–700, large but restrained; often just a mission or vehicle name.
- **Body / captions:** sentence-case sans, `Inter`, weight 400, `--text-muted`.
- **Numerals:** tabular for countdowns, altitude, velocity, payload mass.
- **Mono:** `JetBrains Mono` — telemetry readouts, T-minus timers, coordinates.

Scale: 11 / 12 / 14 / 16 / 20 / 28 / 40 / 64 / 96.

11–14px letterspaced caps dominate the chrome; 64–96px for a vehicle/mission title over film.

## 4. Component Stylings

**Full-bleed film hero** (the whole design)
- Autoplaying muted looping footage of a vehicle / launch / orbit; edge-to-edge.
- Minimal centered or bottom-left UPPERCASE label; optional thin CTA.
- Scrim only where text sits (bottom or radial), never a full darkening that hides the footage.

**Buttons**
- Primary: thin 1px `--border-strong` white outline, UPPERCASE letterspaced label, transparent fill; hover fills white with black text. (e.g. "EXPLORE", "WATCH").
- No pills, no fills at rest — outline is the register.

**Nav**
- Transparent over film, UPPERCASE letterspaced links, generous spacing, hairline divider on scroll only. Wordmark "SPACEX" letterspaced.

**Mission / launch strip**
- Full-width dark band: mission name (caps) + vehicle + date + a mono countdown; hairline `--border` separators. Tabular/mono numerics.

**Cards (rare)**
- `--surface` over black, 1px `--border` hairline, radius 2–4px (near-square). Image-led, caption in caps.

**Inputs (rare)**
- Transparent fill, 1px `--border`, square-ish; focus → `--border-strong`. Mono for any ID/coordinate.

## 5. Layout Principles

- Full-bleed sections stacked vertically; each is essentially one piece of footage + one label.
- Content confined to generous margins; center or bottom-left anchoring.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96.
- Hard, near-square geometry (2–4px radii); hairline white rules for any structure.
- Desktop-first cinematic; scales down but never loses the full-bleed footage.

## 6. Depth & Elevation

Pure black — there is no elevation system to speak of; footage and hairline white rules provide all structure.

- Rare card: `0 8px 30px rgba(0,0,0,0.6)`.
- Text-scrims are linear `rgba(0,0,0,0 → 0.5)` only where labels sit.

No neumorphism, no glow, no gradients on chrome. Flat black + film.

## 7. Do's and Don'ts

**Do**
- Let full-bleed footage be the design; keep type minimal and out of the way.
- Use letterspaced UPPERCASE for chrome, nav, and labels.
- Thin white-outline buttons that fill on hover.
- Tabular/mono numerals for countdowns, altitude, velocity, payload.
- Keep everything monochrome; scrim only under text.

**Don't**
- Introduce any brand accent colour (the red is alert-only, near-never).
- Use rounded pills or filled buttons at rest.
- Darken footage globally or add decorative gradients.
- Set long body copy in caps (labels/titles only).
- Add shadows/glow as decoration.

## 8. Responsive Behavior

- Footage crops to keep the vehicle/subject framed; hero label scales 96 → 34 on mobile.
- Nav collapses to a minimal menu; letterspacing tightens slightly.
- Full-bleed sections stack; mission strips scroll horizontally with hairline separators.
- Desktop-first; never sacrifice the edge-to-edge footage.

## 9. Motion Notes

- Footage autoplays muted, loops; honour `prefers-reduced-motion` with a still frame.
- Transitions are slow, weighty, and few (300–500ms) — monumental, not snappy.
- Countdowns tick in mono; only the active timer animates.

## 10. Agent Prompt Guide

Bias: pure black canvas (#000), full-bleed rocket/launch footage as the entire design, strictly monochrome (white on black, no brand accent), letterspaced UPPERCASE chrome/nav/labels (D-DIN/Gotham/Inter), thin white-outline buttons that fill on hover, near-square geometry + hairline white rules, tabular/mono for countdowns/altitude/velocity/payload, scrim only under text, slow weighty motion.

Reject: any brand accent colour, rounded pills or filled-at-rest buttons, global footage darkening or decorative gradients, body copy set in caps, shadows/glow as decoration, snappy/bouncy motion.
