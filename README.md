# KOMINFOTIK JAKARTA BARAT - STOK BARANG

## Pengembangan Aplikasi Mobile untuk Mendukung Pencatatan dan Pengelolaan Barang Habis Pakai di Lingkungan Sudis Kominfotik Jakarta Barat

---

# Deskripsi Aplikasi

Kominfotik Jakarta Barat - Stok Barang merupakan aplikasi mobile berbasis Flutter yang dikembangkan untuk membantu proses pencatatan, pengelolaan, dan monitoring barang habis pakai di lingkungan Sudis Kominfotik Jakarta Barat.

Aplikasi ini dirancang sebagai solusi atas proses pencatatan barang yang sebelumnya masih dilakukan secara manual menggunakan Microsoft Excel maupun dokumen fisik. Dengan adanya aplikasi ini, seluruh proses pencatatan barang masuk, barang keluar, pengelolaan stok gudang, serta distribusi barang ke setiap UKPD dapat dilakukan secara lebih cepat, akurat, dan terdokumentasi dengan baik.

Aplikasi menggunakan database SQLite sehingga seluruh data disimpan secara lokal pada perangkat tanpa memerlukan koneksi internet maupun server backend.

---

# Latar Belakang

Pengelolaan barang habis pakai merupakan salah satu kegiatan penting dalam mendukung operasional Sudis Kominfotik Jakarta Barat. Selama ini proses pencatatan barang masih dilakukan secara manual sehingga sering ditemukan beberapa kendala, seperti:

- Kesalahan pencatatan data barang.
- Sulit mengetahui jumlah stok yang tersedia.
- Riwayat distribusi barang kurang terdokumentasi.
- Proses pencarian data membutuhkan waktu yang cukup lama.
- Monitoring stok barang belum dilakukan secara real-time.

Berdasarkan kondisi tersebut, dikembangkan sebuah aplikasi mobile yang mampu membantu proses pencatatan dan monitoring stok barang secara digital sehingga pengelolaan barang menjadi lebih efektif dan efisien.

---

# Tujuan Pengembangan

Aplikasi ini dikembangkan dengan tujuan untuk:

- Mempermudah proses pencatatan barang habis pakai.
- Mempermudah proses pengelolaan stok barang.
- Mempermudah pencatatan barang masuk.
- Mempermudah proses distribusi barang keluar.
- Menyediakan informasi stok barang secara real-time.
- Menyediakan riwayat transaksi barang.
- Mengurangi kesalahan pencatatan secara manual.

---

# Teknologi yang Digunakan

| Komponen | Teknologi |
|-----------|-----------|
| Framework | Flutter |
| Bahasa Pemrograman | Dart |
| Database | SQLite |
| Platform | Android |
| IDE | Android Studio / Visual Studio Code |
| Version Control | Git |

---

# Fitur Aplikasi

Aplikasi memiliki beberapa fitur utama sebagai berikut.

## 1. Splash Screen

Halaman pembuka aplikasi yang menampilkan identitas aplikasi sebelum pengguna masuk ke halaman utama.

---

## 2. Dashboard

Dashboard merupakan halaman utama aplikasi yang digunakan sebagai pusat navigasi menuju seluruh menu aplikasi.

---

## 3. Master Barang

Menu ini digunakan untuk mengelola data barang habis pakai.

Fitur yang tersedia:

- Menambah data barang.
- Mengubah data barang.
- Menghapus data barang.
- Menambahkan foto barang.
- Menampilkan stok gudang pusat.

Data barang terdiri dari:

- Kode Barang
- Nama Barang
- Merek
- Tipe
- Satuan
- Stok Gudang
- Foto Barang

---

## 4. Master Lokasi

Digunakan untuk menyimpan data lokasi atau UKPD tujuan distribusi barang.

Data yang disimpan meliputi:

- Kode Lokasi
- Nama Lokasi
- Alamat

---

## 5. Barang Masuk

Menu Barang Masuk digunakan untuk mencatat setiap barang yang masuk ke gudang pusat sehingga stok barang akan bertambah secara otomatis.

Data transaksi meliputi:

- Barang
- Jumlah
- Tanggal
- Keterangan

---

## 6. Barang Keluar

Menu Barang Keluar digunakan untuk mendistribusikan barang dari gudang pusat menuju lokasi atau UKPD.

Fitur yang tersedia:

- Memilih barang.
- Memilih lokasi tujuan.
- Mengisi jumlah distribusi.
- Menentukan tanggal distribusi.
- Upload Berita Acara.
- Menambahkan keterangan.

Sistem akan melakukan validasi stok sehingga jumlah barang yang didistribusikan tidak melebihi stok yang tersedia.

---

## 7. Detail Barang

Halaman Detail Barang digunakan untuk melihat informasi lengkap suatu barang.

Informasi yang ditampilkan meliputi:

- Foto Barang
- Kode Barang
- Nama Barang
- Merek
- Tipe
- Satuan
- Jumlah Stok
- Riwayat Barang Masuk
- Riwayat Barang Keluar

---

# Struktur Database

Aplikasi menggunakan SQLite sebagai media penyimpanan data.

Database terdiri dari beberapa tabel utama.

## Tabel Barang

| Field |
|--------|
| id |
| kode_barang |
| nama |
| merek |
| tipe |
| satuan |
| stok_pusat |
| foto_path |

---

## Tabel Lokasi

| Field |
|--------|
| id |
| kode_lokasi |
| nama |
| alamat |

---

## Tabel Barang Masuk

| Field |
|--------|
| id |
| barang_id |
| jumlah |
| tanggal |
| user_id |
| keterangan |

---

## Tabel Barang Keluar

| Field |
|--------|
| id |
| barang_id |
| lokasi_id |
| jumlah |
| tanggal |
| berita_acara_path |
| user_id |
| keterangan |

---

# Persyaratan Sistem

## Software

- Flutter SDK
- Dart SDK
- Android Studio
- Visual Studio Code
- Android SDK

## Hardware

Minimal spesifikasi:

- RAM 4 GB
- Storage 2 GB
- Android 8.0 atau lebih baru

---

# Cara Instalasi

1. Clone atau ekstrak project.

2. Masuk ke folder project.

3. Jalankan perintah berikut.

```bash
flutter pub get
```

4. Pastikan emulator Android atau perangkat Android sudah terhubung.

5. Jalankan aplikasi.

```bash
flutter run
```

---

# Cara Menggunakan Aplikasi

### Menambah Barang

1. Pilih menu **Barang**.
2. Tekan tombol **Tambah**.
3. Isi data barang.
4. Simpan.

---

### Menambah Lokasi

1. Pilih menu **Lokasi**.
2. Tekan tombol **Tambah Lokasi**.
3. Isi data lokasi.
4. Simpan.

---

### Barang Masuk

1. Pilih menu **Barang Masuk**.
2. Pilih barang.
3. Masukkan jumlah barang.
4. Pilih tanggal.
5. Tambahkan keterangan jika diperlukan.
6. Simpan transaksi.

---

### Barang Keluar

1. Pilih menu **Barang Keluar**.
2. Pilih barang.
3. Pilih lokasi tujuan.
4. Masukkan jumlah distribusi.
5. Upload berita acara.
6. Tambahkan keterangan.
7. Simpan transaksi.

---

### Melihat Detail Barang

1. Pilih salah satu barang.
2. Halaman detail akan menampilkan:

- Informasi barang
- Foto barang
- Jumlah stok
- Riwayat transaksi masuk
- Riwayat transaksi keluar

---

# Struktur Folder Project

```
lib
│
├── models
├── screens
├── services
├── widgets
├── utils
├── database_helper.dart
├── app_theme.dart
└── main.dart

assets

android

ios
```

---

# Dokumentasi Tampilan

Dokumentasi screenshot aplikasi yang disarankan:

- Splash Screen
- Dashboard
- Master Barang
- Tambah Barang
- Detail Barang
- Master Lokasi
- Barang Masuk
- Barang Keluar
- Riwayat Barang
- Monitoring Stok

---

# Pengujian

Aplikasi telah diuji menggunakan metode Black Box Testing.

Pengujian dilakukan terhadap seluruh fitur utama aplikasi, antara lain:

- Login (jika diterapkan)
- Dashboard
- Tambah Barang
- Edit Barang
- Hapus Barang
- Barang Masuk
- Barang Keluar
- Upload Berita Acara
- Monitoring Stok
- Riwayat Barang

Seluruh fungsi utama dapat berjalan sesuai dengan kebutuhan pengguna.

---

# Kelebihan Aplikasi

- Tampilan sederhana dan mudah digunakan.
- Berjalan secara offline.
- Menggunakan database SQLite.
- Tidak memerlukan koneksi internet.
- Memiliki riwayat transaksi barang.
- Mendukung upload foto barang.
- Mendukung upload berita acara distribusi.
- Monitoring stok dilakukan secara otomatis.

---

# Kekurangan Aplikasi

- Belum mendukung sinkronisasi data secara online.
- Belum memiliki fitur backup database.
- Belum mendukung multi-user.
- Belum tersedia export laporan ke PDF maupun Excel.

---

# Pengembangan Selanjutnya

Beberapa pengembangan yang dapat dilakukan pada versi berikutnya antara lain:

- Integrasi dengan server.
- Sinkronisasi cloud database.
- Login multi-user.
- Hak akses administrator.
- Dashboard statistik.
- Export laporan PDF.
- Export Excel.
- Notifikasi stok minimum.
- Backup dan Restore Database.
- Integrasi QR Code Barang.

---

# Penulis

**Nama :** Grafica Jati Sugiyarto

**NIM :** 1135170135

**Program Studi :** Teknik Informatika

**Konsentrasi :** Software Engineering

**Perguruan Tinggi :** Institut Teknologi dan Bisnis Bina Sarana Global

**Tahun :** 2026

---

# Lisensi

Aplikasi ini dikembangkan sebagai Project 3 Program Studi Teknik Informatika Konsentrasi Software Engineering Institut Teknologi dan Bisnis Bina Sarana Global.

Aplikasi digunakan sebagai media implementasi pencatatan dan pengelolaan barang habis pakai di lingkungan Sudis Kominfotik Jakarta Barat.