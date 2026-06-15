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
- The app loads Tailwind CSS and SheetJS from public CDNs.
- Do not commit credentials, tokens, or private deployment settings into this project.
