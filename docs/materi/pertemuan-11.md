---
sidebar_label: "Pertemuan 11: Laravel 2 (Migration Seeder Factory) & Authentication"
sidebar_position: 10
Path: docs/materi/pertemuan-10
---

# Pertemuan 11: Laravel 2 (Migration Seeder Factory) & Authentication

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## 1. Migration
Migration adalah fitur Laravel yang memungkinkan kita mengelola versi skema database menggunakan kode PHP. Setiap perubahan struktur database ditulis dalam file migration, sehingga pengelolaan skema database menjadi lebih terstruktur, terdokumentasi, dan bisa dikontrol versi-nya.

### Kelebihan Menggunakan Migration
- Menghindari inkonsistensi struktur database.
- Dapat digunakan oleh tim secara kolaboratif.
- Bisa rollback jika ada kesalahan pada struktur.
- Dapat diatur menggunakan version control seperti Git.

### Perintah Dasar

```bash
php artisan make:migration create_users_table
php artisan migrate
php artisan migrate:rollback
```

### Contoh Migration

```php
// database/migrations/xxxx_xx_xx_create_products_table.php
public function up()
{
    Schema::create('products', function (Blueprint $table) {
        $table->id();
        $table->string('name');
        $table->double('price');
        $table->timestamps();
    });
}
```

---

## 2. Seeder & Factory

### Pengertian

- **Seeder**: Digunakan untuk mengisi data awal atau data dummy ke dalam tabel database. Cocok untuk testing dan pengembangan.
- **Factory**: Menghasilkan data dummy secara otomatis dengan atribut acak berdasarkan template yang ditentukan, menggunakan library Faker.

### Kelebihan
- Menghemat waktu input manual saat testing.
- Dapat mengisi database dalam jumlah besar.
- Dapat digunakan pada CI/CD pipeline.

### Langkah-langkah

#### a. Membuat Factory

```bash
php artisan make:factory ProductFactory --model=Product
```

```php
// database/factories/ProductFactory.php
public function definition()
{
    return [
        'name' => $this->faker->word(),
        'price' => $this->faker->randomFloat(2, 1000, 100000),
    ];
}
```

#### b. Membuat Seeder

```bash
php artisan make:seeder ProductSeeder
```

```php
// database/seeders/ProductSeeder.php
public function run()
{
    \App\Models\Product::factory(10)->create();
}
```

#### c. Menjalankan Seeder

```bash
php artisan db:seed --class=ProductSeeder
```

#### d. Menjalankan Semua Seeder

Tambahkan ke `DatabaseSeeder.php`:

```php
public function run()
{
    $this->call(ProductSeeder::class);
}
```

Jalankan:

```bash
php artisan db:seed
```

---

## 3. Authentication

### A. Auth Secara Manual (Vanilla Laravel)

Laravel dapat menangani otentikasi secara manual tanpa menggunakan starter kit seperti Breeze atau UI. Berikut adalah langkah-langkahnya:

#### 1. Migration dan Model User

Pastikan tabel `users` sudah tersedia dari default Laravel.

```php
// users table migration (default)
$table->string('name');
$table->string('email')->unique();
$table->timestamp('email_verified_at')->nullable();
$table->string('password');
```

#### 2. Routing

Tambahkan route login, register, dan logout:

```php
// routes/web.php

use App\Http\Controllers\AuthController;

Route::get('/register', [AuthController::class, 'showRegisterForm']);
Route::post('/register', [AuthController::class, 'register']);

Route::get('/login', [AuthController::class, 'showLoginForm'])->name('login');
Route::post('/login', [AuthController::class, 'login']);

Route::post('/logout', [AuthController::class, 'logout'])->name('logout');
```

#### 3. Controller

```bash
php artisan make:controller AuthController
```

```php
// app/Http/Controllers/AuthController.php

use App\Models\User;
use Illuminate\Http\Request;
use Illuminate\Support\Facades\Auth;
use Illuminate\Support\Facades\Hash;

class AuthController extends Controller
{
    public function showRegisterForm()
    {
        return view('auth.register');
    }

    public function register(Request $request)
    {
        $request->validate([
            'name' => 'required',
            'email' => 'required|email|unique:users',
            'password' => 'required|min:6|confirmed',
        ]);

        User::create([
            'name' => $request->name,
            'email' => $request->email,
            'password' => Hash::make($request->password),
        ]);

        return redirect('/login');
    }

    public function showLoginForm()
    {
        return view('auth.login');
    }

    public function login(Request $request)
    {
        $credentials = $request->only('email', 'password');

        if (Auth::attempt($credentials)) {
            $request->session()->regenerate();
            return redirect()->intended('/dashboard');
        }

        return back()->withErrors([
            'email' => 'Login gagal. Periksa kembali email dan password.',
        ]);
    }

    public function logout(Request $request)
    {
        Auth::logout();
        $request->session()->invalidate();
        $request->session()->regenerateToken();
        return redirect('/login');
    }
}
```

#### 4. View Blade

Buat folder `resources/views/auth` dan tambahkan dua file:

- `login.blade.php`
- `register.blade.php`

Isi sederhana:

```blade
<!-- resources/views/auth/login.blade.php -->
<form method="POST" action="/login">
    @csrf
    <input name="email" type="email" placeholder="Email">
    <input name="password" type="password" placeholder="Password">
    <button type="submit">Login</button>
</form>
```

```blade
<!-- resources/views/auth/register.blade.php -->
<form method="POST" action="/register">
    @csrf
    <input name="name" type="text" placeholder="Name">
    <input name="email" type="email" placeholder="Email">
    <input name="password" type="password" placeholder="Password">
    <input name="password_confirmation" type="password" placeholder="Confirm Password">
    <button type="submit">Register</button>
</form>
```

#### 5. Proteksi Halaman

Gunakan middleware `auth`:

```php
Route::get('/dashboard', function () {
    return view('dashboard');
})->middleware('auth');
```

---

### B. Starter Kit (Breeze, UI, Jetstream)

Laravel juga menyediakan starter kit otentikasi yang siap pakai untuk mempercepat pengembangan.

#### Laravel Breeze

##### Instalasi

```bash
composer require laravel/breeze --dev
php artisan breeze:install
npm install && npm run dev
php artisan migrate
```

##### Jalankan Server

```bash
php artisan serve
```

Akses:
- `http://localhost:8000/register`
- `http://localhost:8000/login`

#### Laravel UI (Alternatif)

```bash
composer require laravel/ui
php artisan ui bootstrap --auth
npm install && npm run dev
php artisan migrate
```

---

## Referensi

- [Laravel Migrations](https://laravel.com/docs/migrations)
- [Laravel Seeding](https://laravel.com/docs/seeding)
- [Laravel Authentication](https://laravel.com/docs/starter-kits)
- [Laravel Manual Auth](https://laravel.com/docs/authentication)

---
