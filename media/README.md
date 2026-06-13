# media

Working media store, split into `finals/` and `raw/`.

## What belongs here

- `finals/` for finished, exported media ready to use or share
- `raw/` for source media, only when intentionally approved
- Media not yet curated into `portfolio/`

## What does not belong here

- Curated showcase selects (use `portfolio/`)
- Editing app caches and proxies (ignored by `.gitignore`)

## Safety notes

- No secrets, API keys, or credentials.
- No private client data unless explicitly approved.
- No raw media unless intentionally approved. Large approved media must use
  Git LFS (see `.gitattributes`). Watch GitHub LFS storage limits.
