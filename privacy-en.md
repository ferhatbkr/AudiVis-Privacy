# Privacy Policy - AudiVis Player

**Last Updated:** December 27, 2024

## Overview

AudiVis Player respects your privacy and **does not collect, store, or share any personal data**.

## Data Collection

This application:
- ❌ Does not collect personal information
- ❌ Does not send usage statistics
- ❌ Does not use analytics services
- ❌ Does not display advertisements
- ❌ Does not require account creation

## Permissions and Usage

### 📁 Storage Permissions
**Permissions:**
- `READ_EXTERNAL_STORAGE`
- `READ_MEDIA_VIDEO`
- `MANAGE_EXTERNAL_STORAGE`

**Purpose:** Used to read video and subtitle files on your device.

**Data Sharing:** No. All files remain on your device.

### 🌐 Internet Access
**Permission:** `INTERNET`

**Purpose:** Used to access media files on remote servers via FTP and SMB protocols.

**Data Sharing:** No. The app does not send data to any servers.

**Note:** No analytics, advertising, or tracking services are used.

### 📶 Network State
**Permissions:**
- `ACCESS_WIFI_STATE`
- `ACCESS_NETWORK_STATE`

**Purpose:** Used to check if network connectivity is available.

**Data Sharing:** No.

### 🎵 Foreground Service
**Permissions:**
- `FOREGROUND_SERVICE`
- `FOREGROUND_SERVICE_MEDIA_PLAYBACK`
- `WAKE_LOCK`

**Purpose:** Used to continue video playback in the background and display notifications.

**Data Sharing:** No.

### 🔊 Text-to-Speech (TTS)
**Permission:** `TTS_SERVICE` (query)

**Purpose:** Uses your device's system TTS engine to read subtitles aloud.

**Data Sharing:** Data processed by the TTS engine is subject to your TTS provider's privacy policy (e.g., Google TTS, Samsung TTS).

## Data Security

### Local Storage
- All app data is stored locally on your device
- No data is uploaded to cloud servers

### Server Credentials
- FTP/SMB server credentials are stored encrypted using Android's `EncryptedSharedPreferences` API
- These credentials remain only on your device and are never shared

### Network Security
- The app only connects to FTP/SMB servers you configure
- No connections are made to third-party servers

## Third-Party Services

AudiVis Player **does not use any third-party services**:
- ❌ No Google Analytics
- ❌ No Firebase
- ❌ No ad networks
- ❌ No crash reporting services

**Exception:** Your device's system TTS engine (user-selected).

## Children's Privacy

This app does not knowingly collect data from children under 13. The app does not require any age verification and does not collect any user data.

## Changes

This privacy policy may be updated from time to time. Changes will be posted on this page.

## Contact

For privacy-related questions:
- **GitHub:** https://github.com/ferhatbkr/AudiVis-Privacy/issues

## Open Source

AudiVis Player is an open-source project:
- **License:** Apache License 2.0
- **Source Code:** https://github.com/ferhatbkr/audivis-player

---

**Summary:** AudiVis Player is a completely offline, privacy-respecting video player. Your data stays only on your device.
