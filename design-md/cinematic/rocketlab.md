# Rocket Lab — Cinematic Dark

Reference DESIGN.md for an aerospace / end-to-end space company: near-black canvas, full-bleed aerial launch-complex film, oversized letterspaced condensed-uppercase display, a single signature red. Epic, industrial, mission-grade.

## 1. Visual Theme & Atmosphere

"The end-to-end space company." Rocket Lab's brand is scale and capability — wide aerial footage of the launch site, huge technical display type, and one decisive red mark. The register is engineered and cinematic, not playful; every screen should feel like a mission page.

Mood: epic, precise, industrial. Less consumer-tech, more "hardware that goes to orbit."

## 2. Color Palette & Roles

```
--bg:              #0a0a0a   /* near-black canvas */
--bg-alt:          #121316   /* section lift */
--surface:         #16181c   /* card */
--surface-raised:  #1e2126
--text:            #f4f5f6
--text-muted:      #a3a8b0
--text-dim:        #6b7178
--border:          #262a30
--border-strong:   #363b43
--on-film:         #ffffff

--accent:          #e4002b   /* Rocket Lab red — logo, key CTA, live/launch marker */
--accent-hover:    #ff1f45
--accent-deep:     #b00020

/* mission / status */
--status-go:       #2fbf71   /* GO / nominal */
--status-hold:     #e6a417   /* hold / T-minus paused */
--status-abort:    #e4002b   /* abort / scrub (shares brand red) */
--status-idle:     #6b7178
```

Rule: red is scarce and load-bearing — the logo, one primary CTA, and the live/launch marker. Never wash surfaces in red or use it as a generic accent; its scarcity is what makes a launch feel serious.

## 3. Typography Rules

- **Display / hero:** condensed uppercase grotesque (`Saira Condensed`, `D-DIN Condensed`, `Oswald`, fallback `Arial Narrow`), heavy weight, **wide letter-spacing**, huge. This letterspaced-condensed-caps look is the brand signature (e.g. "THE END-TO-END SPACE COMPANY").
- **Headings:** same family, medium weight, uppercase for section labels.
- **Body / UI:** a technical sans (`Roboto`, `Inter`), weight 400/500, sentence case, line-height 1.5.
- **Numerals:** tabular for payload mass, altitude, T-minus clocks, mission counts.
- **Mono:** `JetBrains Mono`, `SF Mono` — mission IDs, coordinates, telemetry readouts, T-minus timers.

Scale: 12 / 13 / 14 / 16 / 20 / 28 / 40 / 64 / 96 / 128.

96–128px letterspaced caps for the hero; 12–14px for body/UI; mono for telemetry.

## 4. Component Stylings

**Film hero** (the centrepiece)
- Full-bleed aerial/launch footage, muted loop. Dark bottom gradient scrim for legibility.
- Centered oversized letterspaced-caps headline in `--on-film`; a small "SCROLL FOR MORE" + down-arrow cue.
- Optional live-mission ribbon: `--accent` dot + `T- 00:14:22` mono countdown.

**Nav**
- Slim `--bg` bar, red-swoosh "R" logo + letterspaced "ROCKET LAB" wordmark left; hamburger/menu right.
- Transparent over film at top, solid on scroll.

**Mission / launch cards**
- `--surface` fill, 1px `--border`, radius 6px (hard, technical — not soft pills).
- Header: mission name (condensed caps) + status pill via `--status-*`.
- Metric strip: payload, orbit, customer, date — mono tabular, right-aligned.

**Stat tiles**
- Big tabular number + uppercase micro-label (launches, success rate, payload to orbit). Red underline used once for the headline stat only.

**Buttons**
- Primary: `--accent` fill, white text, radius 4px, uppercase, letter-spaced, weight 600 — used sparingly.
- Secondary: transparent, `--text`, 1px `--border-strong`, uppercase.

**Badges / tags**
- Small, squared (radius 3px), uppercase mono. Vehicle (Electron/Neutron), orbit, status.

**Inputs**
- `--bg-alt` fill, 1px `--border`, radius 4px. Focus: 2px `--accent` ring.
- Mono for any field taking a mission ID or coordinate.

## 5. Layout Principles

- 1280px max content shell, 24px gutter; film/mission sections break full-bleed.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96.
- Alternating full-bleed footage and dark data sections (specs, mission tables).
- Hard rectangular geometry over rounded — reinforce the engineered register.
- Desktop-first for mission/spec density; responsive down.

## 6. Depth & Elevation

Near-black canvas — depth via background steps (`--bg` → `--bg-alt` → `--surface` → `--surface-raised`) and film layering, not glow.

- Card: `0 2px 12px rgba(0,0,0,0.5)`
- Overlay/menu: `0 12px 40px rgba(0,0,0,0.6)`
- Film scrims: linear `rgba(0,0,0,0 → 0.55)`.

No neumorphism, no coloured glow. Borders and hard edges carry structure.

## 7. Do's and Don'ts

**Do**
- Lead with wide aerial/launch footage and a dark scrim.
- Use oversized letterspaced condensed-uppercase display as the signature.
- Keep red scarce: logo, one CTA, live/launch marker only.
- Hard rectangular geometry (3–6px radii), uppercase micro-labels.
- Tabular mono numerals for payload, altitude, T-minus clocks.

**Don't**
- Wash surfaces in red or use it as a generic accent.
- Soften into rounded pills or playful shapes.
- Go light-canvas — the register is dark and cinematic.
- Set long body copy in condensed caps (display only; body is sentence-case sans).
- Add coloured glows or gradients on chrome.

## 8. Responsive Behavior

- Hero footage crops to keep the vehicle/site in frame; display scales 128 → 40 on mobile.
- Nav collapses to a menu; live-mission ribbon persists.
- Full-bleed media stacks; spec tables scroll horizontally with a sticky first column.
- Mission dashboards are desktop-first; mobile is read-mostly.

## 9. Motion Notes

- Hero footage autoplays muted and loops; honour `prefers-reduced-motion` with a still frame.
- Live countdowns tick in mono; only the active timer/marker animates.
- Transitions are crisp and controlled (200–350ms) — engineered, not bouncy.

## 10. Agent Prompt Guide

Bias: near-black canvas (#0a0a0a), full-bleed aerial cinematic film with dark scrim, oversized letterspaced condensed-uppercase display (Saira/D-DIN Condensed) at 96–128px, scarce load-bearing Rocket Lab red (#e4002b) for logo/one-CTA/live-marker, technical sans body, tabular mono for payload/altitude/T-minus, hard rectangular geometry (3–6px radii), uppercase micro-labels, crisp controlled motion.

Reject: red as a generic accent or surface wash, rounded pills / playful shapes, light canvas, body copy set in condensed caps, coloured glows/gradients on chrome, bouncy motion, centered numeric columns.
