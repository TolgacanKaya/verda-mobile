# 📱 VERDA MOBILE: AI-Powered Agricultural Assistant & XAI Field Scanner

[![Flutter](https://img.shields.io/badge/Flutter-3.x-02569B.svg?logo=flutter&logoColor=white)](https://flutter.dev/)
[![Dart](https://img.shields.io/badge/Dart-3.x-0175C2.svg?logo=dart&logoColor=white)](https://dart.dev/)
[![Android](https://img.shields.io/badge/Platform-Android%20%7C%20iOS-green.svg?logo=android&logoColor=white)](https://flutter.dev/)
[![XAI Enabled](https://img.shields.io/badge/XAI-Grad--CAM%20Visualizer-brightgreen.svg)](#-key-features)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

**VERDA MOBILE** is a cross-platform mobile application developed with **Flutter** and **Dart**. Designed for farmers, agronomists, and field workers, it provides real-time crop disease diagnosis by taking leaf photos, visualizing **Explainable AI (Grad-CAM)** heatmaps on-screen, providing **Text-to-Speech (TTS)** voice prescription guidance, and generating exportable PDF diagnostic reports.

---

## 🔗 Ecosystem Repositories

Verda Mobile connects directly to the Verda AI backend ecosystem:

| Component | Repository | Description |
| :--- | :--- | :--- |
| 🧠 **AI & ML Core** | [plant_disease_xai](https://github.com/TolgacanKaya/plant_disease_xai) | Deep learning model training, GrabCut segmentation, and XAI evaluation metrics. |
| 🌐 **Web Backend & API** | [verda-web](https://github.com/TolgacanKaya/verda-web) | Django REST API server, SQLite treatment database, and web administration portal. |
| 📱 **Mobile Application** | [verda-mobile](https://github.com/TolgacanKaya/verda-mobile) | Flutter mobile application for real-time camera scanning, XAI visualization, and TTS audio remedies. |

---

## 🌟 Key Features

* **📷 AI-Powered Camera Diagnosis**: Capture leaf images using the device camera or select from photo gallery, sending binary payloads to the Django REST API for deep neural network evaluation.
* **🔍 Explainable AI (XAI) Heatmap Overlay**: Displays Grad-CAM (Gradient-weighted Class Activation Mapping) visual overlays showing exact lesion locations responsible for the diagnosis.
* **🔊 Text-to-Speech (TTS) Prescription Reader**: Synthesizes dual organic (ecological) and chemical (fungicide) treatment advice into spoken audio for field convenience.
* **📄 PDF Diagnostic Certificate Exporter**: Generates exportable, printable PDF diagnostic certificates directly on-device.
* **🌿 Agronomy Encyclopedia & Pathology Library**: Browsable catalog containing crop pathology definitions, prevention strategies, and botanical metadata.
* **⚡ Guest Access & Quick Onboarding**: Instant guest evaluation mode allowing immediate app testing without requiring mandatory user login.
* **🎨 Modern Outdoor UI**: High-contrast Material Design 3 interface optimized for outdoor sunlight visibility and effortless one-handed field operation.

---

## 🛠️ Technology Stack & Dependencies

* **Framework**: Flutter SDK (Dart 3.x)
* **Image Handling**: `image_picker` (Camera & Gallery integration)
* **Networking**: `http` (RESTful API JSON communication)
* **Accessibility**: `flutter_tts` (Text-to-Speech engine)
* **Document Generation**: `pdf` & `printing` (On-device PDF creation)
* **UI & Typography**: `google_fonts`, `cupertino_icons`
* **Local Persistence**: `shared_preferences`, `path_provider`

---

## 📁 Repository Directory Structure

```
verda-mobile / mobile_app/
├── android/                 # Android native project files & manifest configuration
├── assets/                  # App logos, branding assets & icon graphics
├── ios/                     # iOS native project files & Runner settings
├── lib/                     # Dart application source code
│   ├── config/              # API URL endpoints & server IP settings
│   ├── models/              # Data models for diagnosis, pathology & prescriptions
│   ├── screens/             # UI screens (Home, Camera Scanner, Diagnosis, Encyclopedia)
│   ├── services/            # REST API service calls, TTS player & PDF generator
│   └── widgets/             # Reusable UI widgets, cards & animated components
├── pubspec.yaml             # Flutter dependencies & asset declarations
└── README.md                # Project documentation
```

---

## 🚀 Getting Started & Setup Instructions

### Prerequisites
* [Flutter SDK](https://docs.flutter.dev/get-started/install) (v3.10.3 or higher)
* Android Studio / VS Code with Flutter extension
* Android Emulator or physical Android/iOS device

### 1. Clone Repository

```bash
git clone https://github.com/TolgacanKaya/verda-mobile.git
cd verda-mobile
```

### 2. Fetch Dependencies

```bash
flutter pub get
```

### 3. Configure Backend Connection

To connect the mobile app to your local Django REST API server:
1. Open `lib/config/` (or `lib/config.dart`).
2. Update the API base URL with your local machine's IP address (or `10.0.2.2:8000` for Android Emulator):
   ```dart
   const String baseUrl = 'http://192.168.1.X:8000/api';
   ```

### 4. Run Application

```bash
# Run on connected device or active emulator
flutter run
```

---

## 📦 Pre-compiled Android APK

A pre-built, ready-to-test APK is available in the root of the main AI repository:
* Download [`Verda.apk`](https://github.com/TolgacanKaya/plant_disease_xai/raw/main/Verda.apk) to install directly on any Android device.

---

## 📜 License

This project is licensed under the MIT License — see the `LICENSE` file for details.
