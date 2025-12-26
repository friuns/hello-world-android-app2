# Test App

A minimal Android application created as a test app.

## Description

This is a simple "Hello World" Android application built with:
- Android SDK 34 (target)
- Minimum SDK 21
- Java 8
- AndroidX libraries
- Gradle build system

## Features

- Simple MainActivity with a TextView
- Material Design theme
- ConstraintLayout for responsive UI

## Building

The app can be built using Gradle:

```bash
./gradlew assembleDebug
```

The debug APK will be generated at: `app/build/outputs/apk/debug/app-debug.apk`

## Deployment

This repository is configured with GitHub Actions workflows that automatically:
- Detect the Android project type
- Build the debug APK on every push
- Create GitHub releases with the APK attached
- Post deployment information to pull requests

See `.github/workflows/deploy.yml` for the complete deployment configuration.

## App Structure

```
app/
├── build.gradle              # App-level Gradle configuration
├── proguard-rules.pro        # ProGuard rules
└── src/main/
    ├── AndroidManifest.xml   # App manifest
    ├── java/com/example/testapp/
    │   └── MainActivity.java # Main activity
    └── res/
        ├── layout/
        │   └── activity_main.xml  # Main layout
        └── values/
            └── strings.xml   # String resources
```

## License

This is a test application.
