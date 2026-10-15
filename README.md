# Database System & Analytics - Bakehaus 🥐☕

**Mata Kuliah:** Database Technology (Assessment of Learning)  
**Sektor Industri:** Small Medium Business (F&B)

---

## 📌 Deskripsi Proyek
Proyek ini membangun sistem *Point of Sale* (POS) dan *Dashboard Analytics* terintegrasi untuk UMKM Bakehaus. Sistem dirancang untuk menggantikan alur kasir standar yang masih memiliki keterbatasan, dengan fokus utama pada kustomisasi catatan pesanan, otomatisasi antrean, manajemen stok menu, dan penyajian laporan analitik performa penjualan yang terpusat.

## 👥 Anggota Tim & Peran
* **Adilla Berliana Febrianti** - System Analyst, UI/UX, & Front-end
* **Andre Wijaya** - Database Architect & Back-end 
* **Muhammad Maulana Aldiansyah (Didi)** - Database Implementation & Data Analytics

---

## ✨ Fitur-Fitur Sistem

**1. Sistem Kasir (Point of Sale)**
* **Kustomisasi Pesanan:** Kolom input catatan khusus dari pelanggan (contoh: "pedas", "no sugar") yang akan langsung terhubung ke struk cetak dapur.
* **Manajemen Tipe Pesanan:** Pemisahan pencatatan transaksi untuk *Dine-in*, *Takeaway*, dan *Delivery* (termasuk pesanan *Pre-Order* via WhatsApp).
* **Automasi Antrean & Cetak Struk:** Sistem memberikan instruksi *print* otomatis beserta nomor order terstruktur segera setelah status pembayaran berubah menjadi lunas.
* **Integrasi Payment Gateway:** Simulasi pembayaran QRIS Dinamis menggunakan *environment Sandbox* (Midtrans/Xendit) untuk memproses penyelesaian transaksi secara sistem.

**2. Dashboard Admin & Analytics**
* **Manajemen Master Data:** Fitur untuk menambah, mengedit, dan mengatur harga menu/promo.
* **Toggle Ketersediaan Stok:** Kemampuan admin untuk menonaktifkan (*unavailable*) menu secara *real-time* apabila bahan baku habis di tengah hari operasional.
* **Laporan Analitik:** Visualisasi data transaksi yang mencakup omzet per shift kasir, daftar menu paling laris, dan tren efektivitas penggunaan promo.

---

## 📦 Output Proyek

1. **Dokumen Laporan (Report Chapter 1 - 7)**
   Laporan komprehensif yang berisi latar belakang masalah mitra, deskripsi dataset, dokumentasi tahap perancangan database (normalisasi & ERD), implementasi kode, hingga justifikasi pemilihan teknologi database.
2. **Prototipe & Source Code Aplikasi**
   Sistem POS dan *Dashboard Admin* (Front-end & Back-end) yang berfungsi, memiliki UI/UX minimalis (Merah, Hitam, Putih), dan terhubung penuh ke dalam *database*.
3. **Presentasi & Live Demo**
   Demonstrasi berdurasi 8-10 menit yang menampilkan skenario operasional sistem dari sisi kasir maupun admin, interaksi dengan *database*, dan sesi Q&A.

---

## 🗄️ Komponen & Tahapan Database

Proyek ini menerapkan perancangan *database* dari tahap mentah hingga implementasi fisik menggunakan *Relational Database Management System* (RDBMS), dengan tah
