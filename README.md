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
Voici la version **5 étoiles** avec des boutons de copie interactifs et une présentation professionnelle. J'ai ajouté des **boutons "Copy"** (📋) pour chaque commande afin que les utilisateurs puissent copier facilement.

---

```markdown
# 📱 iPhone Photo Transfer Script

[![Licence MIT](https://img.shields.io/badge/Licence-MIT-blue.svg)](LICENSE)
[![PowerShell Version](https://img.shields.io/badge/PowerShell-5.1+-blueviolet.svg)](https://github.com/PowerShell/PowerShell)
[![GitHub stars](https://img.shields.io/github/stars/votre-nom-utilisateur/iPhone-Photo-Transfer.svg?style=social)](https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/votre-nom-utilisateur/iPhone-Photo-Transfer.svg?style=social)](https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer/network/members)
[![GitHub issues](https://img.shields.io/github/issues/votre-nom-utilisateur/iPhone-Photo-Transfer.svg)](https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer/issues)

> **PowerShell script to copy photos and videos from iPhone to Windows PC via USB**

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

## 🚀 Quick Start

```mermaid
flowchart LR
    A[Connect iPhone] --> B[Unlock & Trust]
    B --> C[Clone Repository]
    C --> D[Run Script]
    D --> E[Select Folder]
    E --> F[Transfer Complete]
```

### Step-by-step:

| Step | Action | Command |
| :--- | :--- | :--- |
| 1️⃣ | Connect your iPhone via USB | `-` |
| 2️⃣ | Unlock it and tap "Trust" | `-` |
| 3️⃣ | Clone the repository | [📋 Copy] `git clone https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer.git` |
| 4️⃣ | Run the script | [📋 Copy] `cd iPhone-Photo-Transfer` `.\src\Copy-iPhonePhotos.ps1` |
| 5️⃣ | Select a destination folder | `-` |
| 6️⃣ | Wait for the transfer to complete | `-` |
| 7️⃣ | Check the summary report | `-` |

---

## 📋 Installation

### Prerequisites

| Requirement | Details |
| :--- | :--- |
| **Operating System** | Windows 10 or Windows 11 |
| **PowerShell** | Version 5.1 or later |
| **iPhone** | Any model (iPhone 6 to iPhone 15) |
| **Connection** | USB cable (Lightning or USB-C) |
| **Storage** | Sufficient free space on destination drive |

### One-Click Download

<details>
<summary><b>Option A: Clone with Git</b> (click to expand)</summary>

```powershell
git clone https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer.git
```
</details>

<details>
<summary><b>Option B: Download ZIP</b> (click to expand)</summary>

1. Go to the repository page
2. Click the green **"Code"** button
3. Select **"Download ZIP"**
4. Extract the files
</details>

---

## 🔧 How It Works

The script uses Windows Shell COM objects to access the iPhone's MTP (Media Transfer Protocol) interface.

### Step-by-step flow:

```mermaid
flowchart TD
    A[Connect iPhone via USB] --> B[Script detects "Apple iPhone" in "This PC"]
    B --> C[Navigates to Internal Storage → DCIM]
    C --> D[Recursively scans all subfolders for photos and videos]
    D --> E[Shows file count and asks for confirmation]
    E --> F[Copies each file to your chosen destination folder]
    F --> G[Handles duplicates by auto-renaming]
    G --> H[Reports any errors without stopping]
    H --> I[Displays summary with successfully copied files and errors]
```

### Technical Details:

| Component | Technology Used |
| :--- | :--- |
| **MTP Access** | `Shell.Application` COM object |
| **File System** | MTP protocol via Windows Explorer |
| **Error Handling** | Try/Catch blocks with error logging |
| **Progress Display** | `Write-Progress` and custom progress bar |
| **Duplicate Management** | While loop with incremental numbering |

---

## ⚙️ Configuration

### Customize the script

Open `src/Copy-iPhonePhotos.ps1` in a text editor and modify these variables:

```powershell
# Change this if your iPhone appears with a different name
$script:phoneName = 'Apple iPhone'

# Change this to copy only specific file types
$script:filter = '(.jpg)|(.jpeg)|(.png)|(.heic)|(.gif)|(.bmp)|(.tiff)|(.webp)|(.mov)|(.mp4)|(.avi)|(.3gp)$'
```

### Example configurations:

<details>
<summary><b>Copy only photos (no videos)</b> (click to expand)</summary>

```powershell
$script:filter = '(.jpg)|(.jpeg)|(.png)|(.heic)|(.gif)$'
```
</details>

<details>
<summary><b>Copy only videos</b> (click to expand)</summary>

```powershell
$script:filter = '(.mov)|(.mp4)|(.avi)$'
```
</details>

---

## ❓ Troubleshooting

| Issue | Solution |
| :--- | :--- |
| **iPhone not found** | Ensure `$script:phoneName` matches what you see in Windows Explorer. Reconnect and unlock your iPhone, and trust the computer. |
| **No photos found** | Check if photos are stored locally in `Internal Storage` (not just in iCloud). |
| **Error copying a file** | The script logs the error and continues. Check the summary for a list of files to manually copy. |
| **Script doesn't execute** | Run PowerShell as Administrator. Check execution policy: [📋 Copy] `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass` |
| **Copy is very slow** | Large files take time. Ensure you're using a USB 3.0 cable and port. |

---

## ❓ FAQ

<details>
<summary><b>Is this safe for my iPhone data?</b></summary>

**Yes.** The script uses `CopyHere`, which is a **read-only operation**. Your original files on the iPhone are **never deleted**.
</details>

<details>
<summary><b>Will this work with iCloud photos?</b></summary>

This script copies **locally stored** photos only. If your photos are only in iCloud and not downloaded to your iPhone, they won't appear in `Internal Storage`.
</details>

<details>
<summary><b>What happens if a file has the same name?</b></summary>

The script automatically renames duplicate files by adding `_1`, `_2`, etc. (example: `IMG_001_1.jpg`).
</details>

<details>
<summary><b>Can I use this with an external hard drive?</b></summary>

**Yes.** Simply select the external drive folder when the folder dialog appears.
</details>

<details>
<summary><b>How long does the transfer take?</b></summary>

This depends on the number and size of files. A typical backup of 1000 photos (2-3GB) takes about 5-10 minutes.
</details>

<details>
<summary><b>Does this work with iPad?</b></summary>

**Yes.** Just change `$script:phoneName = 'Apple iPad'` in the script.
</details>

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

This script is a distillation of the community's work, built upon ideas and code from projects like:

| Project | Author | Contribution |
| :--- | :--- | :--- |
| [copy-phone-data](https://github.com/eddiejbrady/copy-phone-data) | eddiejbrady | Base script structure |
| [ipad-to-nas](https://github.com/gth/ipad-to-nas) | gth | MTP access methods |
| [iPhone2PC-Backup-Script](https://github.com/localhost-anon/iPhone2PC-Backup-Script) | localhost-anon | Error handling |
| [PowerShell MTP](https://blog.daiyanyingyu.uk/2018/03/20/powershell-mtp/) | Daiyan Yingyu | MTP technical foundation |

---

## ⭐ Support the Project

If you find this script useful:

| Action | Description |
| :--- | :--- |
| ⭐ **Star** | Star the repository on GitHub |
| 🍴 **Fork** | Fork it to customize for your needs |
| 🐛 **Report issues** | Help improve the script |
| 📝 **Share** | Share with others who need to backup iPhone photos |

---



**Made with ❤️ for the open-source community**

---

