# Automated TrollRestore Installer for Windows

An automation script designed to streamline the **TrollRestore** installation process. This tool leverages a `.bat` wrapper to trigger the installation sequence automatically upon USB connection.

Directly utilizes the core logic from [JJTech0130/TrollRestore](https://github.com/JJTech0130/TrollRestore/).

## 🚀 Features
* **Plug-and-Play:** Zero-touch execution once the script is active.
* **Auto-Detection:** Automatically detects your iOS device via USB to initiate the restore process.
* **Windows Optimized:** Tailored specifically for Windows environments.

## 📋 Prerequisites
* **OS:** Windows 10 or 11.
* **iTunes:** **Mandatory.** Must be installed for mobile device drivers (Win32 version recommended).
* **TrollRestore:** Ensure the `TrollRestore` executable is present in the working directory.

## 📱 iOS Version Support

| Version Range | Support Status |
| :--- | :--- |
| **iOS 15.2 - 16.7 RC (20H18)** | ✅ Supported |
| **iOS 17.0 (All Builds)** | ✅ Supported (21A326, 21A327, 21A329, 21A331) |
| **iOS 15.0 - 15.1.1** | ⚠️ Experimental (Potential restore issues) |
| **iOS 14.x and below** | 🚫 Disabled (Stability issues) |

## 🛠 Usage
1.  Download the latest release and extract all files to a folder (.exe must include).
2.  Launch the automation script:
    ```cmd
    trollrestore.bat
    ```
3.  Connect your device via USB. The script will handle the deployment automatically.
4.  **Post-Installation:** Once the process finishes successfully, open the **Tips** app on your device to proceed with the TrollStore installation.

## ⚠️ Important Notes (Read Before Use)

### Language & Target App Localization
If your device is set to a language other than English, the script may fail to locate the **Tips** app. 
* **Recommended Fix:** Change the target application to **Bridge** (Watch app) to ensure compatibility. 
* To do this via command line:
  ```cmd
  echo Bridge>troll_input.txt
