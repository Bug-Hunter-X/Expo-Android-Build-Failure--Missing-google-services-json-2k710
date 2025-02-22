# Expo Android Build Failure: Missing google-services.json

This repository demonstrates a common error encountered when building Android APKs using the Expo CLI. The error is caused by a missing `google-services.json` file, which is required by the Google Services Plugin for integrating Firebase or other Google services.

## Problem

The Expo build process fails with the following error:

```
FAILURE: Build failed with an exception.
* What went wrong: 
Execution failed for task ':app:processDebugGoogleServices'.
> File google-services.json is missing. The Google Services Plugin cannot function without it.
```

## Solution

The solution involves ensuring that the `google-services.json` file is correctly placed within the Android project directory.

1.  **Download `google-services.json`:**  Go to your Firebase project settings and download the `google-services.json` file.
2.  **Place the file:** Place the downloaded `google-services.json` file inside the `android/app/` directory of your Expo project.
3.  **Rebuild:** Try building your Android APK again using the Expo CLI.