# Agent Instructions

## Repository Purpose

- This repository hosts Refuelr's production website and public legal pages for Refuelr, Team Master, and Trip Wire.
- The apps share `refuelr.co.uk` because the owner already owns the domain and wants to reuse it. Shared hosting does not make them one product or give them a shared privacy policy or terms.
- Keep Refuelr's website and legal pages at the root. Update `privacy.html`, `terms.html`, and `delete-account.html` here.
- Keep Team Master pages under `team-master/` and Trip Wire pages under `trip-wire/`. Each app's privacy policy and terms belong in its own directory.
- See `README.md` for existing pages and pages still to be added. Do not claim that missing pages are live or link to them.

## App Sources and Legal Copy

- Verify each app's data practices and functionality against that app's source before changing its legal copy. Do not copy claims between apps.
- Refuelr's app source of truth is `/Users/markmillsopp/Projects/refuelr`.
- Do not update `/Users/markmillsopp/Projects/refuelr/docs/` for production legal changes.
- Keep Refuelr's in-app legal text under `/Users/markmillsopp/Projects/refuelr/lib/` aligned when changing Refuelr legal copy.
- Team Master and Trip Wire source locations are not yet documented here. Confirm the correct source before making app-specific legal claims, and record verified locations in `REFUELR_SOURCE_OF_TRUTH.md`.
- Keep each app's in-app legal text and links aligned with its own published pages.

## Change Rules

- Keep the existing dark-green design.
- Preserve mobile responsiveness.
- Clearly identify the app covered by each legal page.
- Check local links after edits. Use app-specific canonical URLs and update `sitemap.xml` when adding public pages.
- Never print or commit secrets.
