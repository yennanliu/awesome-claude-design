# Langfuse — Data-Dense Pro

Reference DESIGN.md for a light, high-contrast, keyboard-driven console for tracing and evaluating LLM & agent applications. Open-source developer tooling; trace trees, token/cost/latency metrics, and eval scores as the UI.

## 1. Visual Theme & Atmosphere

Open-source dev tool, on paper. Warm off-white canvas, near-black text, and a single loud signature: a yellow highlighter marker used like someone took a real one to the page. Keyboard shortcuts surfaced inline — this is a tool for engineers who live in it.

Mood: technical, high-contrast, quietly confident, a touch playful via the marker. Less SaaS-gradient, more "well-typeset README that happens to be an app."

## 2. Color Palette & Roles

```
--bg:              #f6f5ef   /* warm off-white paper — app canvas */
--bg-alt:          #efeee7   /* sidebar / rail / inset */
--surface:         #ffffff   /* card, dialog, raised row */
--text:            #0a0a0a   /* near-black, primary */
--text-muted:      #6b6b63
--text-dim:        #9a9a90
--border:          #e3e2d9
--border-strong:   #cfcec3

--ink:             #111111   /* primary buttons, strong UI, keyboard badges */
--ink-hover:       #2a2a2a

--highlight:       #f5f56b   /* SIGNATURE yellow marker — brand, text highlight, active row */
--highlight-strong:#ebeb3d   /* denser yellow for selected / focus marker */
--link:            #1d4ed8   /* the one functional blue — inline links only */

/* observation / span types (Langfuse trace primitives) */
--obs-generation:  #7c3aed   /* GENERATION (LLM call) */
--obs-span:        #2563eb   /* SPAN (nested work) */
--obs-event:       #0891b2   /* EVENT (point-in-time) */
--obs-tool:        #d97706   /* TOOL / retriever call */

/* score / status */
--score-pass:      #16a34a
--score-fail:      #dc2626
--score-partial:   #d97706
--status-error:    #dc2626
--status-pending:  #9a9a90
```

Rule: yellow is a **highlight, not a CTA**. Primary actions are `--ink` (near-black) buttons. The marker marks — brand wordmark, the active trace row, a matched search term. Never fill a button or a large surface with `--highlight`; it loses its punch and hurts legibility on text.

## 3. Typography Rules

- **UI / body:** `Inter`, system-ui fallback. Tabular numerals always on (`font-variant-numeric: tabular-nums`) for any token count, cost, latency, score, or stat column.
- **Display / hero:** Inter (or a grotesk like `Geist`), weight 700–800, very tight tracking, large. Hero text often sits on a `--highlight` marker band.
- **Mono / code / IDs:** `JetBrains Mono`, `Geist Mono`, `SF Mono`. Use for trace/observation IDs, model strings (`gpt-4o`, `claude-opus-4`), token counts in dense views, prompt diffs, JSON, and keyboard-shortcut badges.
- Stat values in the rail (GitHub stars, counts) are mono, right-aligned, tabular.

Scale: 11 / 12 / 13 / 14 / 16 / 18 / 20 / 24 / 32 / 48 / 64.

11–13px dominates the console (trace rows, score tables, rail stats). 48–64px reserved for the marker-highlighted marketing hero.

## 4. Component Stylings

**Keyboard-shortcut badges** (signature affordance)
- Inline next to buttons/links: a small `--surface` chip, 1px `--border-strong`, radius 4px, mono 11px, single letter (`S`, `D`, `G`).
- Sit to the right of the label inside or beside the control. Reinforce that the app is keyboard-first.

**Trace tree / observation waterfall** (the hero component)
- Left: collapsible tree of observations (GENERATION / SPAN / EVENT / TOOL), 28px rows, 16px indent per nesting level.
- Each node: type dot coloured by `--obs-*` + name (Inter 500) + duration (mono, right-aligned).
- Right: timeline waterfall, bar coloured by `--obs-*`, on a shared time ruler (sticky).
- Selected node gets a `--highlight` marker band across the full row.
- Drill-in detail drawer shows input/output, model, token in/out, cost — mono.

**Metric tiles & rail stats**
- Compact rows: label (`--text-muted`) left, value (mono tabular, `--text`) right-aligned.
- Sparkline or tiny bar optional; keep ≤ 24px tall. No big chart chrome in the rail.

**Score / eval tables**
- Row height 32px, zebra `--bg-alt` on odd rows, sticky header.
- Score cells: numeric mono right-aligned; pass/fail/partial pill via `--score-*`.
- Trace ID column mono with copy-on-hover.

**Buttons**
- Primary: `--ink` fill, white text, radius 8px, weight 600 — often with a kbd badge.
- Secondary: `--surface` fill, `--text`, 1px `--border-strong`.
- Destructive: `--status-error` text on `--surface` outline, fill only on confirm.

**Badges / tags**
- Pill, 20px tall, 11px. Model, environment (`prod`/`staging`), prompt version `v3`.
- Observation-type tags use `--obs-*` text on a 10%-alpha tint.

**Inputs**
- `--surface` fill, 1px `--border`, radius 6px. Focus: 2px `--ink` ring, 2px offset.
- Search match highlights the term with a `--highlight` marker span.
- Mono font for any field taking an ID, model string, or filter DSL.

## 5. Layout Principles

- Marketing pages: 1200px max, 24px gutter; persistent left info-rail (community stats, changelog) is part of the brand.
- Console: full-viewport, resizable panels, no max-width.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Left nav 240px (projects / tracing / evals / prompts / datasets), collapsible to 56px.
- Trace view splits ~60/40: tree+waterfall vs. selected-observation detail drawer (resizable).
- Subtle diagonal-hatch texture allowed in empty/hero corners only — never behind data.

## 6. Depth & Elevation

Light paper canvas — depth via background steps (`--bg` → `--bg-alt` → `--surface`) and crisp 1px borders, not shadow.

Shadows sparingly:
- Cards: `0 1px 2px rgba(0,0,0,0.05)`
- Popover/menu: `0 8px 24px rgba(0,0,0,0.10)`
- Dialog: `0 16px 48px rgba(0,0,0,0.14)`

No neumorphism, no glow, no gradients on primary surfaces. Borders and the yellow marker carry emphasis. Glassmorphism only on transient overlays.

## 7. Do's and Don'ts

**Do**
- Keep yellow as a highlight/marker; make primary buttons near-black `--ink`.
- Surface keyboard shortcuts as kbd badges on key actions.
- Tabular mono numerals for tokens, cost, latency, scores, and rail stats.
- Mono for trace/observation IDs, model strings, prompt versions.
- Make the trace tree + waterfall the centre of gravity.
- Colour observation rows by type consistently across tree and timeline.

**Don't**
- Fill buttons or large surfaces with `--highlight` yellow.
- Use a dark primary console canvas (Langfuse is paper-light).
- Center-align numeric columns.
- Put the hatch texture or any decoration behind live data.
- Reuse score green/red for non-eval meaning.
- Drop below font-weight 400 for body text at 11–13px.

## 8. Responsive Behavior

- Desktop-first for tracing/evals — do not force the waterfall into 375px.
- Tablet (768–1024px): detail drawer becomes a modal; tree stacks over timeline.
- Mobile (< 768px): read-only trace summaries, score cards, and stats; swipe between traces. Prompt/eval editing is desktop-only.

## 9. Real-Time & State Notes

- Traces stream in as runs complete (SSE/polling); new observations append without reflowing the whole tree.
- Pending observations render `--status-pending` and reconcile to a type colour on completion; errored spans get a `--status-error` left accent.
- Long-running generations show an indeterminate bar on that span only — don't animate the whole waterfall.
- Show ingestion/connection state so engineers trust live data; dim stale data to `--text-dim` after disconnect rather than implying it's current.

## 10. Agent Prompt Guide

Bias: warm off-white canvas (#f6f5ef), near-black text (#0a0a0a), Inter + JetBrains Mono, tabular numerals, signature yellow highlighter (#f5f56b) as marker only, near-black (#ink) primary buttons, keyboard-shortcut kbd badges, 4px grid, trace-tree + waterfall as the hero, observation-type colour coding (generation #7c3aed / span #2563eb / event #0891b2 / tool #d97706), eval score pass/fail pills, mono for all IDs/models/prompt versions.

Reject: dark primary canvas, yellow used as a button/CTA fill, non-tabular numerals, serif body, gradients/glow on surfaces, decoration behind data, centered numeric columns, score colours used decoratively.
