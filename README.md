# Melody — Offline Android Music Player

A lightweight Kotlin Android project. It scans music already stored on the phone, searches by title/artist, and plays tracks locally. It does not stream or bundle copyrighted music.

## Build on Windows
1. Install Android Studio (or Android SDK + JDK 17).
2. Extract this ZIP.
3. In Android Studio choose **Open** and select the `MelodyAndroid` folder.
4. Let Gradle sync. If prompted, install Android SDK Platform 35 and Build Tools.
5. Choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. The APK will be at `app/build/outputs/apk/debug/app-debug.apk`.
7. Transfer it to your Android phone, open it, and allow audio access.

## Notes
- Minimum Android: 6.0 (API 23).
- This starter version plays local audio files indexed by Android MediaStore.
- No account, internet connection, ads, or streaming required.


## Build the APK in the cloud (no Android Studio needed)
This project includes a GitHub Actions workflow at `.github/workflows/android.yml`.

1. Create a free repository on GitHub.
2. Upload the **contents** of this project folder to the repository (keep the `.github/workflows/android.yml` file and its folders).
3. Open the repository's **Actions** tab and select **Build Melody APK**.
4. If it has not run automatically, choose **Run workflow**.
5. When the run finishes successfully, open that run and download the **Melody-debug-apk** artifact.
6. Extract the downloaded artifact ZIP; it contains `app-debug.apk`. Transfer it to your Android phone and install it.

GitHub account sign-in and the initial repository upload are required; the cloud workflow compiles the APK for you.
