# SnoreCatcher Official Website

Official landing page, interactive multi-modal acoustic lab, privacy policy, and terms of use for **SnoreCatcher (Snore Detector: Sleep Recorder)** on iOS & iPadOS.

- **Production Domain**: https://snorecatcher.netlify.app
- **App Store**: https://apps.apple.com/app/id6757622696
- **Synchronized App Version**: `v1.0.8 (Build 10)` · iOS 17.0+

## Architecture

```text
SnoreCatcherWebsite/
├── index.html       # Bilingual (EN / 中文) landing page & interactive acoustic/vitals simulator
├── index.css        # Deep Nocturnal Slate design system & responsive tokens
├── privacy.html     # Bilingual Privacy Policy (Sandbox, HealthKit 5.1.1(v), GDPR/ATT, AdMob)
├── terms.html       # Bilingual Terms of Use (Guideline 1.4.1 Medical Disclaimer & StoreKit 2 PRO)
├── app-ads.txt      # Authorized Digital Sellers verification for Google AdMob
├── netlify.toml     # Clean URL rewrites (/privacy, /terms) & security headers
└── assets/          # Official 1024x1024 AppIcon & localized EN/ZH native app screens
```

## Local Preview

```bash
python3 -m http.server 8000
```
