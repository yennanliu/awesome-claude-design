# AWS — Data-Dense Pro

Reference DESIGN.md for enterprise cloud at scale: the squid-ink + smile-orange identity, Amazon Ember type, and the famously dense AWS Console. Marketing is dark and campaign-driven; the product surface is a high-density control plane of services, resources, and billing. Multi-region, multi-locale (this reference captured on the Japan site).

## 1. Visual Theme & Atmosphere

Industrial-grade cloud. AWS has to signal reliability across 200+ services and every enterprise on earth — so the identity is sober navy, a single confident orange, and information density that assumes a professional operator. Marketing layers in a campaign motif (magenta pixel-gradient), but the durable core is Squid Ink + Smile Orange.

Mood: dependable, technical, enterprise. Less lifestyle, more "the console your infra runs on."

## 2. Color Palette & Roles

```
--bg:              #0f1b2d   /* app / marketing canvas — deep navy */
--bg-alt:          #16273d   /* panel / section lift */
--squid-ink:       #232f3e   /* AWS navy — global nav, headers */
--surface:         #ffffff   /* console works on white; cards on marketing dark */
--surface-dark:    #1a2739   /* card on dark sections */
--text:            #ffffff   /* on dark */
--text-ink:        #16191f   /* on light (console) */
--text-muted:      #b6c2d2
--text-dim:        #7d8ba0
--border:          #e9ebed   /* on light console surfaces */
--border-dark:     #2a3a52   /* on dark marketing surfaces */

--accent:          #ff9900   /* Smile Orange — primary CTA, active, highlights */
--accent-hover:    #ec7211   /* deeper orange, pressed */
--link:            #0972d3   /* console blue — links, secondary actions */
--link-hover:      #0561a5

/* campaign accent (marketing only) */
--campaign-a:      #e0218a   /* magenta */
--campaign-b:      #c724b1   /* violet-magenta gradient partner */

/* status (console) */
--status-ok:       #037f0c   /* healthy / running */
--status-warn:     #b25d00   /* warning */
--status-error:    #d13212   /* alarm / failed */
--status-info:     #0972d3
```

Rule: Smile Orange is the primary action colour; console blue is for links/secondary. The magenta campaign gradient is decorative and marketing-only — never let it stand in for the orange CTA or a status colour.

## 3. Typography Rules

- **UI / body:** `Amazon Ember`, `Inter`, system-ui fallback. Tabular numerals on (`font-variant-numeric: tabular-nums`) for pricing, resource counts, metrics, and any console column.
- **Display / hero:** Amazon Ember, weight 700, tight tracking.
- **Mono / code / IDs:** `Amazon Ember Mono`, `SF Mono`, `JetBrains Mono`. Use for ARNs, resource IDs (`i-0a1b2c…`), region codes (`ap-northeast-1`), CLI snippets, JSON/YAML, and log lines.
- **CJK / i18n:** always include a regional stack — `Noto Sans JP`, `Noto Sans TC`, `Noto Sans KR`; AWS serves every locale (this reference is the JP site).

Scale: 12 / 13 / 14 / 16 / 18 / 20 / 24 / 32 / 40 / 56.

12–14px dominates the console (resource tables, nav, breadcrumb). 32–56px reserved for marketing hero.

## 4. Component Stylings

**Global navigation**
- Full-width `--squid-ink` bar, white text, orange hover underline. Account/region menus right-aligned.
- Secondary product nav below on white with `--border` hairline.

**Resource tables** (the console workhorse)
- Row height 36px, sticky header, zebra on white (`#fafafa` odd rows). Selectable rows with checkbox column.
- Resource IDs/ARNs mono + copy-on-hover. Numeric columns right-aligned tabular.
- Status cell: coloured dot + label via `--status-*`; never a full-row fill.

**Service cards / tiles (marketing)**
- Glassy card on dark: `--surface-dark` with 1px `--border-dark`, radius 12px, subtle inner highlight.
- Icon + service name (Ember 700) + one-line description; orange "Learn more" link.
- Campaign sections may use the magenta pixel-gradient block motif behind, not on, content.

**Metric / billing tiles**
- Compact: label (`--text-muted`) + big tabular value + delta. Cost figures mono, right-aligned, currency per locale.

**Buttons**
- Primary: `--accent` fill, `--squid-ink` text, radius 8px (marketing) / 4px (console), weight 700.
- Secondary: white/transparent fill, `--link` text, 1px border.
- Pill CTAs on marketing ("AWS で無料で始める"): fully rounded, high contrast.

**Badges / tags**
- Pill, 20px tall, 11px. Region, service category, "New", pricing tier.
- Region/service badges mono in `--bg-alt` + `--text-muted`.

**Inputs**
- White fill (console) `#ffffff`, 1px `--border`, radius 4px. Focus: 2px `--link` ring.
- Mono for any field taking an ARN, resource ID, or region code.

## 5. Layout Principles

- Marketing: 1200px max, 24px gutter, alternating dark/navy sections; glassy cards.
- Console: full-viewport, left service rail, resizable, no max-width; extreme density is expected.
- 4px base grid. Spacing scale: 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64.
- Console left nav ~240px (services / resources), collapsible; breadcrumb bar persistent.
- Marketing hero: left-anchored glass card over a campaign-gradient field.

## 6. Depth & Elevation

Marketing (dark): depth via navy steps (`--bg` → `--bg-alt` → `--surface-dark`) + glass cards with a faint 1px top highlight.

Console (light): flat, border-driven, minimal shadow —
- Card: `0 1px 4px rgba(0,0,0,0.08)`
- Dropdown/modal: `0 8px 24px rgba(0,0,0,0.15)`

No neumorphism. Gradients belong to campaign backgrounds only, never on console chrome or buttons.

## 7. Do's and Don'ts

**Do**
- Keep Smile Orange as the single primary action colour; console blue for links.
- Amazon Ember everywhere; include a regional CJK stack for localized sites.
- Tabular mono numerals for pricing, metrics, and resource counts.
- Mono for ARNs, resource IDs, region codes.
- Confine the magenta campaign gradient to marketing backgrounds.
- Coloured status dots in console tables, never full-row fills.

**Don't**
- Let the campaign magenta replace the orange CTA or read as a status colour.
- Use dark canvas for the console (console is white/light for density).
- Center-align numeric columns.
- Assume one currency/locale — AWS is multi-region by default.
- Over-round console controls (4px there; pills are for marketing).

## 8. Responsive Behavior

- Console is desktop-first — do not force resource tables into 375px; allow horizontal scroll with a sticky first column.
- Tablet (768–1024px): collapse service rail to icons; stack marketing cards 2-up.
- Mobile (< 768px): marketing fully responsive; console is read-mostly (status, billing summary), heavy editing is desktop.

## 9. Internationalisation & Multi-Region Notes

- Every string localizes: language, currency, and region defaults (this reference is `ap-northeast-1` / 日本語).
- Currency per locale (¥ JPY, $ USD, € EUR…) with locale-correct separators; never hardcode USD.
- Region codes stay in mono ASCII (`ap-northeast-1`) even in localized UIs.
- Type stack must cover JP/TC/SC/KR without clipping line-height; keep layouts flex-direction reversible for RTL locales.
- Dates as `YYYY-MM-DD` in data, localized display (e.g. 2026-06-17) via Intl.

## 10. Agent Prompt Guide

Bias: Squid Ink navy (#232f3e / canvas #0f1b2d), Smile Orange primary action (#ff9900), console blue links (#0972d3), Amazon Ember + regional CJK stack, tabular numerals, dense white console resource tables with sticky headers, mono for ARNs/resource-IDs/region-codes, status dots (ok #037f0c / warn #b25d00 / error #d13212), 4px console radii / pill marketing CTAs, magenta pixel-gradient as marketing-only decoration.

Reject: campaign magenta used as CTA or status, dark-canvas console, non-tabular numerals, serif fonts, gradients on console chrome, centered numeric columns, hardcoded single currency/locale.
