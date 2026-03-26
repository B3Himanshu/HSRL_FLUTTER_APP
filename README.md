# HSRL Dashboard

A Flutter WebView app that wraps the HSRL Business Performance Dashboard.

## About

This app loads the HSRL dashboard website inside a native Android/iOS WebView, providing a mobile app experience for the Business Performance Dashboard (Quick Insights, Fuel, Shop, Coffee & Valet, ROI).

## Configuration

The app reads configuration from the `.env` file in the project root:

```
BASE_URL=http://103.72.170.138:9000
APP_NAME=HSRL Dashboard
```

## Features

- WebView wrapper for the HSRL dashboard
- Loading spinner while page loads
- Error screen with Retry button if server is unreachable
- Portrait and landscape orientation support
- HTTP traffic allowed for internal server

## Setup

### Prerequisites
- Flutter SDK
- Android Studio or VS Code
- Android device or emulator

### Run

```powershell
flutter pub get
flutter run -d <device-id>
```

### Build Android APK

```powershell
flutter build apk --release
```

APK output: `build/app/outputs/flutter-apk/app-release.apk`

### Build iOS (requires Mac)

```bash
flutter build ipa
```

## Dependencies

- `webview_flutter: ^4.4.2` — WebView widget
- `flutter_dotenv: ^5.1.0` — Load config from `.env`

## Device

Tested on: CPH2487 (Android 16, API 36)
