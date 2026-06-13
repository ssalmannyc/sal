# website

Website source, assets, and related files.

## What belongs here

- Website source code and configuration
- Web-optimized images and assets
- Content and copy for the site

## What does not belong here

- Heavy raw media (optimize for web first; keep originals in `media/`)
- `node_modules/`, build output, and caches (ignored by `.gitignore`)
- Curated showcase originals (use `portfolio/`)

## Safety notes

- No secrets, API keys, tokens, or `.env` files. Use environment variables in
  your host or local environment, never committed.
- No private client data.
- Large approved media must use Git LFS (see `.gitattributes`).
