# Contributing

This is a proprietary personal portfolio and Sal Media repository. It is not
an open source project.

## Public contributions are not accepted

Public contributions are **not** accepted unless Sal gives prior written
approval. Pull requests, issues, or changes submitted without written
approval will not be reviewed, merged, or used.

If you wish to propose work, contact Sal directly and obtain written approval
before doing anything in this repository.

## Written approval is required first

Written approval from Sal is required **before** any of the following:

- Opening a pull request
- Making a commit
- Pushing to any branch
- Changing a design
- Uploading or replacing media
- Changing the website

Do not perform any of these actions on assumption. If it is not approved in
writing, do not do it.

## Rules for authorized work

If, and only if, you have written approval, your work must follow these rules.

### 1. Follow the repository structure

Place files in the correct existing folders (for example `brand`,
`portfolio`, `media`, `projects`, `presentations`, `website`, `docs`,
`scripts`). Do not invent new top-level folders or restructure the repository
without approval.

### 2. Protect confidential and private materials

Do not add client-private, personal, or confidential materials unless they
are explicitly approved for this repository. When in doubt, leave it out and
ask first.

### 3. Never commit secrets

Do not commit API keys, passwords, tokens, credentials, private keys, or
`.env` files. The `.gitignore` is set up to help prevent this, but you are
responsible for double-checking every commit. If a secret is ever committed,
report it to Sal immediately so it can be rotated.

### 4. Do not upload raw media unless approved

Do not commit raw camera files or large source footage unless that specific
upload has been approved. Prefer finished exports. Heavy raw libraries are
often better kept outside the repository.

### 5. Use Git LFS for approved large media

When approved large media is added, it must use Git LFS. The tracked types
are defined in `.gitattributes` (for example PSD, AI, INDD, MOV, MP4, MXF,
WAV, TIF, TIFF, CR2, CR3, NEF, ARW, DNG, ZIP, 7Z). Run `git lfs install`
once on your machine before adding any such files, and confirm they are
tracked by LFS before committing.

## Licensing

All materials in this repository are governed by the `LICENSE` and `NOTICE`
files. Nothing in this document grants any license or right to use the
materials.

## Contact

For approval or questions, contact Sal directly.
