# CrewAI — Data-Dense Pro

Reference DESIGN.md for a dark-first, telemetry-heavy console that runs, observes, and debugs fleets of autonomous agents. Multi-agent orchestration as the product; execution traces, token/cost meters, and run state as the UI.

## 1. Visual Theme & Atmosphere

Mission control for agents. A dense observability console where a single crew run spawns dozens of agent spans — the UI's job is to make that legible at a glance and drillable to the token.

Dark canvas primary (the dashboard lives here for hours), warm red-orange accent borrowed from the CrewAI mark. Mood: production-grade, fast, slightly industrial. Less "AI toy demo," more "the SRE dashboard your agents run on."

## 2. Color Palette & Roles

```
--bg:              #0b0e14   /* app canvas */
--bg-alt:          #0f131b   /* panel / rail */
--surface:         #161b26   /* card / row */
--surface-raised:  #1c2230   /* dialog, popover, hover */
--text:            #e6e9ef
--text-muted:      #9aa4b5
--text-dim:        #5b6675
--border:          #232a38
--border-strong:   #313b4d

--accent:          #ff5e4d   /* CrewAI red-orange — primary CTA, active run, links */
--accent-hover:    #ff7563
--accent-light:    #2a1714   /* low-alpha tint behind accent badges on dark */

/* run / span status */
--status-running:  #ff5e4d   /* active, in-flight (often animated) */
--status-success:  #2dd4a7   /* completed OK */
--status-failed:   #f0506a   /* errored / exception */
--status-queued:   #c9a227   /* queued / waiting on dependency */
--status-idle:     #5b6675   /* not started / skipped */

/* categorical — agent roles, tool calls, span types */
--cat-1:           #ff5e4d
--cat-2:           #5b8cff
--cat-3:           #2dd4a7
--cat-4:           #c084fc
--cat-5:           #f5b14c
--cat-6:           #4cc9d6
```

Rule: status colours are reserved for run/span/task state. Never reuse `--status-success` green or `--status-failed` red as decorative or categorical fills — operators scan by colour to triage, and a false-positive green is worse than no colour.

## 3. Typography Rules

- **UI / body:** `Inter`, system-ui fallback. Tabular numerals always on (`font-variant-numeric: tabular-nums`) for token counts, latency, cost, and any metric column.
- **Display / hero:** Inter, weight 700–800, tight tracking (marketing pages only).
- **Mono / code / IDs:** `JetBrains Mono`, `SF Mono`. Use for run IDs, agent/task IDs, tool names, model strings (`gpt-4o`, `claude-opus-4`), prompts, JSON tool args, and log lines.
- Span/trace labels and the timeline ruler are mono — alignment matters more than warmth.

Scale: 11 / 12 / 13 / 14 / 16 / 18 / 20 / 24 / 32 / 48.

11–13px dominates the console (trace rows, log stream, metric tiles). 24px+ reserved for hero metrics and the marketing page.

## 4. Component Stylings

**Agent / crew cards**
- `--surface` fill, 1px `--border`, radius 10px.
- Header row: agent avatar/role icon + role name (Inter 600) + model badge (mono 11px).
- Status dot (8px) top-right, coloured by `--status-*`; running state pulses.
- Footer metric strip: tasks, tokens, cost, wall-time — mono, tabular, right-aligned.

**Execution trace / span timeline** (the hero component)
- Horizontal Gantt of spans on a shared time ruler. Row height 28px.
- Span bar filled by `--cat-*` (by agent) with a 2px left border in its `--status-*`.
- Nested tool calls indent 16px under their parent agent span; collapsible tree.
- Hover → tooltip with start offset, duration (ms), token in/out, tool name.
- Sticky time ruler (top) and sticky span-label gutter (left).

**Run tables**
- Row height 32px. Zebra `--bg-alt` on odd rows. Sticky header.
- Status pill in column 1; run ID mono + copy-on-hover.
- Numeric columns (tokens, cost, latency, retries) right-aligned, mono, tabular.
- Failed rows: 2px `--status-failed` left accent, never a full red fill.

**Log / output stream**
- Mono 12px on `--bg`, line-height 1.5. Timestamp gutter in `--text-dim`.
- Level tags: `INFO` muted, `WARN` `--status-queued`, `ERROR` `--status-failed`.
- Tool-call lines prefixed with the tool name in `--cat-*`; JSON args syntax-tinted.
- Auto-scroll with a "jump to latest" pill when scrolled up.

**Token / cost meters**
- Compact horizontal bar: used vs. budget, fill in `--accent`, track in `--surface`.
- Label: `1,284,302 tok · $4.17` mono tabular. Over-budget → bar turns `--status-failed`.

**Buttons**
- Primary: `--accent` fill, `#0b0e14` text (dark text on warm accent), radius 8px, weight 600.
- Secondary: `--surface` fill, `--text`, 1px `--border-strong`.
- Run control: "Run crew" primary; "Stop" uses `--status-failed` outline, not fill.

**Badges / tags**
- Pill, 20px tall, 11px mono. Agent role, model, tool, framework version.
- Model badges in `--accent-light` bg + `--accent` text.

**Inputs**
- `--bg-alt` fill, 1px `--border`, radius 6px.
- Focus: 2px `--accent` ring, 2px offset.
- Mono font for any field taking an ID, model string, or YAML/JSON config.

## 5. Layout Principles

- Marketing pages: 1200px max, 24px gutter, 12-column, light or dark sections.
- Console: full-viewport, resizable panels, no max-width.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Left rail 240px (crews / flows / deployments), collapsible to 56px icon rail.
- Primary split: trace/timeline gets 60–70% width; selected-span detail drawer gets the remainder (resizable, dismissible).
- Bottom dock for the live log stream, collapsible to a status bar.

## 6. Depth & Elevation

Dark canvas — depth via background steps (`--bg` → `--bg-alt` → `--surface` → `--surface-raised`), not shadow.

Shadows sparingly, and darker rather than softer:
- Popover/menu: `0 8px 24px rgba(0,0,0,0.45)`
- Dialog: `0 16px 48px rgba(0,0,0,0.55)`

Borders carry most separation. No neumorphism, no glow except a 1px `--accent` ring on the active/running element. Glassmorphism only for transient overlays.

## 7. Do's and Don'ts

**Do**
- Tabular mono numerals for every token count, cost, latency, and retry figure.
- Mono for run IDs, agent/task IDs, tool names, and model strings.
- Make the span timeline the centre of gravity — it's how operators debug.
- Animate only the running/in-flight state (pulse, indeterminate bar ≤ a slow loop).
- Keep status colour reserved strictly for run/span/task state.
- Offer copy-on-hover for every ID.

**Don't**
- Use status green/red as decorative or categorical colour.
- Light primary canvas for the console (reserve light for marketing).
- Center-align numeric columns.
- Animate the trace bars on every render — only the live span moves.
- Bury cost/token totals; they belong in the persistent header.
- Use font-weight below 400 for body text at 11–13px.

## 8. Responsive Behavior

- Desktop-first for the console — do not force the trace timeline into 375px.
- Tablet (768–1024px): collapse the detail drawer into a modal; stack timeline over logs.
- Mobile (< 768px): read-only run summary cards, status, and totals; swipe between runs. Editing crews/flows is desktop-only.

## 9. Real-Time & State Notes

- Live runs stream via SSE/WebSocket; new spans animate in from the right of the ruler.
- Use optimistic `--status-queued` immediately on dispatch, reconcile to running/success/failed.
- Never reflow the whole timeline on each tick — append and extend the active span only.
- Show a connection-state chip (live / reconnecting / replay) so operators trust the view.
- Stale data after disconnect must dim to `--text-muted`, not silently keep "running."

## 10. Agent Prompt Guide

Bias: dark canvas (#0b0e14), Inter + JetBrains Mono, tabular numerals, CrewAI red-orange accent (#ff5e4d), 4px grid, span/Gantt execution timeline as the hero, mono for all IDs/models/tools, status colour pair reserved for run state (success #2dd4a7 / failed #f0506a / running #ff5e4d), categorical palette for agent roles.

Reject: light primary console canvas, status colours used decoratively, non-tabular numerals, serif fonts, glows/shadows as primary separation, animating the whole trace on every tick, centered numeric columns.
