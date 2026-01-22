# UAS-Pemrograman-Web: Inventaris Pro 

**NAMA                : RAFI UBAYDILLAH**
**NIM                 : 312410542**
**KELAS               : TI.24.A.5**
**MATKUL              : PEMROGRAMAN WEB 1**

---

## Deskripsi Singkat
Aplikasi **Inventaris Pro** adalah sistem manajemen stok barang berbasis web yang dibangun menggunakan **PHP Native** dengan arsitektur **OOP (Object Oriented Programming)**. Aplikasi ini dirancang secara **Modular** dan menggunakan **Routing App (.htaccess)** untuk pengelolaan URL yang bersih dan profesional.

---

## Fitur Utama (Sesuai Kriteria UAS)
- **Login Multi-Role**: Sistem autentikasi yang membedakan hak akses antara `Admin` (akses penuh) dan `User` (hanya melihat data).
- **CRUD (Create, Read, Delete)**: Fitur pengelolaan data barang secara dinamis langsung ke database MySQL menggunakan PDO.
- **Filter Pencarian**: Fitur pencarian barang berdasarkan nama secara *real-time* untuk memudahkan pencarian data yang banyak.
- **Pagination**: Sistem pembatasan tampilan data per halaman agar performa aplikasi tetap ringan dan rapi.
- **Responsive & Modern Design**: Menggunakan **Bootstrap 5** dengan pendekatan *Mobile First* sehingga nyaman diakses dari smartphone maupun desktop.
- **Routing Clean URL**: Menggunakan file `.htaccess` sehingga navigasi halaman lebih rapi (contoh: `admin-dashboard` bukan `index.php?page=admin`).

---

## Teknologi yang Digunakan
- **PHP 8.x**: Menggunakan paradigma OOP (Class & Object) untuk struktur kode yang lebih rapi.
- **MySQL (PDO)**: Sebagai sistem database untuk menyimpan data user dan barang secara aman.
- **Bootstrap 5**: Digunakan untuk styling UI yang modern dan responsif.
- **Apache (.htaccess)**: Digunakan untuk menangani Routing App.

---

## Cara Menjalankan (Lokal)
1. **Persiapan Database**:
   - Buka `phpMyAdmin` dan buat database baru bernama `db_inventaris`.
   - Import file SQL yang tersedia (atau jalankan query yang ada di folder `config/`).
2. **Struktur Folder**: Pindahkan folder proyek `inventaris_uas/` ke direktori `C:/xampp/htdocs/`.
3. **Aktifkan Modul Rewrite**: Pastikan modul `mod_rewrite` pada Apache di XAMPP sudah dalam keadaan *Enable*.
4. **Akses Aplikasi**: Buka browser dan akses `http://localhost/inventaris_uas/`.
5. **Akun Login**:
   - Admin: `admin` / `admin123`
   - User: `user` / `user123`

---

## Struktur Folder Proyek (Modular)
```text
inventaris_uas/
├── config/             # Koneksi Database (Class Database)
├── controllers/        # Logika Bisnis (Proses Login & CRUD)
├── models/             # Query SQL OOP (Class User & Barang)
├── views/              # Tampilan (Layout, Auth, Admin, User)
├── public/             # File statis (CSS, JS, Gambar)
├── .htaccess           # File Routing
└── index.php           # Front Controller (Gerbang Utama)


Link Dokumentasi:
•	Link YouTube: https://youtu.be/ptd1VzhGiSw

