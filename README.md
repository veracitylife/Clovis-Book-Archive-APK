# Clovis Book Archive APK

This repository contains the ready-to-install Android APK for the Clovis Star Library / Book Archive app.

## APK

- File: `clovis-star-library-1.1.0.apk`
- Package: `com.clovisstar.library`
- Version: `1.1.0`
- Version code: `5`
- Min SDK: `23`
- Target SDK: `36`
- Size: `94,365` bytes
- SHA-256: `7F5FE78D6414758D3E7E1A51C4B9963424877A8E52F3BA5125D8A7607627E24B`

## App Details

The app provides a modern mobile interface for searching and reading the Clovis Star library archive. It uses the live archive feed at:

`https://clovisstar.com/api/library.php`

The app also includes mobile menu links for:

- Royal Game of Ur: `https://royalgameofur.clovisstar.com/`
- Senterej: `https://senterej.clovisstar.com/`

## Repository Scope

This repository intentionally includes only the compiled APK, this README, and `.gitignore`. It does not include development source files, build folders, signing keys, database credentials, or other internal project files.

## License

All rights reserved. No source or binary redistribution rights are granted except by the repository owner.

## THOTH 1.2.0 update

The `android-thoth-app/` directory contains the Android source for version 1.2.0. It preserves the complete book-library experience and adds an Ask THOTH button that opens a full-page chat screen at `https://clovisstar.com/members/thoth/`. The live site remains authoritative for login, CSRF, membership entitlements, hourly/daily/monthly quotas, notes, and payment upgrades.

The root GitHub Actions workflow builds a debug APK. A production in-place upgrade requires the original Android release signing key, which is not stored in this repository.
