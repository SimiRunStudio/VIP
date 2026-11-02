# Asmaron APK Build — Hindi Guide

## Is package mein kya update hua
- Aapke diye hue Asmaron Learn Languages logo ko square app artwork mein crop karke 1024×1024 PNG banaya gaya.
- Launcher icon, Android adaptive icon aur splash screen mein wahi branding set ki gayi.
- Expo config mein app display name `Asmaron Learn Languages`, version `19.0.2` aur Android versionCode `21` set hai.
- GitHub Actions workflow Android debug APK build karke artifact upload karta hai.

## GitHub se APK kaise nikalein
1. Is ZIP ko extract karein.
2. `asmaron_apk_ready` folder ke **andar ki saari files aur folders** repository ke root mein upload karein. `.github` hidden folder ko bhi upload karein.
3. GitHub → Actions → Build Asmaron Android APK → Run workflow.
4. Green tick aane par run kholein aur `Asmaron-Supreme-v19-debug-apk` artifact download karein.

## Zaroori sachchai
APK build pass hona packaging ko verify karta hai. Is current source mein kuch starter learning screens aur local demo interactions hain; planned har advanced feature, AI, cloud sync ya live service abhi implemented/connected hone ka daawa nahi hai. APK ko device par install karke alag se test karna hoga.
