> **PowerShell script to copy photos and videos from iPhone to Windows PC via USB**


## What problem does this solve?

Transferring photos from an iPhone to a Windows PC is often a frustrating experience. Windows doesn't always recognize the iPhone as a standard drive, and manually copying files from folders like `100APPLE` or `200801__` is time-consuming and error-prone.

**This script solves that problem** by:
1. **Automatically detecting** your connected iPhone
2. **Finding** all photos and videos regardless of folder structure
3. **Copying** them to a folder of your choice
4. **Handling duplicates** automatically
5. **Reporting errors** without stopping the transfer

> 🎯 **Target users:** Anyone who wants a reliable, one-click solution to back up iPhone photos and videos to an external hard drive or Windows PC.

---

## ✨ Features

| Feature | Description |
| :--- | :--- |
| 🔍 **Automatic iPhone Detection** | Detects your iPhone by name (`Apple iPhone`) without needing a drive letter |
| 📂 **Smart Folder Selection** | Opens a classic Windows folder dialog to choose your destination |
| 📸 **Copies Everything** | Photos (`.JPG`, `.PNG`, `.HEIC`) and videos (`.MOV`, `.MP4`) |
| 🔄 **Duplicate Handling** | Automatically renames files if a file with the same name already exists |
| 📊 **Detailed Progress Bar** | Visual progress bar with percentage complete |
| ❌ **Resilient Error Handling** | Continues even if a single file fails; provides a summary at the end |
| 💾 **100% Safe** | Uses `CopyHere` - **never deletes** your original iPhone files |
| 🚀 **No Installation Required** | Just download and run - no third-party software needed |

---

## 📖 Table of Contents

- [What problem does this solve?](#what-problem-does-this-solve)
- [Features](#features)
- [Quick Start](#quick-start)
- [Installation](#installation)
- [How It Works](#how-it-works)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)
- [FAQ](#faq)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---


# 📱 iPhone Photo Transfer Script

[![Licence MIT](https://img.shields.io/badge/Licence-MIT-blue.svg)](LICENSE)
[![PowerShell Version](https://img.shields.io/badge/PowerShell-5.1+-blueviolet.svg)](https://github.com/PowerShell/PowerShell)
[![GitHub stars](https://img.shields.io/github/stars/votre-nom-utilisateur/iPhone-Photo-Transfer.svg?style=social)](https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/votre-nom-utilisateur/iPhone-Photo-Transfer.svg?style=social)](https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer/network/members)

## 🚀 Quick Start

```powershell
# 1. Connect your iPhone via USB
# 2. Unlock it and tap "Trust"
# 3. Clone the repository
git clone https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer.git

# 4. Run the script
cd iPhone-Photo-Transfer
.\src\Copy-iPhonePhotos.ps1

# 5. Select a destination folder
# 6. Wait for the transfer to complete
# 7. Check the summary report
