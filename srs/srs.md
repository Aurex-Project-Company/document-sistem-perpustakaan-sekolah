# SOFTWARE REQUIREMENTS SPECIFICATION

## SISTEM PERPUSTAKAAN SEKOLAH BERBASIS WEB

Versi: 1.0

15 Januari 2026

---

## **Pendahuluan**

### **Tujuan**

Dokumen Software Requirements Specification (SRS) ini bertujuan untuk memberikan gambaran lengkap dan terstruktur mengenai kebutuhan perangkat lunak **Sistem Perpustakaan Sekolah Berbasis Web**. Dokumen ini menjadi acuan bagi pengembang, analis sistem, dan pihak sekolah dalam proses perancangan, pengembangan, pengujian, serta evaluasi sistem.

### **Ruang Lingkup**

Sistem Perpustakaan Sekolah Berbasis Web adalah aplikasi yang digunakan untuk mengelola seluruh aktivitas perpustakaan sekolah, meliputi pengelolaan data buku, anggota, transaksi peminjaman dan pengembalian, serta penyajian laporan perpustakaan secara terkomputerisasi.

### **Referensi**

- Dokumen contoh SRS Sistem Pembayaran SPP Sekolah Berbasis Web
- IEEE 830 Software Requirements Specification

---

## **Gambaran Umum Sistem**

### **Deskripsi Umum**

Sistem Perpustakaan Sekolah Berbasis Web adalah sistem informasi yang digunakan untuk membantu pengelolaan perpustakaan sekolah secara efektif dan efisien. Sistem ini menggantikan proses manual seperti pencatatan buku dan transaksi peminjaman dengan sistem terkomputerisasi yang terintegrasi.

### **Fungsi Utama Sistem**

- Mengelola data buku dan kategori buku
- Mengelola data anggota perpustakaan
- Mengelola transaksi peminjaman dan pengembalian buku
- Menghitung denda keterlambatan
- Menyediakan laporan perpustakaan

### **Karakteristik Pengguna**

<table><tbody><tr><td><strong>No</strong></td><td><strong>Pengguna</strong></td><td><strong>Deskripsi</strong></td></tr><tr><td>1</td><td>Admin / Petugas</td><td>Mengelola seluruh data dan transaksi perpustakaan</td></tr><tr><td>2</td><td>Anggota (Siswa/Guru)</td><td>Melihat katalog buku</td></tr></tbody></table>

### **Batasan Sistem**

- Sistem berbasis web
- Digunakan dalam lingkup satu sekolah
- Tidak mencakup integrasi dengan sistem eksternal
- Tidak mencakup e-book atau peminjaman digital

---

## **Kebutuhan Fungsional**

### **Manajemen Pengguna**

- Sistem menyediakan fitur login dan logout
- Admin dapat mengelola data akun pengguna

### **Manajemen Data Buku**

- Admin dapat menambah, mengubah, menghapus, dan melihat data buku
- Data buku meliputi: kode buku, judul, pengarang, penerbit, tahun terbit, kategori, dan stok

### **Manajemen Kategori Buku**

- Admin dapat mengelola kategori buku
- Kategori digunakan untuk pengelompokan buku

### **Manajemen Anggota**

- Admin dapat mengelola data anggota perpustakaan
- Data anggota meliputi: nomor anggota, nama, jenis anggota, kelas (jika siswa), dan alamat

### **Transaksi Peminjaman Buku**

- Admin mencatat transaksi peminjaman buku
- Sistem menyimpan tanggal pinjam dan tanggal jatuh tempo
- Sistem mengurangi stok buku secara otomatis

### **Transaksi Pengembalian Buku**

- Admin mencatat pengembalian buku
- Sistem menghitung denda keterlambatan jika ada
- Sistem menambah stok buku

### **Laporan**

- Laporan data buku
- Laporan peminjaman
- Laporan pengembalian
- Laporan denda

---

## **Kebutuhan Non-Fungsional**

### **Kebutuhan Perangkat Lunak**

- Web server (Apache/Nginx)
- Database server (MySQL/PostgreSQL)
- Browser modern (Chrome, Firefox)
