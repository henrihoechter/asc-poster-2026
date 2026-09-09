# asc-poster-2026

Landing page behind the QR code on the ASC 2026 poster (3LPo1G-05,
*Assessing Vanadium Oxide Smart Insulation for Fusion-relevant HTS Magnets*).
The QR code encodes this repo's GitHub Pages URL, which never changes — only
the contents of this repo change when the destination changes.

<https://henrihoechter.github.io/asc-poster-2026/>

| File | Size | Role |
|---|---|---|
| `index.html` | — | landing page: title, authors, download, contact |
| `poster.pdf` | 21 MB | print-quality export, the primary download |
| `poster-web.pdf` | 2.2 MB | downsampled export, offered as the slow-connection fallback |
| `poster-thumb.jpg` | 289 kB | 1584 px preview shown on the page |

Both PDFs are the 2026-09-04 export of the poster at 1828 × 914 mm and differ
only in raster resolution. The thumbnail is regenerated from the light export:

    pdftoppm -r 22 -jpeg -jpegopt quality=82 -f 1 -l 1 poster-web.pdf thumb

## To repoint the QR code

Either edit `index.html` in place, or replace it with a one-line meta refresh
to a new destination (a Zenodo DOI, an interactive site), then commit and push.
Live within about a minute, no reprint needed.
