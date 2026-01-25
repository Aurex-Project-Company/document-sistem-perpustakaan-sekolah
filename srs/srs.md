# SOFTWARE REQUIREMENTS SPECIFICATION

## SISTEM PERPUSTAKAAN SEKOLAH BERBASIS WEB

Versi: 1.1

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

Kebutuhan fungsional sistem disusun berdasarkan **Use Case Diagram** yang telah ditentukan, dengan aktor utama **Admin/Petugas Perpustakaan** dan **Anggota Perpustakaan (Siswa dan Guru)**.

### **Kebutuhan Fungsional Admin / Petugas Perpustakaan**

### **Manajemen Data Siswa**

- Sistem menyediakan fitur untuk menambah, mengubah, menghapus, dan melihat data siswa
- Data siswa meliputi NIS, nama siswa, jenis kelamin, dan alamat

### **Manajemen Data Guru**

- Sistem menyediakan fitur untuk menambah, mengubah, menghapus, dan melihat data guru
- Data guru meliputi NIP, nama guru, alamat, dan nomor kontak

### **Manajemen Data Anggota**

- Sistem menyediakan fitur untuk mendaftarkan anggota perpustakaan
- Sistem mengelola jenis anggota (siswa atau guru)

### **Manajemen Data Kelas**

- Sistem menyediakan fitur untuk mengelola data kelas
- Data kelas meliputi nama kelas dan tingkat

### **Manajemen Tahun Ajar**

- Sistem menyediakan fitur untuk mengelola data tahun ajar
- Sistem dapat menentukan tahun ajar aktif

### **Manajemen Riwayat Kelas**

- Sistem menyediakan fitur untuk mencatat riwayat kelas siswa setiap tahun ajar
- Sistem mengaitkan data siswa, kelas, dan tahun ajar

### **Manajemen Data Buku**

- Sistem menyediakan fitur untuk menambah, mengubah, menghapus, dan melihat data buku
- Data buku meliputi judul, pengarang, penerbit, tahun terbit, kategori, dan stok

### **Manajemen Kategori Buku**

- Sistem menyediakan fitur untuk menambah, mengubah, menghapus, dan melihat kategori buku

### **Transaksi Peminjaman Buku**

- Sistem menyediakan fitur pencatatan peminjaman buku oleh anggota
- Sistem memvalidasi ketersediaan stok buku sebelum peminjaman
- Sistem menyimpan tanggal pinjam dan tanggal jatuh tempo

### **Transaksi Pengembalian Buku**

- Sistem menyediakan fitur pencatatan pengembalian buku
- Sistem menghitung denda keterlambatan secara otomatis
- Sistem memperbarui status peminjaman dan stok buku

### **Laporan**

- Sistem menyediakan laporan peminjaman buku
- Sistem menyediakan laporan pengembalian buku
- Sistem menyediakan laporan denda

### **Kebutuhan Fungsional Anggota (Siswa dan Guru)**

### **Melihat Katalog Buku**

- Anggota dapat melihat daftar dan detail buku yang tersedia di perpustakaan

---

## **Kebutuhan Non-Fungsional**

### **Kebutuhan Perangkat Lunak**

- Web server (Apache/Nginx)
- Database server (MySQL/PostgreSQL)
- Browser modern (Chrome, Firefox)

### **Kebutuhan Perangkat Keras**

- Server minimal RAM 4 GB
- Komputer client dengan koneksi internet
