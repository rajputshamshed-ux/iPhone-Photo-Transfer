# iPhone-Photo-Transfer
PowerShell script to copy photos and videos from iPhone to Windows PC via USB. Automatic detection, folder selection, duplicate handling, and error reporting.

# 📱 iPhone Photo Transfer Script

[![Licence MIT](https://img.shields.io/badge/Licence-MIT-blue.svg)](LICENSE)
[![PowerShell Version](https://img.shields.io/badge/PowerShell-5.1+-blueviolet.svg)](https://github.com/PowerShell/PowerShell)

Un script PowerShell robuste et facile à utiliser pour copier toutes vos photos et vidéos de votre iPhone vers un dossier de votre choix sur un PC Windows.

---

## ✨ Fonctionnalités

- **🔍 Détection automatique de l'iPhone** : Détecte votre iPhone connecté par son nom (`Apple iPhone` par défaut) sans avoir besoin d'une lettre de lecteur.
- **📂 Sélection intelligente du dossier** : Ouvre une boîte de dialogue Windows classique pour choisir exactement où enregistrer vos photos.
- **📸 Copie tout** : Transfère tous les médias, y compris les photos (`.JPG`, `.PNG`, `.HEIC`) et les vidéos (`.MOV`, `.MP4`).
- **🔄 Gestion des doublons** : Renomme automatiquement les fichiers si un fichier avec le même nom existe déjà dans la destination.
- **📊 Barre de progression détaillée** : Une barre de progression visuelle indique l'état du transfert et le pourcentage complété.
- **❌ Gestion robuste des erreurs** : Le script continue même si un fichier échoue, et fournit un résumé des erreurs à la fin.
- **💾 100% Sûr** : Le script utilise `CopyHere`, donc vos fichiers originaux sur l'iPhone **ne sont jamais supprimés**. C'est une opération en lecture seule.

---

## 📋 Prérequis

- Un PC Windows avec **PowerShell 5.1 ou supérieur** (Windows 10 et 11 sont recommandés).
- Votre **iPhone connecté** au PC via un câble USB.
- Votre iPhone **déverrouillé** et vous avez **approuvé l'ordinateur** en appuyant sur "Approuver" lorsque vous y êtes invité.
- Suffisamment d'espace libre sur votre disque de destination.

---

## 🚀 Comment utiliser

### 1. Télécharger le script

**Option A : Cloner le dépôt (recommandé)**
```powershell
git clone https://github.com/votre-nom-utilisateur/iPhone-Photo-Transfer.git
