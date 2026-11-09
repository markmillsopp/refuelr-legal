# Team Master notification privacy update

Date: 9 November 2026.
Scope: publish Team Master notification disclosures and verified app-source mapping. Other apps and the existing design remain unchanged.

## Independent accuracy review

Reviewer: `/root/review_public_privacy`, separate fresh-context agent.
Status: passed after correction and recheck.

Required finding resolved: registration data can be stored during signed-in refresh even while alerts are off. Public and in-app copy now distinguish registration from notification opt-in and delivery eligibility. Other reviewed disclosures match the implementation: generic payload, viewer email exclusion, conditional feature availability, sign-out limitations, retention and account erasure. This is source accuracy review, not legal-compliance certification.

Reviewed/applied policy SHA-256: `46c4bba0d3922d446df926659c34f528efae3ffe4012133c3ba9726df0d28efa`.

## Verification

- Applied page matches the independently reviewed hash.
- Local links/assets resolve; canonical URL remains app-specific.
- Whitespace checks pass. No new pages or sitemap entries are needed.
- Source mapping records the authoritative Team Master checkout and relevant implementation files.
- Live publication is verified separately after the main-branch push; publishing this copy does not enable notification delivery.
