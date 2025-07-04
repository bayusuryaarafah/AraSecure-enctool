# Aracrypt - File Encryption Tool 🔐

**Aracrypt** adalah aplikasi GUI berbasis Python yang digunakan untuk mengenkripsi dan mendekripsi berbagai jenis file menggunakan algoritma AES-GCM 256-bit dengan perlindungan passphrase. Aplikasi ini cocok untuk pengguna umum hingga teknisi yang ingin menjaga keamanan data file mereka secara lokal.

---

## 📌 Fitur Utama

- 🔐 **Enkripsi dan Dekripsi File** dengan AES-GCM (256-bit)
- 🔑 **Validasi Passphrase**: Cek kekuatan dan kesesuaian passphrase
- 🧠 **Indikator Kekuatan Passphrase**: Weak, Medium, atau Strong
- 📁 **Pilih Lokasi Output File**: Bebas menentukan lokasi hasil enkripsi
- 📊 **Progress Bar**: Menunjukkan status proses enkripsi
- ✅ **Checksum Verifikasi SHA-256**: Memastikan integritas file saat dekripsi
- 🛡️ **File Asli Tidak Dihapus**: Proses enkripsi tidak menghapus file sumber

---

## 📎 Jenis File yang Didukung

Aracrypt dapat mengenkripsi **semua jenis file**, seperti:
- 📄 `.pdf`, `.docx`, `.txt`
- 🖼️ `.jpg`, `.png`, `.bmp`
- 🎥 `.mp4`, `.mkv`
- 📦 `.zip`, `.rar`, `.exe`
- Dan file biner lainnya

---

## 🛠️ Teknologi yang Digunakan

| Komponen       | Fungsi                                      |
|----------------|---------------------------------------------|
| `Python 3.8+`  | Bahasa pemrograman                          |
| `Tkinter`      | Antarmuka GUI                               |
| `cryptography` | Enkripsi AES-GCM & derivasi kunci (Scrypt) |
| `hashlib`      | Verifikasi SHA-256                          |
| `PyInstaller`  | Konversi ke `.exe` (opsional)               |
| `PyArmor`      | Obfuscation (opsional)                      |

---

## 📥 Instalasi & Prasyarat

### 1. Instal Python dan pip
Pastikan Python 3.8+ telah terpasang. Unduh dari: https://www.python.org

### 2. Instal dependensi
```bash
pip install cryptography

🧪 Cara Menggunakan
🔐 Enkripsi File
Pilih file yang ingin dienkripsi

Pilih lokasi output hasil enkripsi

Masukkan dan konfirmasi passphrase

Klik tombol "Enkripsi"

File .enc dan checksum akan dihasilkan

🔓 Dekripsi File
Pilih file .enc

Masukkan passphrase yang sesuai

Klik "Dekripsi"

File asli akan dikembalikan dengan .dec jika passphrase & checksum cocok
