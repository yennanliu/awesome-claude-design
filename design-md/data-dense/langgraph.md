# LangGraph — Data-Dense Pro

Reference DESIGN.md for a dark, developer-first console for building and inspecting stateful agent graphs. Low-level orchestration framework as the product; the state machine / execution graph, node runs, and token telemetry as the UI.

## 1. Visual Theme & Atmosphere

Balance control with agency. LangGraph is a low-level agent runtime — the design has to feel like infrastructure you trust, not a demo. Near-black navy canvas, cool sky-blue accent, and a signature move: **monospace for all UI chrome** (nav, labels, buttons) against a clean geometric-sans display. Thin flowing graph lines evoke agent state transitions.

Mood: precise, engineered, calm. Less "AI magic," more "the runtime your agents actually run on."

## 2. Color Palette & Roles

```
--bg:              #0d1117   /* app canvas — near-black navy */
--bg-alt:          #111826   /* panel / rail */
--surface:         #161d2b   /* card / node */
--surface-raised:  #1d2637   /* dialog, popover, hover */
--text:            #e8eef7
--text-muted:      #9fb0c8
--text-dim:        #5d6b82
--border:          #202a3c
--border-strong:   #2d3a52

--accent:          #7aa8ff   /* sky blue — links, active node, focus */
--accent-hover:    #97bbff
--accent-soft:     #cfe0ff   /* periwinkle — display headlines on dark */
--accent-tint:     #142033   /* low-alpha blue behind badges */

/* node / run status */
--status-running:  #7aa8ff   /* in-flight (animated) */
--status-success:  #35c98d   /* completed OK */
--status-failed:   #f0506a   /* errored / exception */
--status-interrupt:#e6b450   /* human-in-the-loop / paused */
--status-idle:     #5d6b82

/* categorical — node types, edges, channels */
--cat-1:           #7aa8ff
--cat-2:           #b48cff
--cat-3:           #35c98d
--cat-4:           #f5a25d
--cat-5:           #4cc9d6
--cat-6:           #e879b9
```

Rule: status colours are reserved for node/run state. Never reuse success green or failed red as decorative or categorical fills — the graph is debugged by colour, and a false-positive green misleads.

## 3. Typography Rules

- **UI chrome (nav, labels, buttons, badges):** `JetBrains Mono`, `IBM Plex Mono`, `SF Mono`. The mono chrome is the signature — keep it for nav items, tab labels, button text, and the `langgraph` wordmark.
- **Display / hero:** geometric sans (`Public Sans`, `Inter`), weight 600–700, tight tracking, in `--accent-soft` periwinkle on dark.
- **Body / prose:** `Inter`, system-ui. Tabular numerals on (`font-variant-numeric: tabular-nums`) for token counts, step indices, latency, cost.
- **Code / IDs:** mono for node IDs, thread IDs, checkpoint IDs, state keys, model strings, JSON state, and log lines.

Scale: 11 / 12 / 13 / 14 / 16 / 20 / 24 / 32 / 44 / 64.

11–13px mono dominates the console (graph labels, state inspector, logs). 44–64px sans reserved for the marketing hero.

## 4. Component Stylings

**State graph / DAG** (the hero component)
- Nodes: `--surface` fill, 1px `--border`, radius 8px, mono label + type dot in `--cat-*`.
- Active/running node: 1px `--accent` ring + subtle pulse; completed nodes carry a `--status-success` left tick.
- Edges: 1px `--border-strong` bezier curves; conditional edges dashed; the live path highlights `--accent`.
- Thin converging "flow lines" motif allowed on the marketing hero only, never behind a live graph.

**State inspector / run detail**
- Key–value table of graph state per step. Mono keys, right-aligned tabular values, zebra `--bg-alt`.
- Step scrubber along the top; selecting a step diffs state (added/changed keys tinted).

**Run tables**
- Row height 32px, sticky header, zebra `--bg-alt`. Thread ID mono + copy-on-hover.
- Numeric columns (steps, tokens, cost, latency) right-aligned mono tabular.
- Failed rows: 2px `--status-failed` left accent, never a full red fill. Interrupted rows: `--status-interrupt`.

**Log / stream**
- Mono 12px on `--bg`, line-height 1.5. Timestamp gutter `--text-dim`.
- Level tags: `INFO` muted, `WARN` `--status-interrupt`, `ERROR` `--status-failed`.
- Node-scoped lines prefixed with the node name in `--cat-*`.

**Buttons**
- Primary: `--accent-soft` fill, `#0d1117` text, radius 6px, mono 13px weight 600.
- Secondary: transparent fill, `--text`, 1px `--border-strong`, mono (e.g. "Read the docs").
- Both keep the mono chrome look.

**Badges / tags**
- Pill, 20px tall, 11px mono. Node type, model, channel name, framework version.
- Model/version badges in `--accent-tint` bg + `--accent` text.

**Inputs**
- `--bg-alt` fill, 1px `--border`, radius 6px. Focus: 2px `--accent` ring, 2px offset.
- Mono for any field taking an ID, state key, or JSON/YAML config.

## 5. Layout Principles

- Marketing: 1200px max, 24px gutter, dark sections; thin line-art graphics bleed to the right edge.
- Console: full-viewport, resizable panels, no max-width.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Left rail 240px (graphs / threads / deployments), collapsible to 56px.
- Primary split: graph canvas 60–70%; selected-node / state drawer the remainder (resizable).
- Bottom dock for the run log, collapsible to a status bar.

## 6. Depth & Elevation

Dark canvas — depth via background steps (`--bg` → `--bg-alt` → `--surface` → `--surface-raised`), not shadow.

Shadows sparingly:
- Popover/menu: `0 8px 24px rgba(0,0,0,0.5)`
- Dialog: `0 16px 48px rgba(0,0,0,0.6)`

Borders and the 1px `--accent` ring on the active node carry separation. No neumorphism, no glow except the active-node ring. Glassmorphism only for transient overlays.

## 7. Do's and Don'ts

**Do**
- Keep monospace for all UI chrome — it's the brand's fingerprint.
- Pair mono chrome with a periwinkle geometric-sans display.
- Tabular mono numerals for tokens, steps, latency, cost.
- Make the state graph the centre of gravity; animate only the running node/edge.
- Reserve status colour strictly for node/run state.
- Copy-on-hover for thread / checkpoint / node IDs.

**Don't**
- Use status green/red as decorative or categorical colour.
- Light primary canvas for the console.
- Center-align numeric columns.
- Animate the whole graph on every tick — only the live path moves.
- Mix a second display typeface into the mono chrome.
- Drop below font-weight 400 for body at 11–13px.

## 8. Responsive Behavior

- Desktop-first for the graph canvas — do not force a DAG into 375px.
- Tablet (768–1024px): state drawer becomes a modal; graph stacks over logs.
- Mobile (< 768px): read-only run summaries, status, and token totals; swipe between threads. Graph editing is desktop-only.

## 9. Real-Time & State Notes

- Runs stream via SSE/WebSocket; nodes light up as they execute, edges animate along the live path.
- Human-in-the-loop interrupts render `--status-interrupt` and hold until resumed — make the paused node unmistakable.
- Checkpoints are first-class: show a checkpoint marker per step so operators can time-travel/replay.
- Never reflow the whole graph on each tick — update the active node/edge only.
- Stale data after disconnect dims to `--text-muted`; show a connection-state chip.

## 10. Agent Prompt Guide

Bias: near-black navy canvas (#0d1117), monospace UI chrome (JetBrains Mono) + periwinkle geometric-sans display (#cfe0ff), sky-blue accent (#7aa8ff), tabular numerals, 4px grid, state-graph/DAG as the hero, mono for all IDs/state-keys/models, status colours reserved for node state (success #35c98d / failed #f0506a / interrupt #e6b450 / running #7aa8ff), categorical palette for node types, thin flow-line motif on marketing only.

Reject: light primary console canvas, status colours used decoratively, non-tabular numerals, serif fonts, a second display typeface competing with the mono chrome, glows/shadows as primary separation, animating the whole graph every tick, centered numeric columns.
