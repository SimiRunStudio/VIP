# Asmaron Learn Languages — Android APK

Clean Expo project package for GitHub Actions APK builds.

## Branding included
- App launcher icon: `assets/app-icon.png`
- Android adaptive icon foreground: `assets/branding.png`
- Native splash artwork: `assets/splash-logo.png`
- All three use the square logo artwork supplied by the project owner.

## Build APK on GitHub
1. Upload the **contents** of this folder to the root of the GitHub repository (keep the hidden `.github` folder).
2. Open **Actions** → **Build Asmaron Android APK** → **Run workflow**.
3. Wait for the workflow to finish with a green check.
4. Open the successful run and download the `Asmaron-Supreme-v19-debug-apk` artifact.

The workflow creates an Android debug APK at `android/app/build/outputs/apk/debug/app-debug.apk` and uploads it as an artifact.

## Local build
Run `npm install`, then `npm run apk:debug` on a machine with the Android build prerequisites.

## Scope note
This is the current Expo starter implementation with the supplied branding and APK workflow. A successful APK build confirms packaging, not that every planned product feature or cloud/AI service is implemented. Those require their own implementation and service credentials.
