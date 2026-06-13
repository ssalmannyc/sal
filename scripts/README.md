# scripts

Utility scripts and automation for the repository.

## What belongs here

- Helper scripts (shell, PowerShell, Python, Node) for repo tasks
- Automation for media processing, exports, or housekeeping
- Documented, reviewed scripts only

## What does not belong here

- Untrusted or unreviewed third-party code
- Compiled output, caches, or dependencies (ignored by `.gitignore`)

## Safety notes

- No secrets, API keys, tokens, or passwords hardcoded in scripts. Read them
  from environment variables or local, ignored config files.
- No private client data.
- Review any script before running it. Do not execute unknown code.
