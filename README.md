# Aplikasi Kasir Fullstack - Flutter (Mobile) + Laravel (Backend)

![POS System](https://img.shields.io/badge/POS-System-blue)
![Frontend Flutter](https://img.shields.io/badge/Frontend-Flutter-blue)
![Backend Laravel](https://img.shields.io/badge/Backend-Laravel-red)

Aplikasi kasir point-of-sale (POS) fullstack dengan Flutter sebagai frontend mobile dan Laravel sebagai backend API.

## 📋 Fitur Utama

- ✅ Manajemen Produk
- ✅ Kategori Produk
- ✅ Transaksi Penjualan
- ✅ Laporan Penjualan

## 🚀 Panduan Instalasi

### 📦 Backend (Laravel)

1. Masuk ke folder backend:

   ```bash
   cd laravel-pos-backend
   ```

2. Install dependencies:

   ```bash
   composer install
   ```

3. Setup environment:

   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Konfigurasi database di file `.env`:

   ```env
   DB_DATABASE=nama_database_anda
   DB_USERNAME=username_db
   DB_PASSWORD=password_db
   ```

5. Jalankan migrasi dan seeder:

   ```bash
   php artisan migrate --seed
   ```

6. Buat symbolic link untuk storage:

   ```bash
   php artisan storage:link
   ```

7. Jalankan server:
   ```bash
   php artisan serve --host=IP.ANDA --port=8000
   ```

**User default untuk testing:**

- Email: `irfan@gmail.com`
- Password: `12345678`

### 📱 Frontend (Flutter)

1. Masuk ke folder frontend:

   ```bash
   cd flutter_pos_app
   ```

2. Install dependencies:

   ```bash
   flutter pub get
   ```

3. Konfigurasi alamat API:  
   Buka file `lib/core/constants/variable.dart` dan sesuaikan isinya:

   ```dart
   const String baseUrl = "http://IP-ANDA:8000";
   ```

4. Jalankan aplikasi:
   ```bash
   flutter run
   ```

## 🌟 Dukungan Anda Sangat Berarti!

Tertarik dengan proyek ini dan ingin melihatnya terus berkembang? Anda bisa memberikan dukungan dengan menjadi sponsor. Kontribusi Anda akan sangat membantu dalam pengembangan dan pemeliharaan proyek ini.

[![Dukung Saya](https://img.shields.io/badge/-Dukung%20Saya-blue?style=for-the-badge)](https://saweria.co/anandairfansyah)

Terima kasih telah mendukung karya ini! Bersama, kita bisa menciptakan sesuatu yang luar biasa. 🚀
