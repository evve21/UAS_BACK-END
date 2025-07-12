 UAS Back-End Development

 👨‍💻 Pembuat Proyek
Proyek ini dibuat oleh empat mahasiswa sebagai bagian dari tugas UAS Back-End Development:

[Dunstan Devon] – [220040009]
[James Muda Rido] – [230040158]
[Kshatria Do Fachoi ZIDUHU Wau] – [230040135]


 📦 Deskripsi Proyek
Repositori ini berisi kode back-end menggunakan PHP Native untuk menangani API otentikasi dan manajemen data mahasiswa. API ini menggunakan JWT (JSON Web Token) untuk autentikasi, serta menerapkan proteksi middleware pada setiap endpoint.

 🚀 Fitur Utama

✅ Login menggunakan token (JWT)  
✅ Superadmin default dari SQL (admin/admin123)  
✅ CRUD Data Mahasiswa (Create, Read, Update, Delete)  
✅ Proteksi semua endpoint menggunakan token  
✅ Middleware verifikasi token aktif  
✅ Response seluruhnya dalam format JSON  

 🛠️ Teknologi yang Digunakan

PHP Native  
MySQL  
Composer (untuk instalasi library JWT)  
Apache (via Laragon)  
Postman (untuk pengujian API)  

 🔐 Login Default

Username: admin  
Password: admin123  

 💾 Cara Setup Proyek

1. Ekstrak folder ZIP ke path berikut:  
   C:/laragon/www/BE_DEV/uas

2. Instal dependensi menggunakan Composer:  
   composer install

3. Buat database baru di MySQL:  
   uas_db

4. Import file database.sql ke database uas_db

5. Jalankan Laragon (aktifkan Apache dan MySQL)

6. Akses API di browser atau Postman:  
   http://localhost/uas

 🧪 Panduan Uji API (via Postman)

1. Login untuk mendapatkan JWT:  
   Endpoint: POST /api/auth/login  
   Body (raw JSON):  
   {
     "username": "admin",
     "password": "admin123"
   }

2. Simpan token dari response. Tambahkan ke setiap request selanjutnya:  
   Header: Authorization: Bearer {token}

3. Contoh endpoint lainnya:  
   GET /api/auth/me  
   GET /api/mahasiswa  
   POST /api/mahasiswa  
   PUT /api/mahasiswa/{id}  
   DELETE /api/mahasiswa/{id}  

 📁 Struktur Direktori (Singkat)

uas/
├── api/
│   ├── auth/
│   └── mahasiswa/
├── config/
├── middleware/
├── database.sql
├── composer.json
└── index.php


