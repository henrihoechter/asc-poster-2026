# asc-poster-2026

Stable redirect target for the QR code on the ASC 2026 poster
(3LPo1G-05, *Assessing Vanadium Oxide Smart Insulation for Fusion-relevant
HTS Magnets*). The QR code encodes this repo's GitHub Pages URL, which never
changes — only the contents of this repo change when the destination changes.

| File | Size | Served as |
|---|---|---|
| `poster.pdf` | 21 MB | print-quality export, what the QR code resolves to |
| `poster-web.pdf` | 2.2 MB | downsampled export, offered as the slow-connection fallback |
| `index.html` | — | meta-refresh from the Pages root to `poster.pdf` |

Both PDFs are the 2026-09-04 export of `src/poster/asc2026.typ` plus the
Affinity layout, at 1828 × 914 mm, and differ only in raster resolution.

## To repoint the QR code

Edit the `url=` of the `<meta http-equiv="refresh" ...>` line in `index.html`
to the new destination (a different PDF, a Zenodo DOI, an interactive site),
commit and push. Live within about a minute, no reprint needed.
