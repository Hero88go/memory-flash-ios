# Memory Flash iOS App — Info

## App Store Connect
- **App Name**: Memory Flash
- **Bundle ID**: `com.geekmagnetinc.memoryflash`
- **Apple ID**: TBD — fill after App Store Connect entry exists
- **SKU**: memory-flash-ios
- **Primary Language**: English (U.S.)
- **Platform**: iOS

## Apple Developer
- **Team ID**: L52G64VBAZ
- **Account Holder (Owner)**: Kristin Boster (kristin@kristinboster.com)
- **Developer (Chandler)**: hero88go@gmail.com — under Kristin's account
- **Company**: Geek Magnet Inc

## Codemagic
- **Project**: memory-flash-ios (TODO: create)
- **Repo**: github.com/Hero88go/memory-flash-ios (TODO: create)
- **Provisioning Profile name**: `memory-flash-profile`
- **Distribution Cert name**: `memory-flash-distribution`

## Local Setup (one-time, on this Windows box)
```
cd "c:/Users/Chandler/NEW project/memory-flash-ios"
npm install
npx cap add ios
npx cap sync ios
```

## Asset Pipeline
- Replace `assets/icon.png` with a 1024x1024 PNG branded for Memory Flash (currently a placeholder copied from tempo-ios)
- Then: `npx @capacitor/assets generate --ios`

## Web Source
- Source HTML: `c:/Users/Chandler/NEW project/memory-flash.html`
- iOS-shipped copy: `www/index.html` (viewport patched for safe-area-inset)
- When you update the source, copy back into `www/index.html` and re-apply the iOS viewport meta tags.

## App Store Description (draft)
**Subtitle**: Color grid memory game
**Description**:
A color grid flashes. Memorize. Recreate. The grid grows every level.
Test your visual memory and see how far you can go.

## Notes
- Pure local game — no backend, no Convex.
- No accounts, no analytics yet.
