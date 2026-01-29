# Automated TrollRestore Installer for Windows

An automation script designed to streamline the **TrollRestore** installation process. This tool leverages a `.bat` wrapper to trigger the installation sequence automatically upon USB connection.

Directly utilizes the core logic from [JJTech0130/TrollRestore](https://github.com/JJTech0130/TrollRestore/).

## 🚀 Features
* **Plug-and-Play:** Zero-touch execution once the script is active.
* **Auto-Detection:** Automatically detects your iOS device via USB to initiate the restore process.
* **Windows Optimized:** Tailored specifically for Windows environments.

## 📋 Prerequisites
* **OS:** Windows 10 or 11.
* **iTunes:** **Mandatory.** Must be installed for mobile device drivers.
* **TrollRestore:** Ensure the `TrollRestore` executable is present in the working directory.

## 📱 iOS Version Support

| Version Range | Support Status |
| :--- | :--- |
| **iOS 15.2 - 16.7 RC (20H18)** | ✅ Supported |
| **iOS 17.0 (All Builds)** | ✅ Supported (21A326, 21A327, 21A329, 21A331) |
| **iOS 15.0 - 15.1.1** | ⚠️ Experimental (Potential restore issues) |
| **iOS 14.x and below** | 🚫 Disabled (Stability issues) |

> [!IMPORTANT]
> Support for iOS 14 and below is currently disabled due to backup restoration failures. While 15.0 - 15.1.1 remains enabled, use it with caution as similar issues have been reported post-release.

## 🛠 Usage
1.  Download the latest release and extract all files to a folder.
2.  Launch the automation script:
    ```cmd
    trollrestore.bat
    ```
3.  Connect your device via USB. The script will handle the deployment automatically.

## ⚖️ Disclaimer
This is an unofficial automation wrapper. I am not responsible for any data loss. Always back up your device before performing system-level modifications.

---
**Credits:** Original tool by [JJTech0130](https://github.com/JJTech0130/TrollRestore/).
