# Waymo — Cinematic (Daylight)

Reference DESIGN.md for a premium autonomous-mobility brand: white chrome over full-bleed cinematic film of the vehicle in the real world, oversized light display type, Waymo blue + moss-green accents. A daylight variant of cinematic — media-first, but bright and trust-forward rather than dark.

## 1. Visual Theme & Atmosphere

"Because they're everything." Waymo sells trust in an autonomous car, so the hero is real footage of the vehicle driving a real street — cinematic, but sunlit and calm rather than moody. White chrome floats over the film; the type is large, light-weight, and gets out of the footage's way. Safety and human reassurance are the emotional core.

Mood: premium, calm, futuristic, human. Less "sci-fi dark," more "a beautiful ordinary morning, driven by software."

## 2. Color Palette & Roles

```
--bg:              #ffffff   /* canvas / chrome */
--bg-alt:          #f5f6f8   /* section lift */
--surface:         #ffffff   /* card */
--ink:             #0a0a0a   /* promo bar, footer, primary text on light */
--text:            #1a1c1f
--text-muted:      #5b6167
--text-dim:        #8a9098
--border:          #e6e8ec
--on-film:         #ffffff   /* text over video */

--accent:          #2f6bff   /* Waymo blue — CTA, links, active */
--accent-hover:    #1c53e0
--accent-deep:     #163fb0
--moss:            #34c98a   /* Waymo green — secondary highlight, sensor motif */
--moss-soft:       #e6f7ef

/* status (product / ride app) */
--status-go:       #34c98a   /* trip active / arrived */
--status-wait:     #f0a020   /* en route / waiting */
--status-alert:    #e0402e
```

Rule: Waymo blue is the one action colour; moss green is a secondary highlight and the "perception/sensor" motif — not a second CTA. Reserve status hues for ride/trip state, never decoration.

## 3. Typography Rules

- **Display / hero:** a light-to-regular grotesque (`Waymo Sans` → `Founders Grotesk`, `Neue Haas Grotesk`, `Inter`) at large sizes, weight 300–500, tight tracking. Hero lines run big over film.
- **Wordmark:** uppercase, wide letter-spacing (`WAYMO`) — treat as a lockup, not body type.
- **Body / UI:** same grotesque or `Inter`, weight 400/500, line-height 1.5–1.6.
- **Numerals:** tabular for wait times, ETAs, ratings, safety stats.
- **Mono:** `SF Mono`, `JetBrains Mono` — trip IDs, coordinates, telemetry only.

Scale: 12 / 14 / 16 / 18 / 22 / 28 / 36 / 48 / 64 / 88.

64–88px light display over the film hero; 14–18px for body and UI.

## 4. Component Stylings

**Film hero** (the centrepiece)
- Full-bleed autoplaying, muted, looping footage of the vehicle in daylight streets.
- Centered light display headline in `--on-film` white with a soft radial vignette / gentle bottom scrim for legibility.
- A pill "Watch the film" control with a circular play glyph; a discreet pause toggle bottom-left.

**Promo / utility bar**
- Slim `--ink` black bar above or below the hero: white text + a rounded `--accent` "Take a ride" pill.

**Buttons**
- Primary: `--accent` fill, white text, fully rounded pill, weight 500. Hover `--accent-hover`.
- On film / dark bars: white pill with `--ink` text, or `--accent` pill.
- Secondary: transparent, `--ink` text, 1px `--border`, pill.

**Cards (safety / tech / cities)**
- White fill, 1px `--border`, radius 16px, generous padding, soft shadow.
- Optional moss-green sensor/lidar motif line; imagery-forward, minimal chrome.

**Stat / safety tiles**
- Big tabular number + short label; moss or blue underline. For miles driven, safety comparisons.

**Nav**
- White, transparent-over-film at top then solid on scroll; letterspaced wordmark left, sparse links, search glyph, blue ride CTA right.

**Inputs (ride app)**
- White fill, 1px `--border`, radius 12px (large tap targets). Focus: 2px `--accent` ring.

## 5. Layout Principles

- 1200px max content shell, 24px gutter; hero and film sections break full-bleed to the edge.
- Generous vertical rhythm (56–96px between blocks) — let footage and whitespace breathe.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96.
- Alternating full-bleed media and centered-narrative sections.
- Mobile-first for the ride app; marketing is responsive desktop-down.

## 6. Depth & Elevation

Light, airy — depth from imagery layering and soft shadow, not heavy chrome.

- Card: `0 2px 12px rgba(10,10,10,0.06)`; hover `0 8px 24px rgba(10,10,10,0.10)`.
- Overlay controls on film: subtle blur + `rgba(0,0,0,0.25)` backing for contrast.
- No neumorphism, no hard gradients on flat surfaces; gradients only as film scrims.

## 7. Do's and Don'ts

**Do**
- Lead with real, sunlit footage of the vehicle; keep type light and out of the way.
- Add a scrim/vignette so white type stays legible over film.
- Keep Waymo blue as the single action colour; moss green as secondary/sensor motif.
- Fully rounded pill buttons; letterspaced uppercase wordmark.
- Tabular numerals for ETAs, wait times, and safety stats.

**Don't**
- Go dark-moody — Waymo's cinematic register is daylight and calm.
- Use heavy bold display weights that fight the footage.
- Turn moss green into a second CTA or use status colours decoratively.
- Let white text sit on film without a scrim.
- Over-chrome cards; imagery leads.

## 8. Responsive Behavior

- Hero film crops to keep the vehicle in frame; headline scales 88 → 32 on mobile.
- Nav collapses to a menu; the blue ride CTA persists.
- Full-bleed media stacks; narrative sections single-column.
- Ride-app surfaces are mobile-first with large tap targets and bottom sheets.

## 9. Motion Notes

- Hero footage autoplays muted and loops; respect `prefers-reduced-motion` (swap to a still frame).
- Transitions are gentle and slow (250–400ms ease) — reinforce calm/trust, never frantic.
- The sensor/perception motif (moss lines, point clouds) may animate subtly; keep it ambient.

## 10. Agent Prompt Guide

Bias: white canvas + chrome, full-bleed daylight cinematic film hero of the vehicle, light grotesque display (weight 300–500) at 64–88px over film with a scrim, Waymo blue single action colour (#2f6bff), moss green secondary/sensor motif (#34c98a), letterspaced uppercase wordmark, fully rounded pill buttons, tabular numerals for ETAs/safety stats, generous whitespace, calm slow motion.

Reject: dark-moody cinematic register, heavy bold display fighting the footage, moss green as a second CTA, status colours as decoration, unscrimmed white text on film, cramped spacing, frantic motion.
