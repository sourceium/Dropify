<div align="center">

#  Dropify = 💧 + ❄️ + 🔥

**Share Any File in Seconds. No Internet. No Cloud. No Limits.**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Platform: Android](https://img.shields.io/badge/Platform-Android_7.0+-3DDC84.svg?style=for-the-badge&logo=android&logoColor=white)](https://www.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-Jetpack_Compose-7F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Website](https://img.shields.io/badge/Website-dropifyin.vercel.app-4d43fe.svg?style=for-the-badge&logo=vercel&logoColor=white)](https://dropifyin.vercel.app)
[![GitHub Stars](https://img.shields.io/github/stars/sourceium/Dropify?style=for-the-badge&color=gold)](https://github.com/sourceium/Dropify/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/sourceium/Dropify?style=for-the-badge&color=silver)](https://github.com/sourceium/Dropify/network/members)

<br/>

[**🌐 Official Website**](https://dropifyin.vercel.app) &nbsp;•&nbsp; 
[**📥 Download APK (v1.0)**](https://drive.google.com/file/d/10lRTHGoRYlXTBd6fzdGQgTZ3vCPfBOSq/view?usp=drivesdk) &nbsp;•&nbsp; 
[**📦 Download AAB Bundle**](https://drive.google.com/file/d/1ZU1VCtShwjNWYQk03rsJ9hUk7IJvqRS0/view?usp=drivesdk) &nbsp;•&nbsp; 
[**📜 Privacy Policy**](https://dropifyin.vercel.app/privacy_policy/index.html)

</div>

---

## 📖 Overview

**Dropify** (`com.HaldarAi.Dropify`) is an open-source, ultra-fast peer-to-peer (P2P) nearby file sharing application for Android. Built with 100% Kotlin and Jetpack Compose, Dropify allows you to send gigabytes of 4K videos, full music libraries, APK packages, documents, and folders directly between nearby physical devices at speeds up to **50 MB/s** — **200x faster than standard Bluetooth**.

### 🌟 Key Core Principles
- **100% Offline**: Operates anywhere — on airplanes, subways, or remote locations without cellular data or Wi-Fi internet.
- **Zero-Cloud Architecture**: Files travel exclusively over direct peer-to-peer Wi-Fi Direct and Bluetooth. No files or personal data ever touch any server or cloud database.
- **Zero Ads & Zero Trackers**: No advertising SDKs, no behavioral telemetry, and no account or phone number registration required.
- **Lossless Quality**: No compression or resizing. Files arrive in their exact original byte format.

---

## 🚀 Download & Installation

| Package | Format | Description | Direct Link |
| :--- | :---: | :--- | :--- |
| **Dropify APK** | `.apk` | Standard installer for Android devices (v1.0) | [**Download APK (Google Drive)**](https://drive.google.com/file/d/10lRTHGoRYlXTBd6fzdGQgTZ3vCPfBOSq/view?usp=drivesdk) |
| **Dropify Bundle** | `.aab` | Google Play publishing package & developer bundle | [**Download AAB (Google Drive)**](https://drive.google.com/file/d/1ZU1VCtShwjNWYQk03rsJ9hUk7IJvqRS0/view?usp=drivesdk) |

### 📲 How to Install the APK on Android
1. Download the `.apk` file from the link above.
2. Tap the downloaded file in your browser or **Downloads** folder.
3. If prompted by Android, enable **"Install unknown apps"** for your browser.
4. Tap **Install**, then open Dropify and start sharing!

---

## ✨ Features

- ⚡ **Gigabit Wi-Fi Direct Transfers**: Direct peer-to-peer wireless speeds up to 50 MB/s.
- 📱 **Instant QR Code Pairing**: Scan recipient QR code using Google ML Kit to pair in under 1 second without manual Bluetooth pairing delays.
- 📁 **Universal File Format Support**: Photos, 4K HDR Videos, Audio, Installed APKs, ZIP archives, Documents, and Folders.
- 🔋 **Background Transfer Service**: Active foreground service (`FOREGROUND_SERVICE_DATA_SYNC`) keeps transfers running smoothly even when the app is minimized or screen is locked.
- 📊 **Real-Time Speed & ETA Monitor**: Shows live transfer speed (MB/s), elapsed percentage, and estimated time remaining.
- 🛡️ **Explicit Recipient Confirmation**: Receivers always review incoming sender information and tap "Accept" before any payload is transferred.
- 🗄️ **Local SQLite Transfer History**: Room database stores a clean history log of past transfers on-device, with one-tap history clearing.
- 🎨 **Modern Material 3 Design**: Clean responsive interface with dark/light theme support, custom animated avatar selection, and haptic feedback.

---

## 📊 Speed & Feature Comparison

| Feature | ⚡ Dropify (Nearby P2P) | Standard Bluetooth | Cloud / WhatsApp | Quick Share |
| :--- | :---: | :---: | :---: | :---: |
| **Max Transfer Speed** | **Up to 50 MB/s** | ~1 – 2 MB/s | Dependent on ISP upload | ~30 – 50 MB/s |
| **Internet Required** | ❌ **No (100% Offline)** | ❌ No | ✅ Yes (Burns mobile data) | ❌ No |
| **File Size Limit** | ♾️ **Unlimited** | Infeasible for &gt;100 MB | Capped (16MB / 2GB) | ♾️ Unlimited |
| **Original Quality** | ✅ **100% Lossless** | ✅ Lossless | ❌ Heavy compression | ✅ Lossless |
| **Cloud Storage** | ❌ **Zero Server Storage** | ❌ No | ❌ Uploaded to remote servers | ❌ No |
| **Account Required** | ❌ **None** | ❌ None | ✅ Phone number / Account | Google Account |
| **Open Source** | ✅ **Yes (MIT)** | N/A | ❌ Proprietary | ❌ Closed Source |

---

## 🛠️ Tech Stack & Architecture

- **Language**: Kotlin 2.0+
- **UI Toolkit**: Jetpack Compose with Material Design 3 (M3)
- **Architecture**: MVVM (Model-View-ViewModel) + Clean Architecture repository pattern
- **P2P Transport**: Google Play Services Nearby Connections API (`Strategy.P2P_STAR`)
- **QR Scanning**: Google ML Kit Barcode Scanning + ZXing Core
- **Local Persistence**: Android Room SQLite Database (v2 with automated migrations)
- **Key-Value Store**: Jetpack DataStore Preferences
- **Asynchronous Flow**: Kotlin Coroutines & Reactive `StateFlow`
- **Image & Icon Rendering**: Coil Compose & Vector Drawables
- **Min SDK**: API 24 (Android 7.0 Nougat)
- **Target SDK**: API 36 (Android 15+)

---

## 🔐 Permissions & Privacy Justification

Dropify adheres to the Android Least-Privilege security model:

| Permission | Minimum API | Purpose |
| :--- | :---: | :--- |
| `NEARBY_WIFI_DEVICES` | API 33+ | Discover and connect to nearby Wi-Fi Direct devices without requesting location (`neverForLocation`). |
| `BLUETOOTH_ADVERTISE`, `CONNECT`, `SCAN` | API 31+ | Fast device discovery and local cryptographic handshake (`neverForLocation`). |
| `ACCESS_FINE_LOCATION` | Legacy (API &le;30) | Required by legacy Android OS versions for Wi-Fi and Bluetooth hardware scanning. **Location is never tracked, stored, or uploaded.** |
| `FOREGROUND_SERVICE_DATA_SYNC` | API 29+ | Prevents the Android system from killing active large file transfers when screen is turned off. |
| `POST_NOTIFICATIONS` | API 33+ | Displays live transfer progress and incoming connection prompts. |
| `CAMERA` | All | Scans recipient pairing QR code via on-device ML Kit. Frames are never recorded or uploaded. |
| `Zero Broad Storage Permissions` | API 33+ | Uses Android Photo Picker and Storage Access Framework. Dropify **never** requests unrestricted file system access. |

Full privacy policy available at: [https://dropifyin.vercel.app/privacy_policy/index.html](https://dropifyin.vercel.app/privacy_policy/index.html).

---

## 🏗️ Building from Source

### Prerequisites
- Android Studio Ladybug (2024.2+) or newer
- JDK 17 or JDK 21
- Android SDK 36

### Build Steps
```bash
# 1. Clone the repository
git clone https://github.com/sourceium/Dropify.git
cd Dropify

# 2. Assemble Debug APK
gradle assembleDebug

# 3. Assemble Release APK
gradle assembleRelease

# 4. Run local unit & Robolectric tests
gradle :app:testDebugUnitTest
```

---

## 🌐 Official Web Portal

Dropify's web portal and SEO landing page is hosted on Vercel:
- **Landing Page**: [https://dropifyin.vercel.app/](https://dropifyin.vercel.app/)
- **Privacy Policy**: [https://dropifyin.vercel.app/privacy_policy/index.html](https://dropifyin.vercel.app/privacy_policy/index.html)
- **Sitemap**: [https://dropifyin.vercel.app/sitemap.xml](https://dropifyin.vercel.app/sitemap.xml)

---

## 👤 Developer & Grievance Officer

Developed and maintained with ❤️ by:

- **Author**: Subhojit Haldar
- **GitHub**: [@sourceium](https://github.com/sourceium)
- **Email**: [business.tizongaming@gmail.com](mailto:business.tizongaming@gmail.com)
- **Phone**: +91 8637856826
- **Location**: West Bengal, India

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for complete details.

```
MIT License

Copyright (c) 2026 Subhojit Haldar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```
