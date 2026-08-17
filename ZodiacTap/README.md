# ZodiacTap

**Rebranded fork of Key Mapper** — customized with Zodiac / Mukuro (Date A Live) theme.

- App name: **ZodiacTap**
- Package / applicationId: `com.zodiactap.app`
- Theme: Gold / Yellow primary + Pink accents + Deep space purple (dark mode)
- Custom launcher icon from provided artwork

Original project: https://github.com/keymapperorg/KeyMapper

## How to build APK (GitHub Actions or local)

This is a standard Android Gradle project (Kotlin + Compose).

```bash
./gradlew assembleRelease
# or for FOSS CI style
./gradlew assembleCi
```

You can set up your own GitHub Actions workflow using the existing structure in .github/workflows.

## Changes made in this rebuild
1. Renamed display name to ZodiacTap (all strings)
2. applicationId changed to com.zodiactap.app
3. Material 3 theme colors completely recolored to gold/pink/purple (Mukuro Date A Live inspired)
4. All launcher icons (mdpi~xxxhdpi + adaptive + monochrome + web) replaced with the provided artwork
5. APK output name prefix changed to ZodiacTap-

Note: Internal Kotlin package names (io.github.sds100.keymapper.*) were left unchanged to avoid massive refactor. Only applicationId and UI branding were updated. This is standard and works fine for a private rebrand.
