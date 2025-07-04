# Aracrypt - File Encryption Tool 🔐

**Aracrypt** adalah aplikasi desktop berbasis GUI yang dikembangkan menggunakan Python untuk melakukan proses enkripsi dan dekripsi file secara lokal dengan tingkat keamanan tinggi. Aplikasi ini menggunakan algoritma AES-GCM 256-bit yang modern dan aman, serta dilengkapi proteksi passphrase dan verifikasi checksum SHA-256 guna menjaga integritas data. Dirancang untuk mendukung berbagai jenis file, Aracrypt dapat digunakan oleh pengguna umum, profesional TI, hingga praktisi keamanan siber yang membutuhkan solusi proteksi file yang praktis, cepat, dan kuat tanpa koneksi internet.

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

| Komponen                           | Fungsi                                                                 |
|------------------------------------|------------------------------------------------------------------------|
| `Python 3.8+`                      | Bahasa pemrograman utama                                               |
| `Tkinter`                          | Antarmuka GUI (Graphical User Interface)                               |
| `cryptography.AESGCM`             | Enkripsi & dekripsi menggunakan algoritma AES-GCM 256-bit               |
| `cryptography.Scrypt`             | Derivasi passphrase menjadi kunci aman (Key Derivation Function)        | 
| `hashlib.sha256`                  | Menghasilkan checksum SHA-256 untuk verifikasi integritas file          |
| `re` (Regex)                      | Validasi kekuatan dan kompleksitas passphrase                           |
| `threading`                       | Menjalankan enkripsi tanpa membekukan GUI (proses paralel)              |
| `os`, `struct`, `filedialog` dll. | Akses file, direktori, dan format biner                                 |

---

## 📥 Instalasi & Prasyarat

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
5. File .enc dan checksum akan dihasilkan

---

### 🔓 Dekripsi File
1. Pilih file .enc
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
