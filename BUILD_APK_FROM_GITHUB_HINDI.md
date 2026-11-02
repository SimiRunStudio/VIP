# Asmaron v19 — GitHub se APK build karne ka tarika

## Zaroori sachchai
Yeh source project Expo/React Native starter UI hai. `docs/features_matrix.csv` mein 356 specification rows hain, lekin iska matlab yeh nahi ki 356 features source code mein implemented hain. Real AI voice, accounts, sync, multiplayer, payments, etc. ke liye actual services/backend aur implementation chahiye.

## GitHub Actions se installable debug APK
1. ZIP extract karein.
2. `asmaron_apk_ready` ke **andar ka poora content**, including hidden `.github` folder, apne GitHub repository ke `main` branch ke root mein upload karein. Root par `App.js`, `package.json`, `app.json` aur `.github/workflows/build-apk.yml` dikhna chahiye.
3. GitHub repository → **Actions** → **Build Asmaron Android APK** kholein.
4. **Run workflow** → branch `main` → **Run workflow**.
5. Run green hone par run details ke neeche **Artifacts** se `Asmaron-Supreme-v19-debug-apk` download karein.

Is workflow ko Expo/EAS token ki zaroorat nahi hai. GitHub-hosted runner Node, Java aur Android build tools install/use karta hai. Build fail ho to red run kholkar pehla error log share karein.

## Build scope
Workflow current source ko debug-signed, installable APK mein package karta hai. Yeh missing product features ko khud se implement nahi karta. Real device testing alag se zaroori hai.
