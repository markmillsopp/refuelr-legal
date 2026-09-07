# Refuelr website and shared legal pages

This repository hosts Refuelr's production website and the public privacy policies and terms for Refuelr, Team Master, and Trip Wire on [refuelr.co.uk](https://refuelr.co.uk/).

The domain is reused because the owner already owns it. Each app remains a separate product with its own legal pages; Refuelr's privacy policy and terms do not automatically cover Team Master or Trip Wire.

## Pages and status

| App | Location | Existing pages | Still to add |
| --- | --- | --- | --- |
| Refuelr | Repository root | [Website](index.html), [privacy](privacy.html), [terms](terms.html), [account deletion](delete-account.html) | — |
| Team Master | `team-master/` | [Privacy](team-master/privacy.html), [support](team-master/support.html) | Terms |
| Trip Wire | `trip-wire/` (planned) | None yet | Privacy and terms |

Team Master terms should use `team-master/terms.html`. Trip Wire privacy and terms should use `trip-wire/privacy.html` and `trip-wire/terms.html`. These paths are reserved conventions, not existing pages or confirmed live URLs.

## Updating content

- Follow [AGENTS.md](AGENTS.md) and [source-of-truth guidance](REFUELR_SOURCE_OF_TRUTH.md).
- Verify legal claims against the relevant app's source. Keep policies, terms, and in-app legal links specific to that app.
- Make production legal-page changes here. Refuelr's app repository `docs/` directory is not the production legal website.
- Preserve the dark-green design and mobile layout. Check local links and update `sitemap.xml` when adding public pages.

## Refuelr app downloads

- [App Store](https://apps.apple.com/gb/app/refuelr-fuel-prices-uk-ire/id6765485193)
- [Google Play](https://play.google.com/store/apps/details?id=com.refuelr.refuelr&pcampaignid=web_share)
