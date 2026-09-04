# asc-poster-2026

Stable redirect target for the QR code on the ASC 2026 poster. The QR code
encodes this repo's GitHub Pages URL, which never changes — only the
contents of `index.html` change when the actual destination changes.

## To repoint the QR code

Edit `index.html`:
1. Remove the HTML comment block.
2. Uncomment the `<meta http-equiv="refresh" ...>` line and set `url=` to
   the real destination (hosted PDF, Zenodo DOI, interactive site, etc).
3. Commit and push. Live within ~1 minute, no reprint needed.
