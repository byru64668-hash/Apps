SchoolTrack Android Project

This project wraps the current SchoolTrack HTML/CSS/JavaScript app in a native Android WebView.
The web app files are bundled inside the APK, so the core interface does not require internet access.
No INTERNET permission is requested by the Android manifest.

Build with Android Studio or another Android Gradle build environment.
Recommended: Build > Generate App Bundle(s) / APK(s) > Generate APK(s).

Note: The app's existing service worker is retained in assets, but the Android wrapper loads the bundled files directly. LocalStorage remains the app's data store.
