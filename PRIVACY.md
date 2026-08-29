# Privacy Policy for Super Cleaner C

**Last Updated:** August 29, 2026  
**Effective Date:** August 28, 2026  
**Developer:** WEKA TEAM  
**Contact:** [@Vandiom5](https://t.me/Vandiom5)

---

##  Our Privacy Commitment

**WEKA TEAM** is committed to protecting your privacy and ensuring you have complete control over your personal data. **Super Cleaner C** is engineered under a strict **Privacy-by-Design** philosophy. We build tools to optimize your Windows system, not to harvest your personal information.

This Privacy Policy explains what data Super Cleaner C processes, how and where that data is stored, why it is needed, and your rights to inspect or delete your records.

---

## 📊 Summary of Data Practices

| Category | Description | Stored Locally | Stored in Cloud |
| :--- | :--- | :---: | :---: |
| **Hardware Fingerprint (HWID)** | SHA-256 one-way cryptographic hash of Windows `MachineGuid`. | Yes | Yes (Firebase) |
| **Operating System** | Generic OS family string (e.g. `Windows 10`, `Windows 11`). | N/A | Yes (Firebase) |
| **Application Version** | Installed version number (e.g. `1.2`). | Yes | Yes (Firebase) |
| **Sanitized Machine Name** | Partially anonymized/truncated machine moniker (first 3 characters). | N/A | Yes (Firebase) |
| **Cleaning Metrics** | Cumulative bytes freed and count of clean operations completed. | Yes | Yes (Firebase) |
| **IP Address** | Public IP address recorded strictly during one-time license activation. | No | Yes (Activation Only) |
| **Personal Files & Documents** | Any user files, photos, downloads, desktop content. | **NEVER** | **NEVER** |
| **Browsing & Credentials** | Web history, cookies, passwords, form entries. | **NEVER** | **NEVER** |

---

##  Data We Collect and Process

### 1. Anonymous Hardware Identifier (HWID)
- **What it is:** A 16-character hexadecimal string derived by computing an irreversible SHA-256 hash over the system's Windows `MachineGuid` registry entry.
- **What it is NOT:** It does **not** reveal your motherboard serial number, MAC address, CPU serial, or BIOS information.
- **Why we need it:** To enforce our **1-PC hardware binding** policy for purchased license keys and prevent unauthorized multi-device cloning.

### 2. Operating System & Application Version
- **What it is:** High-level OS identifier (e.g. "Windows 11" or "Windows 10") and the current version string of Super Cleaner C (e.g. "1.2").
- **Why we need it:** To deliver compatible remote cleaning rules, suppress incompatible cleaner options (such as legacy DISM routines), and notify users of critical updates or deprecated builds.

### 3. Partially Anonymized Computer Name
- **What it is:** A truncated, sanitized representation of the computer name (only first 3 characters preserved, e.g. `DES***` or `LAP***`).
- **Why we need it:** Allows users and administrators to recognize their activated devices inside their license management dashboard without disclosing full device network monikers.

### 4. Cleaning Performance Statistics
- **What it is:** Aggregate counters of storage space reclaimed (in bytes) and the total number of maintenance cycles run.
- **Why we need it:** To evaluate the effectiveness of individual cleaner modules across releases and provide users with a lifetime savings tracker.

### 5. Transient IP Address (Activation Only)
- **What it is:** The public IPv4/IPv6 address detected during the single-instance moment of license key binding.
- **Why we need it:** To prevent brute-force activation abuse, geographic license piracy, and key cracking. **IP addresses are never captured or logged during regular system cleaning cycles or background scans.**

---

##  Data We NEVER Collect

We strictly reject the collection of sensitive and personal data. Super Cleaner C **never** accesses, scans, reads, or transmits:

- ❌ **Personal Documents:** Word files, PDFs, spreadsheets, source code, images, videos, or desktop files.
- ❌ **Browsing History & Cookies:** URLs visited, bookmarks, search history, saved form data, or session cookies.
- ❌ **Credentials & Secrets:** Passwords, private keys, SSH tokens, API keys, or Windows user passwords.
- ❌ **Keystrokes & Inputs:** Keylogger functionality is completely absent.
- ❌ **Screen & Media Streams:** No screen captures, window recording, webcam, or microphone access.
- ❌ **Precise Geolocation:** No GPS coordinates, WiFi triangulation, or beacon data.
- ❌ **Personal Identity:** No names, phone numbers, email addresses, or payment card details.

> [!NOTE]
> All cleaning operations on temporary directories, prefetch logs, installer caches, and crash dumps operate locally in memory. The files are purged directly on your storage drive without their contents ever being uploaded to any server.

---

## ☁️ Where Data is Stored & Infrastructure Security

- **Cloud Platform:** Google Firebase Realtime Database (hosted on Google Cloud Platform enterprise infrastructure).
- **Transport Encryption:** All telemetry and license validation requests are secured via **HTTPS / TLS 1.2+** with modern cipher suites.
- **At-Rest Encryption:** Cloud database instances are protected with standard AES-256 storage-level encryption.
- **Local Storage:** On your local device, license validation state is safeguarded inside the Windows Registry (`HKCU\Software\SuperCleanerC\License`) using salted cryptographic hashes.

---

##  Purpose and Lawful Basis of Processing

We process telemetry and hardware identifiers exclusively for the following operational reasons:

1. **License Fulfillment & Verification:** Validating license authenticity and preventing unauthorized simultaneous usage on multiple machines.
2. **Remote Configuration Delivery:** Distributing updated cleaning paths, DISM rule updates, and urgent security patches in real-time.
3. **Operational Stability & Maintenance:** Broadcasting scheduled maintenance notices and preventing deprecated or vulnerable client versions from operating.
4. **Aggregate Analytics:** Calculating global space saved by the community to guide future engine optimizations.

---

##  Data Retention and Right to Deletion

We respect your right to data sovereignty. You may request the permanent purge of your device record from our cloud database at any time.

### How to Request Data Deletion:
1. Contact our support team on Telegram: [https://t.me/Vandiom5](https://t.me/Vandiom5) (@Vandiom5).
2. Provide your License Key or the anonymous HWID displayed in your application About screen.
3. Our administrators will delete your telemetry entry, heartbeat records, and associated activation metadata within **48 hours**.

> [!TIP]
> Uninstalling or deleting `SuperCleanerC.exe` and clearing registry key `HKCU\Software\SuperCleanerC` will instantly halt all communication with our servers.

---

##  Third-Party Sharing

- **Zero Third-Party Advertising:** Super Cleaner C is completely ad-free. We do not integrate any advertising SDKs (such as AdMob, Unity, or AppLovin).
- **Zero Third-Party Analytics:** We do not embed external tracking frameworks such as Google Analytics, Segment, or Facebook Pixel.
- **No Data Brokering:** We do not sell, rent, lease, or monetize user data under any circumstances.

---

##  Updates to this Privacy Policy

We may update this Privacy Policy periodically to reflect new features or regulatory requirements. Any material changes will be broadcasted directly within the application via our real-time cloud notification service.

---

##  Contact Us

If you have questions, concerns, or requests regarding this Privacy Policy, please contact:

- **Developer:** WEKA TEAM
- **Direct Telegram:** [@Vandiom5](https://t.me/Vandiom5)
- **Telegram Support:** [https://t.me/Vandiom5](https://t.me/Vandiom5)
- **GitHub Repository:** [weka-eg/SuperCleanerC-Releases](https://github.com/weka-eg/SuperCleanerC/Releases)
