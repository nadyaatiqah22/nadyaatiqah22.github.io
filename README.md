# 🛍️ Website Toko Pakaian Online

Sistem berbasis web yang dirancang untuk memudahkan proses penjualan produk pakaian secara online. Sistem ini bertujuan untuk mengotomatisasi berbagai aktivitas bisnis seperti pengelolaan produk, pemesanan, pembayaran, dan pelacakan pesanan.

---

## 👥 Anggota Tim

| Nama | NIM |
| :--- | :--- |
| **Nadya Atiqah Adha** | 23050974080 |
| **Teresa Panggabean** | 23050974081 |
| **Afifah Nur Hidayanti** | 23050974108 |
| **Fairuz Salsabila** | 23050974109 |

---

## 🔗 Demo Aplikasi

Akses aplikasi melalui link berikut:
**[🌐 Link Website (Railway)](https://tester-production-83cd.up.railway.app/)**

> **Catatan Penting:** ⚠️ Jika website tidak memuat sempurna atau blank saat pertama kali dibuka, mohon **Refresh halaman sebanyak 2x**. Hal ini mungkin terjadi karena *cold start* pada server deployment.

---

## 🎯 Tujuan Program

1.  **Solusi Digital:** Menyediakan platform digital untuk proses jual beli pakaian secara online yang modern.
2.  **Manajemen Efisien:** Mempermudah pengelolaan produk, transaksi, dan pengguna melalui fitur CRUD (Create, Read, Update, Delete).
3.  **Otomatisasi:** Meningkatkan efisiensi layanan toko melalui dashboard admin dan sistem otomatisasi status pesanan.

---

## 💻 Tech Stack

* **Framework:** Laravel
* **Bahasa:** PHP
* **Database:** MySQL
* **Frontend:** Blade / Bootstrap / Tailwind (Sesuaikan dengan yang dipakai)
* **Deployment:** Railway

---

## 👥 Aktor Pengguna

Sistem ini membagi akses menjadi dua aktor utama:

1.  **Admin / Pemilik Toko**
    * Mengelola data master (produk, kategori, stok).
    * Memantau pesanan masuk dan verifikasi pembayaran.
    * Melihat laporan penjualan.
2.  **Pelanggan**
    * Melihat katalog produk.
    * Melakukan transaksi pembelian (Checkout).
    * Melacak status pesanan dan riwayat pembelian.

---

## 📋 Daftar Fitur & Fungsionalitas

Berikut adalah daftar lengkap fitur berdasarkan pemetaan *Use Case* (UC):

| ID Fitur | Deskripsi Fitur | Kode UC |
| :--- | :--- | :--- |
| **Akun & Profil** | | |
| F00 | Registrasi Akun | UC01 |
| F01 | Login | UC02 |
| F02 | Logout | UC03 |
| F03 | Edit Profil | UC04 |
| F19 | Kelola Data Pengguna (Admin) | UC20 |
| **Manajemen Produk** | | |
| F04 | Lihat Daftar Produk | UC05 |
| F05 | Lihat Detail Produk | UC06 |
| F15 | Tambah Produk (Admin) | UC16 |
| F16 | Edit Produk (Admin) | UC17 |
| F17 | Hapus Produk (Admin) | UC18 |
| F18 | Kelola Kategori Produk | UC19 |
| F29 | Update Stok Manual | UC30 |
| **Transaksi & Keranjang** | | |
| F06 | Tambah ke Keranjang | UC07 |
| F07 | Update Jumlah di Keranjang | UC08 |
| F08 | Hapus Produk dari Keranjang | UC09 |
| F09 | Checkout | UC10 |
| F10 | Masukkan Alamat Pengiriman | UC11 |
| F23 | Tambah Catatan saat Checkout | UC24 |
| F24 | Estimasi Ongkir | UC25 |
| F30 | Pilih Opsi Pengiriman | UC31 |
| **Pembayaran & Pesanan** | | |
| F11 | Pilih Metode Pembayaran | UC12 |
| F12 | Upload Bukti Pembayaran | UC13 |
| F27 | Kelola Bukti Pembayaran | UC28 |
| F13 | Lihat Transaksi Masuk | UC14 |
| F14 | Ubah Status Pesanan | UC15 |
| F22 | Batalkan Pesanan | UC23 |
| F26 | Lihat Status Pesanan Real-time | UC27 |
| F31 | Tolak Pembayaran Tidak Valid | UC32 |
| **Laporan & Layanan** | | |
| F20 | Lihat Laporan Penjualan | UC21 |
| F21 | Lihat Riwayat Pembelian | UC22 |
| F25 | Kirim Email Konfirmasi | UC26 |
| F28 | Rekomendasi Produk | UC29 |
| F32 | Lihat Komplain Pelanggan | UC33 |
| F33 | Tanggapi Komplain Pelanggan | UC34 |

---

## ⚙️ Cara Instalasi (Lokal)

Jika ingin menjalankan proyek ini di komputer lokal (Localhost):

1.  **Clone Repositori**
    ```bash
    git clone [https://github.com/username/nama-repo.git](https://github.com/username/nama-repo.git)
    ```
2.  **Install Dependencies**
    ```bash
    composer install
    npm install && npm run build
    ```
3.  **Setup Environment**
    * Duplikat file `.env.example` menjadi `.env`
    * Sesuaikan konfigurasi database (DB_DATABASE, dll)
4.  **Generate Key & Migrasi**
    ```bash
    php artisan key:generate
    php artisan migrate --seed
    ```
5.  **Jalankan Server**
    ```bash
    php artisan serve
    ```

---

*Dibuat untuk memenuhi tugas Proyek Pengembangan Perangkat Lunak.*
