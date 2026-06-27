# ruandom

Personal site at [ruandom.com](https://www.ruandom.com). Built with plain HTML/CSS/JS, hosted on GitHub Pages.

## Structure

```
index.html          Homepage with room navigation
garage.html         The Garage — owned cars, rentals, car spotting
favicon.svg         Lowercase "r" favicon
.nojekyll           Disables Jekyll on GitHub Pages
assets/
  css/style.css     All styles
  images/           Car, rental, and spotting photos
```

## Design tokens

| Token | Value | Use |
|---|---|---|
| `--bg` | `#FFFFFF` | Page background |
| `--card` | `#F4F4F4` | Card backgrounds |
| `--text` | `#111111` | Body text |
| `--muted` | `#888888` | Secondary text, captions |
| `--border` | `#E4E4E4` | Dividers |
| `--surface` | `#EBEBEB` | Photo placeholders |
| `--accent` | `#FFD100` | Accent (Porsche ceramic brake caliper yellow) |
| `#B8900A` | *(inline)* | Small accent labels (readable on white) |

Font: [Raleway](https://fonts.google.com/specimen/Raleway) via Google Fonts.

## Images

All photos are square (1:1), compressed via `sips` (max 1200px, 75% JPEG quality). To re-compress after adding new images:

```bash
sips -Z 1200 --setProperty formatOptions 75 assets/images/**/*.{jpg,jpeg,png}
```

Images use `loading="lazy"` and `class="zoomable"` for the lightbox.

