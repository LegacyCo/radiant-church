# Radiant Church Design System

Design tokens, typography, and component styles for [radiantcentralcoast.com](https://radiantcentralcoast.com).

## Structure

```
radiant-church/
├── design.md               ← Full human-readable design system
├── design-system.json      ← Machine-readable token definitions
├── tokens/
│   ├── index.css           ← Import all tokens (entry point)
│   ├── colors.css          ← Color primitives + semantic tokens
│   ├── typography.css      ← Font faces, scale, callout pattern
│   └── spacing.css         ← Spacing scale, border radius, shadows
├── components/
│   ├── buttons.css
│   ├── forms.css
│   ├── navigation.css
│   └── content-blocks.css
└── fonts/
    └── README.md           ← Font sourcing notes
```

## Quick Start

```css
@import './tokens/index.css';
```

## Fonts

Two primary families:
- **Aktiv Grotesk Extended** — headings
- **Aktiv Grotesk Condensed** — body copy

Two custom display fonts (self-hosted via Squarespace):
- **span-semiboldcomp** — `<em>` callouts in headings, mobile nav
- **span-regularconditalic** — small text callouts, nav controls

See [`design.md`](./design.md) for the full system.
