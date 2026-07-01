# Hugging Face — Data-Dense Pro

Reference DESIGN.md for the AI community's model & dataset hub: a dark, browsable index where thousands of repos are scannable at a glance. Dense repo cards, mono model IDs, tabular download/like counts, and modality filters — with one warm yellow brand accent and the 🤗 mark.

## 1. Visual Theme & Atmosphere

The AI community, indexed. Hugging Face is a hub — the design's job is to make a firehose of models, datasets, and Spaces legible and filterable. Near-black canvas so repo cards and counts pop, a single warm yellow accent from the mark, and just enough playfulness (emoji task icons) to feel like a community, not a terminal.

Mood: dense but friendly, developer-first, alive. Less "enterprise dashboard," more "the front page of open-source ML."

## 2. Color Palette & Roles

```
--bg:              #0a0a0c   /* app canvas — near-black */
--bg-alt:          #111114   /* rail / filter column */
--surface:         #16161b   /* repo card / row */
--surface-raised:  #1e1e25   /* hover, popover */
--text:            #f5f5f7
--text-muted:      #a0a0aa
--text-dim:        #6a6a74
--border:          #26262e
--border-strong:   #35353f

--accent:          #ffd21e   /* HF yellow — brand, active filter, key highlight */
--accent-hover:    #ffde54
--accent-tint:     #2a2610   /* low-alpha yellow behind badges */
--link:            #7aa2ff   /* repo/user links */

/* modality / category (task & library tags) */
--cat-nlp:         #ff9d5c   /* text tasks */
--cat-vision:      #6ea8ff   /* image/video */
--cat-audio:       #37d0a8   /* speech/audio */
--cat-multi:       #c084fc   /* any-to-any / multimodal */
--cat-lib:         #f7d154   /* libraries (PyTorch, JAX…) */

/* metric signals */
--trending:        #ffd21e   /* the ⚡ trending bolt */
--downloads:       #a0a0aa
--likes:           #ff6b81   /* ♥ likes */
```

Rule: yellow is the brand + "active/trending" signal — use it sparingly (mark, selected filter, trending bolt), never as a surface wash. Category hues are for task/library tags only; keep them consistent across cards and filters so the eye learns them.

## 3. Typography Rules

- **UI / body:** `Inter`, `IBM Plex Sans`, system-ui. Tabular numerals always on (`font-variant-numeric: tabular-nums`) for download counts, likes, param sizes, dates.
- **Display / hero:** Inter/`Source Sans` weight 700–800, tight tracking, large ("The AI community building the future.").
- **Mono / IDs:** `IBM Plex Mono`, `JetBrains Mono`, `SF Mono`. Use for repo IDs (`org/model-name`), revision hashes, param counts (`120B`), file names, and code snippets.
- Repo names are mono; org avatars sit inline to the left.

Scale: 11 / 12 / 13 / 14 / 16 / 20 / 24 / 32 / 44 / 60.

11–13px dominates the hub (repo rows, filter chips, counts). 44–60px for the marketing hero only.

## 4. Component Stylings

**Repo cards / rows** (the workhorse)
- `--surface` fill, 1px `--border`, radius 10px. Hover → `--surface-raised` + 1px `--border-strong`.
- Row 1: org avatar + `org/repo` in mono + trending ⚡ (`--trending`) if hot.
- Row 2 (meta strip): task tag (category-coloured) · param size (mono) · "Updated 2 days ago" (`--text-dim`) · ⬇ downloads (tabular) · ♥ likes (`--likes`, tabular).
- Numeric meta right-aligned, tabular, mono.

**Filter column**
- Grouped facets: Tasks, Libraries, Languages, Licenses, param-size slider.
- Task chips carry a tiny emoji/icon + label; selected chip → `--accent-tint` bg + `--accent` text + 1px `--accent`.
- Param slider is a labeled range (`<1B … >500B`), values in mono.

**Result header**
- "Models 2,555,000" — big tabular count + a "Filter by name" mono input + sort dropdown.

**Buttons**
- Primary: `--accent` yellow fill, `#0a0a0c` dark text, radius 8px, weight 600 (e.g. "Sign Up").
- Secondary: `--surface` fill, `--text`, 1px `--border-strong` (e.g. "Explore AI Apps").
- Ghost/link: `--link`, underline on hover.

**Badges / tags**
- Pill, 20px tall, 11px. Task, library, license, "NEW". Category-coloured text on a 10%-alpha tint.
- Model-size / license badges in mono.

**Inputs**
- Global search: `--bg-alt` fill, 1px `--border`, radius 8px, placeholder `--text-dim`, mono.
- Focus: 2px `--accent` ring, 2px offset.

## 5. Layout Principles

- Marketing hero: split — bold headline + CTAs left, a live dense repo/task panel right (bleeds off the edge).
- Hub: left filter column (240–280px) + main results grid/list, full-viewport, no max-width.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Repo list is single-column dense rows on narrow, 2–3 col cards on wide.

## 6. Depth & Elevation

Near-black canvas — depth via background steps (`--bg` → `--bg-alt` → `--surface` → `--surface-raised`), not shadow.

Shadows sparingly:
- Popover/menu: `0 8px 24px rgba(0,0,0,0.5)`
- Dialog: `0 16px 48px rgba(0,0,0,0.6)`

Borders carry separation. No neumorphism, no glow. Emoji/task icons add warmth instead of decoration.

## 7. Do's and Don'ts

**Do**
- Tabular mono numerals for downloads, likes, params, dates.
- Mono for repo IDs, revisions, file names.
- Keep yellow scarce: brand mark, selected filter, trending bolt.
- Use consistent category colours for tasks/libraries across cards and filters.
- Let repo cards be dense and scannable; meta strip does the work.

**Don't**
- Wash surfaces in yellow or use it as a generic accent.
- Center-align numeric/meta columns.
- Drop tabular numerals on any count.
- Overload cards with chrome — the meta strip + tags are enough.
- Use serif or non-mono for repo identifiers.

## 8. Responsive Behavior

- Desktop-first for the hub — filter column + dense results.
- Tablet (768–1024px): filters collapse into a drawer/modal; results go 2-up.
- Mobile (< 768px): search + single-column repo rows; filters behind a button; marketing hero stacks headline over the panel.

## 9. Real-Time & Community Notes

- Counts (downloads/likes) update live-ish; keep them tabular so numbers don't jitter width.
- Trending ⚡ is computed — surface it consistently; don't fake it per render.
- Community signals (likes ♥, org avatars) are first-class — they build trust in a repo at a glance.

## 10. Agent Prompt Guide

Bias: near-black canvas (#0a0a0c), one warm HF yellow accent used scarcely (#ffd21e — brand/selected/trending), Inter + IBM Plex Mono, tabular numerals, dense repo cards with `org/repo` mono IDs + meta strip (task tag · params · updated · ⬇ downloads · ♥ likes), left facet filter column with emoji task chips, category colours for tasks/libraries, 4px grid.

Reject: yellow as surface wash or generic accent, light primary canvas for the hub, non-tabular counts, centered numeric columns, serif/non-mono repo identifiers, over-chromed cards.
