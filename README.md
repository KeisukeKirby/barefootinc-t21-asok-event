# barefootinc-t21-asok-event

Landing page for **24th Absolute The Festival of Movement**
Vibram FiveFingers × Vivobarefoot — Barefootinc (Thailand)

- **Dates:** 15 September – 4 October 2026
- **Venue:** Terminal 21 Asok, G Floor (10:00–22:00, free entry)
- **Access:** BTS Asok Exit 1 / MRT Sukhumvit Exit 3

## Structure

Single static page, no build step.

| File | Purpose |
| --- | --- |
| `index.html` | The whole page. Images are inlined as base64 data URIs. |
| `og-image.jpg` | 1200×630 social preview image, referenced by `og:image` / `twitter:image`. |

## Editing copy

All user-facing text lives in the `I18N` object at the bottom of `index.html`
(`en` / `th`). Markup carries matching `data-i18n` keys. Thai-language browsers
get Thai automatically; the nav has a manual EN/TH switch.

## Deploy

Vercel, connected to this repository. Framework Preset `Other`, no build
command, no output directory — the repository root is served as-is. Pushes to
`main` deploy to production.
