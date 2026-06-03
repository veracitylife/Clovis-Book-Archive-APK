# Clovis Book Archive APK

This repository contains the release APK for the **Clovis Star Library** Android app.

## App

**Clovis Star Library** makes the Clovis Star Gnostic Library easier to browse on Android. The app provides a searchable catalog, collection filters, readable book summaries, share actions, and one-tap access to the live archive reader pages.

## Archive Source

The app uses the live Clovis Star library feed:

`https://clovisstar.com/api/library.php`

The feed currently exposes the static reader archive under:

`https://clovisstar.com/books/...`

The API is read-only, returns public catalog records, and does not expose database credentials. The app also includes a bundled fallback catalog so the library index remains usable if the live feed is temporarily unavailable.

## Release

- APK: `clovis-star-library-1.0.2.apk`
- Android package: `com.clovisstar.library`
- Version: `1.0.2`
- Version code: `3`
- Minimum Android SDK: `23`
- Target Android SDK: `36`
- SHA-256: `44F045256D001DB5B7FF52B98F4B232988C3090615336AEACB7477C9F1155834`
- Size: `95631` bytes

## Contents

This repository intentionally contains only:

- the release APK
- this README
- the `.gitignore` file that prevents development files from being added

No development files, source code, signing keys, database credentials, build folders, or workspace files are included.

## License

All rights reserved.

No permission is granted to copy, modify, redistribute, sublicense, sell, decompile, reverse engineer, or create derivative works from this APK or associated archive materials unless explicitly authorized in writing by the rights holder.
