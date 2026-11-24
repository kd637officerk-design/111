# XI Media Deck Android

A GitHub-ready Android WebView wrapper for the standalone **XI Hyper-Realistic Media Deck** HTML experience.

## Build the APK on GitHub

1. Create a new GitHub repository.
2. Upload all files and folders from this project, including `.github`.
3. Push to the `main` branch.
4. Open **Actions** > **Build Android APK**.
5. Open the completed run and download the **XI-Media-Deck-APK** artifact.
6. Unzip the artifact to get `app-debug.apk`.

The workflow also supports **Run workflow** from the Actions page.

## Local build

Install Android SDK platform 35, Android build-tools 35.0.0, JDK 17, and Gradle 8.9, then run:

```bash
gradle assembleDebug
```

APK output:

```text
app/build/outputs/apk/debug/app-debug.apk
```

## Notes

- The original HTML is stored at `app/src/main/assets/index.html`.
- Internet permission is enabled because the page references online fonts and an external lyrics API.
- The generated APK is a debug build, suitable for direct testing and sharing. For store distribution, add a private signing configuration and build a release APK or Android App Bundle.
