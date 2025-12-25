# Hello World Android App

A simple "Hello World" Android application built with Java.

## 📱 Description

This is a minimal Android application that displays "Hello World!" text on the screen. The app demonstrates the basic structure of an Android project using Gradle build system.

## 🏗️ Project Structure

```
hello-world-android-app2/
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/com/example/helloworld/
│   │       │   └── MainActivity.java
│   │       ├── res/
│   │       │   ├── layout/
│   │       │   │   └── activity_main.xml
│   │       │   └── values/
│   │       │       └── strings.xml
│   │       └── AndroidManifest.xml
│   ├── build.gradle
│   └── proguard-rules.pro
├── gradle/
│   └── wrapper/
├── build.gradle
├── settings.gradle
├── gradle.properties
└── gradlew
```

## 🔧 Technical Details

- **Language**: Java
- **Min SDK**: 21 (Android 5.0 Lollipop)
- **Target SDK**: 34 (Android 14)
- **Compile SDK**: 34
- **Build System**: Gradle 8.2
- **Android Gradle Plugin**: 8.2.0

## 🚀 Building the App

### Prerequisites

- JDK 17 or higher
- Android SDK

### Build Commands

```bash
# Build debug APK
./gradlew assembleDebug

# Build release APK
./gradlew assembleRelease

# Clean build
./gradlew clean
```

The generated APK will be located at:
- Debug: `app/build/outputs/apk/debug/app-debug.apk`
- Release: `app/build/outputs/apk/release/app-release.apk`

## 📦 Deployment

The project includes automated deployment via GitHub Actions (`.github/workflows/deploy.yml`). When code is pushed to the repository:

1. The workflow automatically detects this as an Android project
2. Sets up Java 17 and Android SDK
3. Builds the debug APK
4. Creates a GitHub Release
5. Uploads the APK to the release

## 🎯 Features

- ✅ Simple MainActivity with TextView
- ✅ Material theme
- ✅ Responsive layout
- ✅ Ready for GitHub Actions deployment

## 📄 License

This is a sample project created for demonstration purposes.
