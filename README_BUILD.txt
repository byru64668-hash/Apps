SchoolTrack Android Project — built from the current SchoolTrack web files

This project packages the current SchoolTrack HTML/CSS/JavaScript app inside a native Android WebView.

Included current app files:
- index.html
- style.css
- app.js
- manifest.json
- service-worker.js
- README.txt

Android wrapper:
- Package: com.schooltrack.inventory
- App name: SchoolTrack
- Version: 1.0 (versionCode 1)
- minSdk: 24
- targetSdk / compileSdk: 37
- Android Gradle Plugin: 9.4.0
- Gradle: 9.6.0
- AndroidX WebKit: 1.17.1

Security-oriented choices:
- The SchoolTrack web files are bundled into the APK rather than fetched from a website.
- No INTERNET permission is declared.
- WebView file access and content access are disabled.
- WebViewAssetLoader is used for local app content instead of file:// URLs.
- The app does not add a JavaScript-to-native bridge.
- The current app's data storage remains its existing browser localStorage storage.

Important:
- This folder is an Android source project, not an APK.
- A build environment with Android SDK + JDK 17 + Gradle 9.6 is required to produce the APK.
- The release APK should be signed before distribution.
