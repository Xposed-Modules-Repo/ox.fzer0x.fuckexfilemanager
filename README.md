# FuckExFileManager

An Xposed module for **EX File Manager** that unlocks Pro features and eliminates advertisements dynamically using DexKit.

## 🚀 Features

- **Pro Unlock**: Automatically unlocks all Premium/VIP features.
- **Ad Block**: Completely removes integrated advertisements and tracking.
- **Dynamic Hooking**: Powered by [DexKit](https://github.com/LuckyPray/DexKit), the module finds the necessary methods by their signatures, making it resilient against app updates and code obfuscation.
- **Multi-Package Support**: Works with both `com.ace.ex.file.manager` and `com.ace.fileexplorer`.

## 🛠 How it works

Unlike traditional Xposed modules that rely on hardcoded method names (which change with every update), FuckExFileManager performs a "scan" of the app's code at runtime:
1. It identifies the Pro-license managers by searching for unique billing strings.
2. It detects the ad-initialization logic via known SDK signatures.
3. It hooks the identified methods regardless of their obfuscated names (e.g., `ace.rn3.a` vs `x.y.z`).

## 📥 Installation

1. Download and install the latest [Release APK](https://github.com/fzer0x/fuckexfilemanager/releases).
2. Open your Xposed Manager (LSPosed, EdXposed, etc.).
3. Enable the **FuckExFileManager** module.
4. Ensure the scope is set to **EX File Manager**.
5. Restart **EX File Manager**.

## 🖥 Screenshots

The module includes a simple UI to verify the status:
- **Module Status**: Active
- **Pro Unlock**: Enabled
- **Ad Block**: Enabled

## ⚠️ Disclaimer

This project is for educational purposes only. If you like the app, consider supporting the developers by purchasing the official Pro version. The author is not responsible for any misuse of this module.

---
Created by **fzer0x**
