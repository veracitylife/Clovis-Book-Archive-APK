# Clovis Star Library Android 1.2.0

This source project adds an `Ask THOTH` entry point and a full-page THOTH WebView to the existing `com.clovisstar.library` package.

The app deliberately uses the live Clovis Star member pages rather than copying authentication or entitlement logic into the APK. The shared WebView cookie jar preserves the signed-in session, while the server remains authoritative for:

- registration, login, password reset, and logout;
- CSRF/session validation;
- membership role and paid-plan entitlements;
- hourly, daily, and monthly THOTH limits;
- THOTH answers and member-note storage.

The THOTH screen loads `https://clovisstar.com/members/thoth/`, which presents login/register and membership options when the visitor is not authenticated.

## Build

```bash
./gradlew assembleDebug
```

The production package ID is preserved as `com.clovisstar.library`. Version `1.2.0` uses version code `6`.

This repository does not contain the original release signing key. A release APK signed with the original key is required for an in-place upgrade over the existing 1.1.0 installation; the debug build is for functional testing only.

