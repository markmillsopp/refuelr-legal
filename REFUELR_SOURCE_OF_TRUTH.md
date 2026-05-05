# Refuelr — Source of Truth

Purpose
- The repository `Personal/refuelr` (local path: `/Users/n1603120/Personal/refuelr`) is the single source of truth for the Refuelr app. This repository (`refuelr-legal`) exists only to present the app and host legal/static pages (index and privacy).

Scope
- Use the app repo for authoritative app content: name, description, screenshots, assets, release notes, manifests (package.json, pyproject.toml), and other app metadata.
- Use this repo only for the public website and legal pages: `index.html` and `privacy.html`.

Guidelines for contributors and automated agents
- Always read app information from the app repo first before editing or publishing content here.
- Do NOT update app metadata in this repo — update it in the source repo and propagate changes.
- When asked for app details, consult the app repo files (README, manifest files, docs) first.
- If the app repo is inaccessible, do not guess. Report "source-of-truth unavailable" and ask for access or the correct content.

Paths / Examples
- App repo (authoritative): `/Users/n1603120/Personal/refuelr`
- This repo public pages: `index.html`, `privacy.html`

Agent instructions (automated use)
- Agents should fetch app-specific text from `/Users/n1603120/Personal/refuelr` (or the configured canonical repo) before using or reproducing app copy.
- Use this repo only to serve the site pages that reference the app; prefer original text from the app repo for accuracy.

Verification
- To verify app details, open the app repo's `README.md` or the app manifest (e.g., `package.json`) in `/Users/n1603120/Personal/refuelr`.

Notes
- Replace owner/maintainer contact details here if desired.
- If you want this file copied into another location or converted to a different name, tell me where and I will add it.
