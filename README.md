🔧 Backend (Laravel API)
RESTful API untuk manajemen data User.

✅ Fitur Utama
Full CRUD untuk entitas User

Validasi input lengkap

Terhubung ke database MySQL

📌 Validasi Input

| Field          | Tipe    | Validasi                    |
| -------------- | ------- | --------------------------- |
| `nama`         | string  | required, max:255           |
| `email`        | string  | required, valid email, unik |
| `nomorTelepon` | string  | required, 10–15 digit angka |
| `statusAktif`  | boolean | required                    |
| `departemen`   | string  | required, max:100           |

🛠️ Cara Menjalankan di Lokal

# 1. Clone repository
git clone https://github.com/abdulrouff10/rouf-backend.git

# 2. Masuk ke folder proyek
cd rouf-backend

# 3. Install dependency
composer install

# 4. Salin file .env dan generate APP_KEY
cp .env.example .env
php artisan key:generate

# 5. Edit konfigurasi database di file .env

# 6. Jalankan migrasi
php artisan migrate

# 7. Jalankan server
php artisan serve
