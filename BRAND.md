# Brand System

This repo contains **two separate brand identities**. Do not mix them.

1. **EPCH** — our brand (the company doing the pitching). Use this for all
   EPCH-authored materials, including any DOCX we brand.
2. **Marley Medical** — an *example client / case study* referenced inside the
   pitch. Its assets exist only to illustrate Marley's work. **Never apply
   Marley styling to EPCH materials, and vice versa.**

The canonical source for EPCH tokens is the inline CSS `:root` block in
`index.html`. This file mirrors it for reuse — keep them in sync.

---

## EPCH (primary brand)

### Color
| Role | Value |
|------|-------|
| Accent — coral (signature) | `#ff6b5b` (site) / `#F07563` (favicon) |
| Coral, soft fill | `rgba(255, 107, 91, 0.12)` |
| Accent — emerald | `#10b981` |
| Accent — amber | `#f59e0b` |
| Background — primary | `#FAF9F7` (warm off-white) |
| Background — secondary | `#F3F2EF` |
| Surface / card | `#FFFFFF` |
| Text — primary | `#1C1917` (warm near-black) |
| Text — secondary | `#57534E` |
| Text — muted | `#94918C` |
| Border — subtle | `rgba(28, 25, 23, 0.06)` |
| Border — default | `rgba(28, 25, 23, 0.10)` |

### Typography
- **Display / headings:** Fraunces (serif) — `'Fraunces', Georgia, serif`, weight 500–600
- **Body:** DM Sans (sans) — `'DM Sans', system-ui, sans-serif`, weight 400–700
- **Mono:** `ui-monospace, "SF Mono", Menlo, Consolas, monospace`

### Shape & depth
- Radii: sm `0.5rem`, md `0.75rem`, lg `1rem`, xl `1.5rem`
- Shadow (card): `0 1px 3px rgba(28,25,23,0.06), 0 1px 2px rgba(28,25,23,0.04)`
- Shadow (elevated): `0 4px 12px rgba(28,25,23,0.08), 0 1px 3px rgba(28,25,23,0.06)`

### Wordmark / logo
- Monospace `{ EPCH }` curly-brace wordmark — see `favicon.svg`
  (coral circle, white SF Mono text, curly braces at ~0.65 opacity).

---

## Marley Medical (example client — keep separate)

> Used only to depict the Marley case study within the pitch. Not EPCH.

### Color
| Role | Value |
|------|-------|
| Brand purple | `#5a38b2` |

### Assets
- `img/skill/marley-monogram-purple.svg` — squircle monogram
- `img/skill/icon-heart.svg`, `icon-pill.svg`, `icon-bp.svg`, `icon-stethoscope.svg` — purple line icons
- `img/marley-deck/` — rendered deck pages
- `Marley_Humana_MA_Pitch_v2_May2026.pdf` — source deck

---

## Quick reference (EPCH CSS tokens)
```css
:root {
  --bg-primary: #FAF9F7;
  --bg-secondary: #F3F2EF;
  --bg-card: #FFFFFF;
  --text-primary: #1C1917;
  --text-secondary: #57534E;
  --text-muted: #94918C;
  --accent-coral: #ff6b5b;
  --accent-coral-soft: rgba(255, 107, 91, 0.12);
  --accent-emerald: #10b981;
  --accent-amber: #f59e0b;
  --border-subtle: rgba(28, 25, 23, 0.06);
  --border-default: rgba(28, 25, 23, 0.10);
  --radius-sm: 0.5rem; --radius-md: 0.75rem; --radius-lg: 1rem; --radius-xl: 1.5rem;
  --font-display: 'Fraunces', Georgia, serif;
  --font-body: 'DM Sans', system-ui, sans-serif;
}
```
