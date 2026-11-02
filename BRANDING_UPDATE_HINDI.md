# Asmaron branding update

- `assets/branding.png` now uses the supplied polished Asmaron Learn Languages logo.
- `assets/app-icon.png` uses the same square high-resolution artwork for the launcher icon.
- `assets/splash-logo.png` uses the same artwork for the splash screen.
- All three image files are 1024 x 1024 PNG files.

## GitHub Actions build

The workflow is at `.github/workflows/build-apk.yml`. It runs Expo prebuild in CI mode and uploads the generated debug APK as the `Asmaron-Supreme-v19-debug-apk` artifact.

To build: open the repository's Actions tab, select `Build Asmaron Android APK`, and choose `Run workflow` on the `main` branch. Download the APK from the completed run's Artifacts section.

A successful cloud build is not guaranteed until GitHub Actions completes successfully. This source package has not itself been compiled into an APK in this environment.
