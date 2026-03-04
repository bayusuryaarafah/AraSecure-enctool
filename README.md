# AraSecure - File Encryption Tool 🔐

**AraSecure** is a security-focused desktop application built in Python for local file encryption and decryption using AES-256-GCM (authenticated encryption). It ensures both confidentiality and integrity by deriving encryption keys from user passphrases through a secure key derivation mechanism and enforcing SHA-256–based integrity verification. The application uses a chunk-based processing architecture to securely handle large files with memory efficiency and operates entirely offline, minimizing network exposure.

AraSecure also includes an integrated checksum utility (MD5, SHA1, SHA256, SHA512) for independent file integrity validation, making it suitable for IT professionals and cybersecurity practitioners who require a practical, modern cryptographic file protection tool.

![Platform](https://img.shields.io/badge/platform-Windows-blue)
![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![Encryption](https://img.shields.io/badge/encryption-AES--256--GCM-green)
![Status](https://img.shields.io/badge/status-Active-success)

## Metadata
- Original File Name: AraSecure.exe
- Version: 3.1.2
- Size: 15.074 KB
- Last Updated: 5/03/2026

### Checksum SHA-256
```bash
2f2be780fd3fe4f2a55c94c83029cb2596d99f93ec87ef59a53957ac4569188c
```
---

# 🚀 Features

## 🔐 Encryption & Decryption
- AES-GCM (256-bit symmetric encryption)
- Authenticated encryption (integrity + confidentiality)
- Chunk-based processing (>10GB support)
- Custom encrypted file header validation

## 🔑 Passphrase Protection
- Input validation & confirmation
- Strength indicator (Weak / Medium / Strong)
- Dictionary-based weak passphrase detection
- Regex-based complexity validation

## 📁 File Management
- Custom output directory
- Optional original file deletion
- Real-time progress bar
- Large file support

## 🧾 Checksum Utility
Supported algorithms:
- MD5
- SHA1
- SHA256
- SHA512

Modes:
- Hash Generator (auto-copy to clipboard)
- Hash Verifier (manual comparison)

---

# 🖥️ Supported Operating System

⚠️ Windows Only

- Windows 10 (32-bit / 64-bit)
- Windows 11 (32-bit / 64-bit)

Linux & macOS support planned.

---

# 📎 Supported File Types

AraSecure can encrypt all types of files:

- Documents (`.pdf`, `.docx`, `.txt`)
- Images (`.jpg`, `.png`, `.bmp`)
- Videos (`.mp4`, `.mkv`)
- Archives (`.zip`, `.rar`)
- Executables (`.exe`)
- Other binary files

No file-type restriction applied.

---

# 📦 File Size Limitation

Designed to securely process files larger than **10GB**  
Chunk size: 4MB per block (memory-efficient design)

---

# 🛠️ Technology Stack

| Component | Purpose |
|------------|----------|
| Python 3.8+ | Core programming language |
| Tkinter | GUI framework |
| cryptography.AESGCM | AES-256-GCM encryption |
| cryptography.Scrypt | Key derivation function (KDF) |
| hashlib | File integrity verification |
| threading | Non-blocking process execution |
| os / struct | File & binary structure management |

---

# 🔐 Security Architecture

1. User provides passphrase
2. Random salt is generated
3. Scrypt derives a 256-bit key
4. AES-GCM performs authenticated encryption
5. Custom file header is written
6. Integrity is verified before decryption

---

# ⚠️ Important Notes

- Lost passphrase = file cannot be recovered.
- Minimum recommended passphrase length: 16+ characters.
- Always backup original file before encryption.
- Do not modify encrypted file structure manually.

---

# 📥 Installation

## Download Release

1. Go to **Releases**
2. Download the installer `.exe`
3. Run installer
4. Done

---

# 👨‍💻 Contributors & Developers

This application was developed by:

### Bayu S. Arafah  
🔐 IT Security Engineer | 🧠 Python Developer  
📍  Jakarta, Indonesia  
🔗 LinkedIn: [linkedin.com/in/bayu-surya-arafah](https://linkedin.com/in/bayu-surya-arafah/)
