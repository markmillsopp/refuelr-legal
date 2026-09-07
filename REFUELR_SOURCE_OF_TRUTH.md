# App sources of truth and shared legal hosting

## Repository scope

`refuelr-legal` hosts Refuelr's production website and public legal pages for Refuelr, Team Master, and Trip Wire. The owner reuses the existing `refuelr.co.uk` domain for these separate apps. Shared hosting does not imply shared data practices, privacy policies, or terms.

Use this repository for public website and legal-page changes. Use each app's own source repository for authoritative functionality, data practices, app metadata, assets, and in-app content.

## App sources and page locations

| App | Authoritative app source | Public pages in this repository |
| --- | --- | --- |
| Refuelr | `/Users/markmillsopp/Projects/refuelr` | `index.html`, `privacy.html`, `terms.html`, `delete-account.html` |
| Team Master | Not yet documented; confirm before changing legal claims | `team-master/`; privacy and support exist, terms still to add |
| Trip Wire | Not yet documented; confirm before changing legal claims | `trip-wire/` planned; privacy and terms still to add |

See [README.md](README.md) for the current page inventory. Record Team Master and Trip Wire source locations here once verified; do not infer them from Refuelr's source.

## Contributor and agent guidance

- Read the relevant app's source before editing or publishing app-specific claims. Verify data collection, service providers, retention, deletion, and functionality against that app.
- Do not reuse another app's legal claims merely because its pages share the domain.
- Update app metadata in its source repository, then propagate relevant public website changes here.
- Do not edit `/Users/markmillsopp/Projects/refuelr/docs/` for production legal-page changes.
- Keep Refuelr's in-app legal text under `/Users/markmillsopp/Projects/refuelr/lib/` aligned with its public pages. Keep other apps' in-app legal text and links aligned in their respective sources.
- If the relevant source is unavailable, report that limitation and obtain the correct source or verified content before drafting app-specific claims.
- Keep each app's privacy policy and terms clearly labelled and use its own page paths. Do not link to planned pages until they exist.
