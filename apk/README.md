# QLBX34 Android APK build

- APK-specific web asset: `android/app/src/main/assets/index.html`.
- The root `/index.html` used by GitHub Pages is intentionally untouched.
- The APK wrapper keeps the Android status bar visible.
- The native `AndroidFile` bridge saves PNG, XLSX and JSON exports to **Downloads/QLBX34** on Android 10+.
- The Android file picker supports restoring JSON and importing XLSX files.
- GitHub Actions builds a debug APK and publishes it as the artifact `QLBX34-Android-APK`.

To build manually from this directory: run Gradle 8.9 with JDK 17 and Android SDK 35, then `gradle -p android assembleDebug`.
