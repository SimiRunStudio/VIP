# Asmaron Supreme v19.0.1 — Build status

This project package contains the React Native / Expo source and a GitHub Actions workflow that builds an installable Android debug APK.

## What is implemented in this source revision
- Working Learn, Practice, Explore and Profile navigation.
- Three local English lesson questions with answer feedback and lesson completion.
- Local word flashcards with reveal/hide and next-card controls.
- Session-level gem and lesson progress updates.
- Subject hub cards for Languages, Math, Music, Chess, DET preparation and Memory.
- Honest feature-state messaging: remote AI voice, WebRTC, cloud sync, payments, online multiplayer, Stockfish integration and speech analysis are not active without their backend/native integrations.

## Build APK
The GitHub Actions workflow at `.github/workflows/build-apk.yml` runs Expo prebuild and Gradle `assembleDebug`, then uploads `app-debug.apk` as an artifact. Push this folder's contents (including `.github`) to the repository root, then open Actions and run **Build Asmaron Android APK**.

## Important scope and verification
The supplied feature matrix has 356 rows, but the supplied app source was a small starter screen. A feature specification is not an implementation. This revision improves the working local app flows but does not claim all 356 items are implemented. Remote services require credentials, backend endpoints and additional integration. A successful CI build and physical Android device test are still required before calling this release production-ready or bug-free.
