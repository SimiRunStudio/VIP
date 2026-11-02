# Asmaron Supreme v19.0.1

Expo / React Native Android project.

## Local development
```bash
npm install
npx expo start
```

## Build installable Android debug APK
Push the complete project to GitHub (including `.github/workflows`) and run **Actions → Build Asmaron Android APK**. The workflow runs Expo prebuild, Gradle `assembleDebug`, and uploads the APK artifact.

For a cloud EAS preview build instead, configure EAS for this app and run `npm run apk:preview`.

See `BUILD_STATUS_HINDI.md` for implemented scope and limitations.
