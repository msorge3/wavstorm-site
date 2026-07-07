# Wavstorm Site

Static replacement for the old WordPress.com Wavstorm site.

## Local preview

```bash
cd public
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173`.

## Deployment

Use `public/` as the static host publish directory. Do not publish the project root, because `exports/` contains private WordPress migration backups.

## Migration notes

- WordPress content export: `exports/wavstorm.WordPress.2026-06-24.xml`
- WordPress media export: `exports/media-export-233802667-from-0-to-150.tar`
- Extracted local media: `assets/original-media/`

The domain currently points to WordPress.com. Deploy this folder to a static host first, then update GoDaddy DNS only after the hosted preview is verified.
