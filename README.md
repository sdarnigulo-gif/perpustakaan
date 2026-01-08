# Perpustakaan - Library Management System

Sebuah sistem manajemen perpustakaan berbasis Laravel untuk mengelola koleksi buku, anggota, dan peminjaman.

## Fitur Utama

- Manajemen Buku
- Manajemen Anggota
- Sistem Peminjaman dan Pengembalian
- Laporan dan Statistik
- Dashboard Admin

## Persyaratan Sistem

- PHP >= 8.1
- Composer
- MySQL 5.7+
- Node.js & NPM (untuk frontend assets)

## Instalasi

### 1. Clone Repository

```bash
git clone https://github.com/sdarnigulo-gif/perpustakaan.git
cd perpustakaan
```

### 2. Install Dependencies

```bash
composer install
npm install
```

### 3. Konfigurasi Environment

```bash
cp .env.example .env
php artisan key:generate
```

Edit file `.env` dan sesuaikan konfigurasi database:

```env
DB_DATABASE=perpustakaan
DB_USERNAME=root
DB_PASSWORD=your_password
```

### 4. Jalankan Migrasi Database

```bash
php artisan migrate
```

### 5. Seed Database (Opsional)

```bash
php artisan db:seed
```

### 6. Kompilasi Assets

```bash
npm run dev
```

### 7. Jalankan Server

```bash
php artisan serve
```

Akses aplikasi di `http://localhost:8000`

## Struktur Direktori

```
perpustakaan/
├── app/
│   ├── Http/
│   │   ├── Controllers/
│   │   ├── Middleware/
│   │   └── Requests/
│   ├── Models/
│   └── Services/
├── database/
│   ├── migrations/
│   ├── seeders/
│   └── factories/
├── resources/
│   ├── views/
│   ├── css/
│   └── js/
├── routes/
│   ├── web.php
│   └── api.php
├── storage/
├── public/
├── tests/
├── vendor/
├── .env.example
├── composer.json
├── package.json
└── README.md
```

## Pengembangan

### Database Migration

```bash
php artisan make:migration create_[table_name]_table
php artisan migrate
```

### Membuat Model

```bash
php artisan make:model [ModelName]
```

### Membuat Controller

```bash
php artisan make:controller [ControllerName]
```

## Testing

```bash
php artisan test
```

## Kontribusi

Silakan fork repository ini dan submit pull request dengan deskripsi yang jelas.

## Lisensi

MIT License. Silakan lihat file LICENSE untuk detail lebih lanjut.

## Kontak

Untuk pertanyaan atau saran, silakan buat issue di repository ini.
