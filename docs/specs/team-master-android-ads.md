# Android banner advertising

## Objective
Enable consent-gated Android banners in Team Master, as requested during Play release preparation. Account users target ages 13+, not under-13s; organisers may manage younger players.

## Scope and constraints
Reuse existing Google Mobile Ads dependency, banner placement and UMP consent/privacy options flow. Add platform-specific Android app/banner IDs from the user's AdMob account. Never reuse iOS IDs. Debug uses Android sample IDs; preview and disabled builds request no ads. Android must never invoke ATT; request non-personalised ads on Android while preserving existing iOS consent/ATT behaviour. No new cloud compute or paid service. AdMob is publisher advertising revenue, not an advertiser spending campaign. Do not create billing or buy ads. Update legal copy and Play ads/Data safety declarations to match behaviour. Public policy publication requires actual source comparison. Preserve unrelated work.

## Acceptance
- Android selects its own test/production banner; release refuses missing/test/mismatched app/banner IDs.
- Consent failure/timeout cannot trigger an initial Android ad request; privacy options remain available when UMP requires them.
- iOS positive regressions retained; Android verifies no ATT calls and correct platform IDs.
- Analysis, tests and Android test-ad emulator checks pass. Never interact with production ads during testing.
- Build next unused Play versionCode through npm run build:android after final changes, verify signature/package/version and upload to existing internal draft with corrected notes. AdMob approval/serving and physical/privacy acceptance are separate from upload.

## Boundaries
mobile-app/lib/core/ads, tests, Android manifest/build, release helper, legal copy and docs. Configure Android AdMob app/banner and privacy message in console; any legal agreement requires action-time confirmation. Target audience 13+; trader status user indicates trader, but formal declaration handled separately in Play.

## Decisions
```brain-decisions
{"feature":"android-ads","decisions":[{"id":"android-npa","title":"Consent-gated Android banners","decision":"Reuse UMP with Android-specific IDs and non-personalised requests, skipping iOS ATT on Android.","rationale":"Provide requested monetisation while preserving iOS behaviour and avoiding unsupported permission calls.","alternatives":["Reuse iOS identifiers: invalid platform configuration.","Request ads before consent: not acceptable."],"consequences":["Requires Android AdMob configuration and privacy-message publication; real serving depends on AdMob readiness."],"paths":["mobile-app/lib/core/ads","mobile-app/android/app/src/main/AndroidManifest.xml"],"supersedes":[]}]}
```

## Open gates
Android production app/banner IDs and privacy-message configuration are not yet verified. Legal/public policy needs Android coverage. Console form completion and required closed testing remain part of the overarching release task.

Legal repository scope: update only Team Master privacy scope, banner/UMP descriptions and device-neutral deletion instructions. Preserve Refuelr and Trip Wire. Main source is /Users/markmillsopp/Projects/team-master/mobile-app.
