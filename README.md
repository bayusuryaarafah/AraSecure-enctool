# AraSecure - File Encryption Tool 🔐

**AraSecure** adalah aplikasi desktop berbasis GUI yang dikembangkan menggunakan Python untuk melakukan proses enkripsi dan dekripsi file secara lokal dengan tingkat keamanan tinggi. Aplikasi ini menggunakan algoritma AES-GCM 256-bit yang modern dan aman, serta dilengkapi proteksi passphrase dan verifikasi checksum SHA-256 guna menjaga integritas data. Pada fitur lain AraSecure menyediakan checksum (hash generator dan verifier) untuk memverifikasi integritas file menggunakan algoritma hash seperti MD5, SHA1, SHA256, dan SHA512. Dirancang untuk mendukung berbagai jenis file, AraSecure dapat digunakan oleh pengguna umum, profesional TI, hingga praktisi keamanan siber yang membutuhkan solusi proteksi file yang praktis, cepat, dan kuat tanpa koneksi internet.

## Metadata
- Original File Name: AraSecure.exe
- Version: 3.1.1
- Size: 14.826 KB
- Last Updated: 03/08/2025

### Checksum SHA-256
```bash
7fec0f4034af9491c9d11d9b418f74fd5982e337da8347cb54f50cdbd1e0b2ce
```
---

## 📌 Fitur Utama

- 🔐 **Enkripsi dan Dekripsi File** dengan AES-GCM (256-bit) symmetric-based encryption
- 🔑 **Validasi Passphrase**: Cek kekuatan dan kesesuaian passphrase
- 🧠 **Indikator Kekuatan dan Pemeriksaan Passphrase**: Weak, Medium, atau Strong dan Deteksi passphrase lemah melalui wordlist dictionary
- 📁 **Pilih Lokasi Output File**: Bebas menentukan lokasi hasil enkripsi
- 📊 **Progress Bar**: Menunjukkan status proses enkripsi
- ✅ **Checksum Verifikasi SHA-256**: Memastikan integritas file saat dekripsi
- 🛡️ **Opsi File Asli Tidak Dihapus**: Dapat menghapus file sumber atau tidak menghapus (Opsional)

---

## 🧾 Checksum Utility

AraSecure mendukung algoritma checksum:
- MD5
- SHA1
- SHA256
- SHA512

Mode: 
- Hash Generator: Menghasilkan hash dari file dan menyalinnya ke clipboard
- Hash Verifier: Membandingkan hash file dengan checksum yang diberikan

---

## 🖥️ Sistem Operasi yang Didukung

> ⚠️ **AraSecure hanya dapat dijalankan pada sistem operasi Windows (Windows 10/11 - 64/86-bit).** Aplikasi ini **belum mendukung** sistem operasi Linux atau MacOS. Coming Soon!

---

## 📎 Jenis File yang Didukung

AraSecure dapat mengenkripsi **semua jenis file**, seperti:
- 📄 `.pdf`, `.docx`, `.txt`
- 🖼️ `.jpg`, `.png`, `.bmp`
- 🎥 `.mp4`, `.mkv`
- 📦 `.zip`, `.rar`, `.exe`
- Dan file biner lainnya

---

## 📦 Batasan Ukuran File

> 📁 **Ukuran maksimum file yang dapat dienkripsi/dekripsi saat ini adalah > 10GB**

---

## 🛠️ Teknologi yang Digunakan

| Komponen                           | Fungsi                                                                 |
|------------------------------------|------------------------------------------------------------------------|
| `Python 3.8+`                      | Bahasa pemrograman utama                                               |
| `Tkinter`                          | Antarmuka GUI (Graphical User Interface)                               |
| `cryptography.AESGCM`             | Enkripsi & dekripsi menggunakan algoritma AES-GCM 256-bit               |
| `cryptography.Scrypt`             | Derivasi passphrase-based encryption (Key Derivation Function)          | 
| `hashlib.sha256`                  | Menghasilkan checksum SHA-256 untuk verifikasi integritas file          |
| `re` (Regex)                      | Validasi kekuatan dan kompleksitas passphrase                           |
| `threading`                       | Menjalankan enkripsi tanpa membekukan GUI (proses paralel)              |
| `os`, `struct`, `filedialog` dll. | Akses file, direktori, dan format biner                                 |

---

## 📥 Instalasi & Prasyarat (Console-only)

### 1. Instal Python dan pip
Pastikan Python 3.8+ telah terpasang. Unduh dari: https://www.python.org

### 2. Instal dependensi
```bash
pip install cryptography
```

## 🧪 Cara Menggunakan
### 🔐 Enkripsi File
1. Pilih file yang ingin dienkripsi
2. Pilih lokasi output hasil enkripsi
3. Masukkan dan konfirmasi passphrase
4. Klik tombol "Enkripsi"
5. File .arasec dan checksum akan dihasilkan

---

### 🔓 Dekripsi File
1. Pilih file .arasec
2. Masukkan passphrase yang sesuai
3. Klik "Dekripsi"
4. File asli akan dikembalikan dengan .dec jika passphrase & checksum cocok

---

# 👨‍💻 Kontributor & Pengembang

Aplikasi ini dikembangkan oleh:

### Bayu S. Arafah  
🔐 IT Security Engineer | 🧠 Python Developer  
📍  Jakarta, Indonesia  
🔗 LinkedIn: [linkedin.com/in/bayu-surya-arafah](https://linkedin.com/in/bayu-surya-arafah/)
