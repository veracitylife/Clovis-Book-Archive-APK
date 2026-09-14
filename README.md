# Clovis Book Archive APK

This repository contains the complete Clovis Star Library Android app, including the book archive experience and the THOTH member chat entry point.

## Downloadable builds

- Legacy release: `clovis-star-library-1.1.0.apk` (version 1.1.0, version code 5)
- THOTH update: `clovis-star-library-1.2.0-thoth-debug.apk` (version 1.2.0, version code 6, debug build)

The 1.2.0 build preserves package ID `com.clovisstar.library` and adds a native Ask THOTH button that opens the full-page member chat at `https://clovisstar.com/members/thoth/`.

The 1.2.0 debug APK is built by GitHub Actions and is intended for functional testing. The original Android release signing key is not stored in this repository, so a release-signed build with that key is required for an in-place upgrade over an existing 1.1.0 installation.

## App behavior

The app uses the live Clovis Star website for the complete experience:

- book-library browsing and reading;
- member registration, login, password reset, and logout;
- THOTH chat;
- member dashboard and saved notes;
- membership entitlements, question limits, and payment upgrades.

The server remains authoritative for authentication, CSRF/session validation, membership permissions, rate limits, and THOTH logic. The Android WebView shares its session cookies between the library and THOTH pages.

The legacy library feed is `https://clovisstar.com/api/library.php`.

## Source and build

The Android source is in `android-thoth-app/`. Build locally with:

```bash
./gradlew assembleDebug
```

The GitHub Actions workflow is at `.github/workflows/build-apk.yml` and publishes a downloadable debug artifact for each source update.

## Repository scope

This repository does not contain signing keys, database credentials, API keys, raw environment files, or other private production configuration.

## License

All rights reserved. No source or binary redistribution rights are granted except by the repository owner.
