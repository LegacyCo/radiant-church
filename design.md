# Radiant Church — Design System

**Site:** [radiantcentralcoast.com](https://radiantcentralcoast.com)

Radiant Church is a vibrant, welcoming community on the Central Coast of California, committed to connecting people to God, to each other, and to a life of purpose. This design system reflects warmth, clarity, and approachability — rooted in earthy, sun-warmed tones and clean, extended typography.

---

## Color Palette

### Primitives

| Token | Name | Hex | HSL |
|---|---|---|---|
| `--color-white` | Warm White | `#FAF3F0` | `12, 33%, 97%` |
| `--color-light-accent` | Soft Butter | `#FCF2BF` | `50.16, 91.04%, 86.86%` |
| `--color-accent` | Warm Sand | `#BEAD93` | `36, 25%, 66%` |
| `--color-dark-accent` | Warm Taupe | `#7A6F65` | `27, 10%, 43%` |
| `--color-black` | Dark Olive | `#474D47` | `120, 4%, 29%` |

### Semantic Assignments

| Role | Value |
|---|---|
| Site Background | `#FAF3F0` |
| Text Primary | `#474D47` |
| Text Heading | `#474D47` |
| Text Heading (bold section) | `#7A6F65` |
| Link | `#474D47` |
| Link Accent | `#BEAD93` |
| Block / Card Background | `#FCF2BF` |
| Image Overlay | `#7A6F65` |
| Global Image Overlay | `rgba(71, 77, 71, 0.5)` |
| Announcement Bar BG | `#474D47` |
| Announcement Bar Text | `#FAF3F0` |

### Button Colors

| Variant | Background | Text |
|---|---|---|
| Primary | `#BEAD93` (Warm Sand) | `#FCF2BF` (Soft Butter) |
| Secondary | `#474D47` (Dark Olive) | `#FCF2BF` (Soft Butter) |
| Tertiary | `#474D47` (Dark Olive) | `#FAF3F0` (Warm White) |

---

## Typography

### Font Families

| Role | Family | Usage |
|---|---|---|
| **Heading** | Aktiv Grotesk Extended | H1–H4 base |
| **Body** | Aktiv Grotesk Condensed | Paragraphs, body copy |
| **Callout** | span-semiboldcomp *(custom)* | `<em>` in headings, mobile nav |
| **Secondary Callout** | span-regularconditalic *(custom)* | Small text callouts, nav controls |

### Custom Font Sources

```css
@font-face {
  font-family: 'span-semiboldcomp';
  src: url('https://static1.squarespace.com/static/67f01da1e0b3122fc6194b9f/t/67f699ec98d97739a8fbd1b0/1744214509051/span-semiboldcomp.otf');
}

@font-face {
  font-family: 'span-regularconditalic';
  src: url('https://static1.squarespace.com/static/67f01da1e0b3122fc6194b9f/t/67f699e11c8d1130d62f082c/1744214497753/span-regularconditalic.otf');
}
```

### Desktop Type Scale

| Level | Font | Size | Notes |
|---|---|---|---|
| H1 | Aktiv Grotesk Extended | `120px` | |
| H1 `<em>` | span-semiboldcomp | inherits | Callout word |
| H2 | Aktiv Grotesk Extended | `118.4px` | |
| H2 `<em>` | span-semiboldcomp | inherits | |
| H3 | Aktiv Grotesk Extended | — | |
| H3 `<em>` | span-semiboldcomp | inherits | |
| H4 | Aktiv Grotesk Extended | — | |
| Body Medium | Aktiv Grotesk Condensed | `12.8px` | |
| Small Callout `<em>` | span-regularconditalic | `28px` | line-height `28px` |
| Summary Header | Aktiv Grotesk Extended | `22px` | `uppercase`, `font-weight: 600` |

### Mobile Type Scale (`max-width: 767px`)

| Level | Size |
|---|---|
| H1 | `50px` |
| H1 `<em>` | `55px` *(slightly larger for emphasis)* |
| H2 | `55px` |
| H2 `<em>` | `55px` |
| H3 | `55px` |
| H3 `<em>` | `55px` |

### Heading Callout Pattern

Wrapping a word in `<em>` inside `h1`–`h3` switches to **span-semiboldcomp**. `font-style: normal` suppresses the italic — `<em>` is used as a typographic switch, not for semantic emphasis.

```html
<h1>Join us <em>Sunday</em></h1>
```

### Hyphens

Automatic hyphenation is disabled globally on all headings. Line breaks must be intentional.

```css
h1, h2, h3, h4 { hyphens: manual !important; }
```

---

## Navigation

### Mobile Nav

| Selector | Font | Size | Transform |
|---|---|---|---|
| Nav links | span-semiboldcomp | `45px` | — |
| Nav controls (e.g., "close") | span-regularconditalic | `25px` | `lowercase` |

### Hamburger Menu

| Property | Value |
|---|---|
| Max height | `70vh` |
| Shadow opacity | `0.15` |
| Overlay opacity | `0` (hidden) |
| Overlay blur | `2px` |
| Bottom border | `2px currentColor` |

---

## Spacing & Shape

| Property | Value |
|---|---|
| Base unit | `4px` |
| Scale | 4, 8, 12, 16, 24, 32, 48, 64, 96 |
| Border radius — global | `0px` — all squares |
| Border radius — buttons | `300px` — full pill |
| Shadows | None |

---

## Components

### Buttons

| Property | Value |
|---|---|
| Border radius | `300px` pill |
| Width (all sizes) | `80%` of container |
| Shadow | None |

### Form Inputs

| Property | Value |
|---|---|
| Background | `#ffffff` |
| Text | `#474D47` |
| Border | `#DCD8D8` |
| Border radius | `0px` square |
| Shadow | None |
| Form block background | `#FCF2BF` |
| Submit button | bg `#474D47` / text `#FAF3F0` |

### Summary Block Headers

| Property | Value |
|---|---|
| Font weight | `600` |
| Font size | `22px` |
| Text transform | `uppercase` |

### Content Blocks (Quote, Accordion, Text, Marquee, Newsletter)

All content blocks share the same block background: `#FCF2BF` (Soft Butter).

---

## Brand Assets

| Asset | Notes |
|---|---|
| Logo | Horizontal, dark wordmark |
| Logo Alt | `Radiant Church` |
| Logo Link | `/` |

---

## Personality

| Attribute | Value |
|---|---|
| Tone | Professional |
| Energy | Medium |
| Audience | Churchgoers and community members on the Central Coast |
| Character | Warm, approachable, editorial — earthy tones with structured extended type |
