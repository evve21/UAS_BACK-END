 UAS Back-End Development

 👨‍💻 Pembuat Proyek
Proyek ini dibuat oleh empat mahasiswa sebagai bagian dari tugas UAS Back-End Development:

1. [Dunstan Devon] – [220040009]  
2. [Nama Lengkap 2] – [NIM 2]  
3. [Nama Lengkap 3] – [NIM 3]  
4. [Nama Lengkap 4] – [NIM 4]  

---

📦 Deskripsi Proyek
Repositori ini berisi kode back-end untuk proyek UAS yang menggunakan teknologi modern berbasis Node.js dan Express. Proyek ini dirancang untuk melayani API yang aman dan terstruktur dengan baik, cocok untuk pengembangan lebih lanjut.

---

 🚀 Cara Menjalankan Proyek

Ikuti langkah-langkah berikut untuk menjalankan proyek ini secara lokal:

🚀 Fitur Utama
   Login menggunakan token (JWT)
   Superadmin default otomatis dari SQL
   CRUD Data Mahasiswa (Create, Read, Update, Delete)
   Proteksi semua endpoint menggunakan token
   Middleware verifikasi token aktif
   Response dalam format JSON

🛠️ Tools
  PHP Native
  MySQL
  Composer (untuk JWT library)
  Apache (via Laragon)
  Postman (untuk pengujian)

🔐 Login Default
  Username	Password
  admin	admin123
  

🧪 Langkah Uji API dengan Postman
  Jalankan POST /api/auth/login
  Masukkan username & password
  Simpan token JWT dari response
  Tambahkan token ke header setiap request berikutnya:
  Header: Authorization: Bearer {token}
  Lanjutkan pengujian:
  GET /api/auth/me
  CRUD mahasiswa sesuai ID


💾 Cara Setup Project
  Extract ke: C:/laragon/www/BE_DEV/uas
  Jalankan composer install
  Buat database uas_db, lalu import database.sql
  Jalankan Laragon (Apache + MySQL)
  Akses project: http://localhost/uas
