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

## THOTH 1.2.0 source update

The `android-thoth-app/` directory now contains the source project for version 1.2.0. It adds an Ask THOTH button and a full-page THOTH chat screen backed by the live Clovis Star member session. Authentication, CSRF, membership entitlements, rate limits, notes, and payment upgrade rules remain server-controlled at `https://clovisstar.com`.

GitHub Actions builds a debug APK for functional testing. A production in-place upgrade requires the original release signing key, which is not stored in this repository.
