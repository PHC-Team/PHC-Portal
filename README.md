# PHC-Portal

<div align="center">

### A modern Steam depot & manifest management application

> **⚠️ Prototype Notice**
> PHC-Portal is currently in active development. Some features, including the manifest generator and several integrated tools, are still a work in progress.

[**⬇ Download Latest Release**](https://github.com/PHC-Team/PHC-Portal/releases/latest)

</div>

---

# Features

## 📦 Manifest Library

Manage and download Steam manifests from a large online database.

* Browse **100,000+** game manifests
* Search by **Game ID** or **Name**
* Language and depot selection
* One-click downloads
* Automatic installation
* Download history with statistics
* Live progress, speed, and ETA

---

## 🎮 Game Preparation (Goldberg Integration)

Automatically prepare downloaded games for offline use.

* Automatic Goldberg Steam Emulator setup
* SteamStub DRM unpacking (7 supported variants)
* Unsupported DRM detection (including Denuvo)
* Automatic emulator configuration generation
* Achievement, DLC, stats, and cloud-save configuration
* Automatic launch executable detection
* ColdClient loader support

---

## 📚 Library Management

Organize your downloaded games and Lua scripts.

* Unified Steam & Lua library
* List and Grid view modes
* Fast SQLite image caching
* Search and sorting
* Batch auto-update management
* Export all Lua files as ZIP

---

## ☁️ Cloud Saves

Powered by CloudRedirect.

* Dropbox support
* OneDrive support
* Google Drive support
* Cloud save dashboard
* Pin games across devices
* Remove orphaned backups

---

## 🛠 Integrated Tools

PHC-Portal includes several built-in utilities.

* DepotDownloader
* DepotDumper
* Config.vdf Extractor
* Goldberg Token Generator

Features include:

* Steam CDN downloads
* Depot information extraction
* 2FA QR code support
* Depot key extraction
* Automatic achievement, DLC, language, and depot metadata retrieval

---

## 🎨 Customization

Personalize the application.

### Themes

* Dark
* Steam
* Light
* Cherry
* Sunset
* Forest
* Grape
* Cyberpunk
* Pink
* Pastel
* Rainbow

Additional customization includes:

* Full custom theme editor
* Gradient editor
* Sidebar & background images
* Live preview
* Theme import/export
* UI scaling (70%–150%)
* High-DPI support

---

## ⚡ Quality of Life

* Automatic updates
* Native Windows notifications
* Minimize to system tray
* Single-instance protection
* Responsive interface
* Settings backup & restore

---

# 🚀 Project Roadmap

Want to see what changed in the latest release?

Check out **[CHANGELOG](CHANGELOG.md)** to see what changed or got improved.

Want to see what's planned for future releases?

Check out **[COMING-SOON](COMING-SOON.md)** to see upcoming features, improvements, and ongoing development plans.

---

# Installation

## Requirements

* Windows 10 or Windows 11
* .NET is **not required** (self-contained executable)
* Approximately 150 MB of free disk space
* Internet connection

## Quick Start

1. Download the latest release.
2. Run **PHC-Portal.exe**.
3. Enjoy.

No installation is required.

---

# First Launch

PHC-Portal will automatically:

* Detect your Steam installation
* Create its configuration folder
* Create the local SQLite cache database

Configuration is stored in:

```text
%AppData%\PHC-Portal
```

---

# Configuration

| Category      | Description                               |
| ------------- | ----------------------------------------- |
| Downloads     | Output folder, auto-install, ZIP cleanup  |
| Display       | Themes, UI scale, layout, window settings |
| Notifications | Toasts and popup settings                 |
| Updates       | Disabled, Check Only, Auto Update         |
| Cloud         | Provider configuration and pinned games   |
| Keys          | Community depot key uploads               |
| Mode          | SteamTools or DepotDownloader             |

---

# Built With

* .NET 8
* WPF
* SteamKit2
* SQLite
* protobuf-net
* CommunityToolkit.Mvvm
* Windows Toast Notifications

---

# Credits

## PHC-Team

PHC-Portal is developed and maintained by **PHC-Team**.

### Included Projects

* DepotDownloader — SteamRE
* DepotDumper — NicknineTheEagle
* Steamless — atom0s
* Goldberg Steam Emulator — Mr_Goldberg
* CloudRedirect — Selectively11 *(Patcher integration coming soon)*

---

<div align="center">

### Community

[GitHub](https://github.com/PHC-Team/) • [Discord](https://discord.gg/RNNg5TS7h5)

</div>
