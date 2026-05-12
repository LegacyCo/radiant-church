# style-reference/

A single-page reference site cataloging every format, CSS snippet, and visual example used by the Radiant Central Coast **/sermon-archive** master message template.

Lives inside this repo so it stays in lockstep with `tokens/` and `components/`. The page loads the canonical CSS directly via `../tokens/*.css` and `../components/*.css` — there is no duplication and no drift.

## Open it

```bash
# from the repo root
python -m http.server 4000
# then visit http://localhost:4000/style-reference/
```

## Files

```
style-reference/
├── index.html             ← The reference page
├── style-reference.css    ← Page chrome only (sidebar, layout, snippet UI)
└── README.md
```

The page consumes (read-only) the existing folders at the repo root:

```
tokens/index.css   tokens/colors.css   tokens/typography.css   tokens/spacing.css
components/buttons.css   components/content-blocks.css   components/forms.css   components/navigation.css
fonts/span-semiboldcomp.otf   fonts/span-regularconditalic.otf
```

## Format cards (16)

01. Color Tokens · 02. Typography & Callouts · 03. Buttons · 04. Hero Video Embed · 05. Metadata Row · 06. Summary Block · 07. More Sermons Carousel · 08. Next Steps Band · 09. Quote Block · 10. Accordion Block · 11. Text / HTML Block · 12. Marquee Block · 13. Image Overlays · 14. Form Block · 15. Announcement Bar · 16. Mobile Nav Overlay

Each card has a deep-link anchor (`#color-tokens`, `#hero-video`, …).

## Merging into the master skill

The reference site is intentionally separate from the design system source. To pull any card back into the skill: open the card, click **Copy** on its snippet, paste into the source file shown in the card header (e.g. `components/buttons.css`).

If you ever want to delete the reference site without affecting production styles, remove this folder. The rest of the repo is unchanged.
