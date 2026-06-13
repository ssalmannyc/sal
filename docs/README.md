# Repository Index

This is the documentation index for the **sal** repository, the proprietary
personal portfolio and Sal Media project owned by Sal.

For the project overview, start with the top-level [README](../README.md).
This index is the map: it explains what the repository is for, how it is
organized, the rules that govern it, and how to add new content safely.

## Purpose

This repository is the home base for Sal's professional creative work. It
organizes finished and in-progress media, brand assets, and client-facing
presentation material in one versioned place. Large media files are tracked
with Git LFS so the repository stays fast.

It holds: photography, videography, creative media, personal brand assets,
website material, presentations, and Sal Media related work.

## Top-level folder structure

| Folder | Purpose | Folder doc |
|--------|---------|-----------|
| `brand/` | Brand identity assets | [brand](../brand/README.md) |
| `brand/logos/` | Logo files and variations | [logos](../brand/logos/README.md) |
| `brand/guidelines/` | Brand standards and usage rules | [guidelines](../brand/guidelines/README.md) |
| `portfolio/` | Curated, finished showcase work | [portfolio](../portfolio/README.md) |
| `portfolio/photography/` | Final photography selects | [photography](../portfolio/photography/README.md) |
| `portfolio/videography/` | Final video work and reels | [videography](../portfolio/videography/README.md) |
| `portfolio/design/` | Final design pieces | [design](../portfolio/design/README.md) |
| `projects/` | Active and archived project work | [projects](../projects/README.md) |
| `projects/sal-media/` | Sal Media business work | [sal-media](../projects/sal-media/README.md) |
| `presentations/` | Decks and presentation material | [presentations](../presentations/README.md) |
| `social-content/` | Social media content | [social-content](../social-content/README.md) |
| `website/` | Website source and assets | [website](../website/README.md) |
| `media/` | Working media store | [media](../media/README.md) |
| `media/finals/` | Finished, exported media | [finals](../media/finals/README.md) |
| `media/raw/` | Source/raw media (approval needed) | [raw](../media/raw/README.md) |
| `docs/` | Documentation and this index | (this file) |
| `scripts/` | Utility scripts and automation | [scripts](../scripts/README.md) |

## Governance files

These define ownership, contribution rules, and how to report problems.

- [README.md](../README.md) - project overview and getting started
- [LICENSE](../LICENSE) - All Rights Reserved proprietary license
- [NOTICE](../NOTICE) - ownership and third-party materials notice
- [CONTRIBUTING.md](../CONTRIBUTING.md) - contribution rules (written approval required)
- [SECURITY.md](../SECURITY.md) - how to report security and exposure concerns

## Git LFS media rules

Large media files are stored with [Git LFS](https://git-lfs.com/). The tracked
types are defined in [.gitattributes](../.gitattributes):

- Design / layout: `.psd`, `.ai`, `.indd`
- Video / audio: `.mov`, `.mp4`, `.mxf`, `.wav`
- High-res images: `.tif`, `.tiff`
- Camera raw: `.cr2`, `.cr3`, `.nef`, `.arw`, `.dng`
- Archives / delivery: `.zip`, `.7z`

Run `git lfs install` once per machine before adding any of these. Confirm a
file is LFS-tracked (`git lfs status`) before committing it.

Note: GitHub free accounts include limited LFS storage and bandwidth. A large
video library can exceed the quota quickly. Plan storage before adding heavy
media. Official docs:
https://docs.github.com/en/repositories/working-with-files/managing-large-files

## Safety rules

These apply to every commit, everywhere in the repository.

- **No secrets.** Never commit API keys, passwords, tokens, credentials,
  private keys, or `.env` files. The [.gitignore](../.gitignore) helps, but
  you are responsible for checking each commit.
- **No private client data** unless explicitly approved for this repository.
  Confirm any model or client release before publishing media.
- **No raw media by default.** Only add raw camera files or source footage
  when their inclusion is intentionally approved, and always via Git LFS.
- **Written approval first.** Per [CONTRIBUTING.md](../CONTRIBUTING.md),
  approval is required before any pull request, commit, push, design change,
  media upload, or website change.
- **Report problems privately** to sal@salman.nyc per
  [SECURITY.md](../SECURITY.md). Do not open public issues for sensitive
  matters.

## Recommended workflow for adding new content

1. **Confirm approval.** Make sure the work is approved per CONTRIBUTING.md.
2. **Pick the right folder.** Use the structure table above. Read that
   folder's README to confirm what belongs there.
3. **Prepare the files.** Export finished media. Keep raw/source out unless
   approved. Optimize web assets.
4. **Check for secrets and private data.** Scan the files before staging.
   Remove anything sensitive.
5. **Handle large media with LFS.** If adding a tracked type, confirm
   `git lfs install` has been run and the file shows as LFS-tracked.
6. **Stage intentionally.** Add only the specific files you mean to commit
   (`git add <path>`), then review with `git status` and
   `git diff --cached --name-only`.
7. **Commit with a clear message.** Describe what changed and why.
8. **Push to `main`.** Use `git push origin main`. Never force push.
9. **Verify.** Confirm the change landed as expected on GitHub.

## Contact

For approval, questions, or to report a concern: sal@salman.nyc
