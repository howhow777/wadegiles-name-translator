# Wade-Giles Name Translator / 護照姓名中翻英轉譯器

A static browser-only web app for converting Chinese names into passport-style Wade-Giles or Hanyu Pinyin formats.

## GitHub Pages

This repository is intended to be served directly by GitHub Pages from the `main` branch root.

## Local run

```bash
python3 -m http.server 8787 --bind 127.0.0.1
```

Open: http://127.0.0.1:8787/

## Notes

- No backend service is required.
- Tailwind CSS and SheetJS are vendored under `assets/` so the GitHub Pages app does not depend on third-party CDN requests at runtime.
- Chinese readings use the vendored `pinyin-pro` browser bundle as a broad pure-JavaScript fallback when a character is not in the curated inline `PINYIN_DB` overrides.
- Wade-Giles fallback syllables use `assets/boca-wg-map.js`, generated from BOCA's passport-name reference table: https://www.boca.gov.tw/cp-2-4226-c0eff-1.html
- Do not commit credentials, tokens, or private deployment settings into this project.
