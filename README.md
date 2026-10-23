# HOPE FOUNDATION Android App (source project)

This project wraps the current HOPE FOUNDATION offline donation-register interface in a native Android WebView app.

## Included
- App label: HOPE FOUNDATION
- Two-page register flow
- Register list initially shows 10, with +10 more
- 100 register slots, each with 100 donor rows
- Donor Name and January–December amount columns
- Monthly totals
- Copy previous year / blank year
- Local browser storage and JSON backup/restore

## Important
This is the Android project source, not a compiled APK. A build environment must compile it before installing. Data is stored locally on the device and should be backed up regularly. This first APK version has no PIN lock or encryption.

## Build in Android Studio
1. Open this folder as a project.
2. Let Gradle sync.
3. Choose Build > Build Bundle(s) / APK(s) > Build APK(s).
4. The debug APK is generated at `app/build/outputs/apk/debug/app-debug.apk`.

## Build using GitHub Actions from a phone
1. Create a GitHub repository and upload the contents of this folder.
2. Open the repository's Actions tab.
3. Run the workflow named `Build HOPE FOUNDATION APK` (or push to `main`).
4. When it finishes, open the workflow run and download the `HOPE-FOUNDATION-APK` artifact.
5. Extract the downloaded artifact ZIP to get `app-debug.apk`, then open it on Android and allow installation from that source if Android asks.

The workflow uses a standard GitHub-hosted build runner; GitHub account access and internet are needed for this build step. The installed app itself works offline.
