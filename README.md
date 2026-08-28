# Super Cleaner C

<div align="center">

```
   _____                      ________                              ______ 
  / ___/__  ______  ___  _____/ ____/ /__  ____ _____  ___  _____   / ____/ 
  \__ \/ / / / __ \/ _ \/ ___/ /   / / _ \/ __ `/ __ \/ _ \/ ___/  / /      
 ___/ / /_/ / /_/ /  __/ /  / /___/ /  __/ /_/ / / / /  __/ /     / /___    
/____/\__,_/ .___/\___/_/   \____/_/\___/\__,_/_/ /_/\___/_/      \____/    
          /_/                                                               
```

**Next-Generation High-Performance Windows System Optimizer & Deep Cleaner**

[![Windows](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20(x64)-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/weka-eg/SuperCleanerC-Releases)
[![.NET 8.0](https://img.shields.io/badge/.NET-8.0%20WPF%20(Self--Contained)-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/)
[![Version](https://img.shields.io/badge/Version-v1.2%20(Production)-2ea44f?style=for-the-badge&logo=semver&logoColor=white)](https://github.com/weka-eg/SuperCleanerC-Releases/releases)
[![Build Status](https://img.shields.io/badge/Build-Passing%20%26%20Signed-brightgreen?style=for-the-badge&logo=powershell&logoColor=white)](https://github.com/weka-eg/SuperCleanerC-Releases)
[![Code Signing](https://img.shields.io/badge/Authenticode-WEKA%20TEAM%20(SHA--256)-blue?style=for-the-badge&logo=security&logoColor=white)](https://github.com/weka-eg/SuperCleanerC-Releases)
[![License](https://img.shields.io/badge/License-Proprietary%20%7C%20WEKA%20TEAM-orange?style=for-the-badge)](https://t.me/Vandiom5)


---

</div>

##  Overview

**Super Cleaner C** is an enterprise-grade, standalone Windows optimization and deep cleaning utility engineered in C# and WPF on .NET 8. It targets supported system junk, temporary data, caches, and Windows maintenance items that may accumulate over time.

Designed as a **portable, single-file executable**, Super Cleaner C requires no installation, leaves no unmanaged registry leftovers, and comes fully bundled with its .NET 8 runtime for instant execution on any modern 64-bit Windows environment.

---

##  Key Features

| Feature | Description |
| :--- | :--- |
| **Deep System Cleaning** | Scans supported Windows locations and identifies removable system and temporary data. |
| **Windows Maintenance** | Provides supported Windows maintenance and optimization tools. |
| **Developer Cache Cleaning** | Helps clean supported caches created by development tools and package managers. |
| **Hibernation Management** | Provides a convenient option to manage Windows hibernation settings. |
| **Background Monitoring** | Optional system-tray monitoring helps track accumulated temporary data. |
| **Cloud Services** | Internet connectivity may be used for activation, configuration, and service-related functionality. |
| **Hardware-Bound Licensing** | Activation keys are associated with the authorized device to help prevent unauthorized use. |
| **Automatic Updates** | The application can notify users when a newer official release is available. |

---

##  Installation

Super Cleaner C is 100% portable. No installer, wizard, or third-party dependencies are required.

1. **Download** the latest release bundle (`SuperCleanerC.exe` or `SuperCleanerC_v1.2.zip`) from the official repository:
   - [Official Releases Repository](https://github.com/weka-eg/SuperCleanerC-Releases/releases)
   - Or contact our team directly via [Telegram Support](https://t.me/Vandiom5)
2. **Move** `SuperCleanerC.exe` to your preferred folder (e.g., `C:\Tools\SuperCleanerC\` or USB flash drive).
3. **Right-click** and select **Run as Administrator** (Administrative elevation is required to manage DISM, Windows Installer caches, and system-level directories).
4. Enter your unique **Activation Key** when prompted. An Internet connection is required for the initial activation.

> [!IMPORTANT]
> Super Cleaner C modifies system-protected caches. **Administrator privileges** are mandatory. The application will automatically request UAC elevation upon launch.

---

##  System Requirements

| Requirement | Minimum Specification | Recommended Specification |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 (64-bit, Version 1809+) | Windows 11 (64-bit, All Builds) |
| **Architecture** | x64 (AMD64 / Intel 64) | x64 |
| **Runtime** | **None** (Bundled .NET 8 Self-Contained) | **None** (Bundled .NET 8 Self-Contained) |
| **Privileges** | Local Administrator Rights | Local Administrator Rights |
| **Memory (RAM)** | 512 MB available | 2 GB+ |
| **Disk Space** | 180 MB free for executable | 500 MB free storage |
| **Network** | Internet connection for initial activation | Broadband connection for real-time cloud updates |

---

##  How It Works

Super Cleaner C uses a multi-stage workflow designed to make supported Windows maintenance tasks simple and safe while keeping proprietary implementation details private.

### 1. Activation & Configuration
The first activation requires an Internet connection. After successful activation, the application can operate in **Offline Mode** for normal supported use without requiring a continuous Internet connection.

Internet access may still be required for services such as activation-related checks, configuration synchronization, or checking for new official releases.

### 2. Scanning
When you start a scan, the application checks supported system and temporary locations and calculates the amount of data that can potentially be cleaned.

### 3. Cleaning
After reviewing the scan results, supported items can be cleaned through the application's interface. The application is designed to avoid interfering with active Windows components and installed applications.

### 4. Background Monitoring
When enabled, the application can remain available in the Windows notification area and periodically monitor supported temporary-data locations.

> **Implementation Note:** The internal cleaning logic, detection rules, licensing implementation, cloud configuration structure, and other proprietary components are intentionally not documented in this repository.

---

##  Integrity & SHA-256 Verification

Every official release binary is code-signed by **WEKA TEAM** and published with a cryptographic SHA-256 checksum. Always verify your download before running.

### 1. Verify SHA-256 Checksum via PowerShell
```powershell
Get-FileHash -Path ".\SuperCleanerC.exe" -Algorithm SHA256 | Format-List
```
Compare the output hash with the official hash published in the [GitHub Release Notes](https://github.com/weka-eg/SuperCleanerC-Releases).

### 2. Verify Authenticode Digital Signature
```powershell
Get-AuthenticodeSignature -FilePath ".\SuperCleanerC.exe" | Format-List
```
Expected Status: `Valid`  
Signer Subject: `CN=WEKA TEAM, O=WEKA TEAM, C=EG`  
Hash Algorithm: `SHA256`

---

##  Security & Privacy

Super Cleaner C is designed with privacy and security in mind.

- The application does not need access to your personal documents, photos, passwords, or keystrokes to perform its supported cleaning functions.
- Internet connectivity is used for supported online services such as activation, configuration, and release/update checks.
- After successful activation, normal supported operation can be performed offline.
- Proprietary implementation details related to licensing, configuration, and internal application logic are not publicly disclosed.

For additional information, please refer to the privacy and security documentation included with the official release when available.

---

##  License

**Super Cleaner C** is proprietary software developed and owned by **WEKA TEAM**.

- **Copyright © 2026 WEKA TEAM. All rights reserved.**
- Single-seat licenses are restricted to **1 physical PC per activation key**.
- Unauthorized redistribution, decompilation, modification, or cracking is strictly prohibited.

---

##  Contact & Support

Need assistance, bulk licenses, or want to report an issue? Reach out directly:

- **Lead Developer**: WEKA TEAM
- **Official Telegram Support**: [@Vandiom5](https://t.me/Vandiom5)
- **Direct Telegram Channel**: [https://t.me/Vandiom5](https://t.me/Vandiom5)
- **GitHub Repository**: [weka-eg/SuperCleanerC-Releases](https://github.com/weka-eg/SuperCleanerC-Releases)

---

<div align="center">
  <sub>Built with ❤️ by WEKA TEAM. Empowering Windows users with cleaner, faster, and healthier PCs.</sub>
</div>
