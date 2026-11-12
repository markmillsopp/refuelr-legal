# Plan: Android ads
Spec: ../../specs/android-ads.md

## Approach
Review contract; inspect/create dedicated Android AdMob configuration; extend platform config and preserve UMP; test Android and iOS contracts; revise release validation/legal copy; rebuild and replace internal draft artifact.

## Order
1. Fresh spec review.
2. Configure platform IDs and privacy messages.
3. Implement guarded Android banners and tests.
4. Independent code review, emulator verification, signed build and Play upload.

## Risks
Consent or AdMob readiness can block serving. Missing production IDs must block release. Preserve iOS. No paid infrastructure or advertising spend. Legal declarations and trader/public contact requirements can require user action.
