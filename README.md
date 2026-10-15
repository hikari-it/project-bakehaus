# Database System & Analytics - Bakehaus 🥐☕

**Mata Kuliah:** Database Technology (Assessment of Learning)
**Sektor Industri:** Small Medium Business (F&B)

---

## 📌 Deskripsi Proyek
Proyek ini bertujuan untuk membangun sistem *Point of Sale* (POS) dan *Dashboard Analytics* terintegrasi untuk UMKM "Bakehaus" di Malang. Sistem ini dirancang secara khusus untuk mengatasi berbagai kendala pada sistem kasir standar mereka saat ini, seperti ketidakmampuan menambahkan catatan kustom pesanan ("pedas", "no sugar"), sistem cetak struk dan nomor antrean yang masih manual, hingga pencatatan pesanan *Pre-Order* (PO) dari WhatsApp yang belum terintegrasi. 

## 👥 Anggota Tim & Peran
* **Adilla Berliana Febrianti** - System Analyst, UI/UX, & Front-end
* **Andre Wijaya** - Database Architect & Back-end 
* **Muhammad Maulana Aldiansyah (Didi)** - Database Implementation & Data Analytics

## ⚙️ Alur Sistem (System Flow)
Sistem ini menggunakan konsep *Role-based Access Control* dengan dua pintu masuk utama[cite: 1]:

**1. Sistem Kasir / POS (Front-end & Back-end Integration)**
* **Tipe Pesanan:** Kasir dapat memisahkan pemesanan menjadi *Dine-in*, *Takeaway*, atau pesanan *Delivery* dari WhatsApp.
* **Kustomisasi Pesanan:** Penambahan catatan khusus konsumen (misal: instruksi dapur) yang langsung terhubung ke *database*.
* **Payment Gateway:** Integrasi metode pembayaran melalui API (Sandbox Midtrans/Xendit) untuk simulasi pembayaran QRIS Dinamis.
* **Automasi Dapur:** Ketika pembayaran terkonfirmasi (berubah menjadi lunas di *database*), sistem otomatis memberikan instruksi *print* struk berisikan Nomor Antrean untuk dapur dan konsumen.

**2. Dashboard Admin & Analytics (Database & Query Implementation)**
* **Manajemen Master Data:** Admin dapat menambah menu, mengatur harga/promo, atau melakukan penutupan ketersediaan menu (Toggle) apabila bahan baku habis.
* **Laporan Analitik:** Sistem mengeksekusi *complex SQL queries* untuk menampilkan laporan langsung ke UI *dashboard* (misalnya: perbandingan omzet per shift kasir, daftar menu paling laris, dan efektivitas penggunaan promo).

---

## 📝 To-Do List (Berdasarkan Instruksi Proyek)

### Fase 1: Pra-Perancangan & Pengumpulan Data
- [ ] Meminta 1-2 sampel struk asli dari Bakehaus (*Un-normalized Form*).
- [ ] Menganalisis anomali data dan *Functional Dependencies* pada sampel data.

### Fase 2: Perancangan Database (Andre)
- [ ] Melakukan tahapan normalisasi: UNF -> 1NF -> 2NF -> 3NF.
- [ ] Mengevaluasi dan mempertimbangkan penerapan BCNF pada data 3NF beserta alasannya.
- [ ] Merancang Entity Relationship Diagram (ERD) dengan metode *Crow's foot* atau *Chen*.
- [ ] Memetakan ERD menjadi *Relational Schema*.

### Fase 3: Implementasi & Analitik Database (Didi)
- [ ] Menulis DDL (CREATE TABLE) di MySQL/PostgreSQL lengkap dengan *Primary Key*, *Foreign Key*, dan *Constraints* (`NOT NULL`, `UNIQUE`, `CHECK`, `DEFAULT`).
- [ ] Melakukan *Populate Table* dengan data *dummy* menggunakan perintah DML (`INSERT`).
- [ ] Membuat demonstrasi *Complex Query* menggunakan kombinasi `JOIN`, *Subquery/CTE*, dan *Aggregate / Window Functions* untuk analitik data Bakehaus.

### Fase 4: Pengembangan Aplikasi (Adilla & Andre)
- [ ] Desain prototipe UI/UX minimalis (Merah, Putih, Hitam).
- [ ] Implementasi Front-end (Layout POS Kasir dan Dashboard Analytics).
- [ ] Membangun logika Back-end (penghitungan transaksi, integrasi *endpoint* WA).
- [ ] QA & Testing: Memastikan input aplikasi dari *front-end* terekam sempurna ke *database* fisik tanpa error.

### Fase 5: Pelaporan & Demo
- [ ] Bab 1: Deskripsi kasus, UMKM mitra, dan identifikasi masalah.
- [ ] Bab 2: Deskripsi *dataset* dan potensi anomali.
- [ ] Bab 3: Langkah demi langkah implementasi normalisasi.
- [ ] Bab 4: Final ERD & pemetaan relasional.
- [ ] Bab 5: Implementasi SQL (DDL, DML) dan penjelasan *complex query*.
- [ ] Bab 6: Justifikasi pemilihan tipe *database* (*Relational/RDBMS*), menjelaskan perbandingan ACID vs BASE serta alasan di balik kebutuhan *Consistency* dalam aplikasi kasir/finansial.
- [ ] Bab 7: Kesimpulan.
- [ ] Mempersiapkan demo aplikasi secara *live* atau *recorded* (8-10 Menit).
