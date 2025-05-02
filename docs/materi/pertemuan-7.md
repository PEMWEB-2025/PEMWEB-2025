---
sidebar_label: "Pertemuan 7: PHP Native & Database MySQL"
sidebar_position: 7
Path: docs/materi/pertemuan-7
---

# Pertemuan 7: PHP Native & Database MySQL

## Pengenalan PHP 

- PHP singkatan dari PHP : Hypertext Preprocessor
- PHP banyak digunakan sebagai bahasa pemrograman yang dikhususkan untuk web development
- PHP sangat mudah digunakan dan banyak sekali diadopsi oleh programmer web
- Bahkan hampir mayoritas kebanyakan web di dunia dibuat menggunakan PHP
- PHP pertama kali dibuat oleh Rasmus Lerdorf pada tahun 1995

<br></br>
## Penulisan Kode PHP

Kode PHP ditulis di antara tag `<?php ... ?>`. Sebagai contoh:
```
<?php
echo "Hello World!";
?>
```

<br></br>
## Variabel & Tipe Data

### Variabel

Variabel pada kode PHP ditandai dengan tanda `$`. Contoh deklarasi variabel pada PHP:
```
$nama = "Budi";
echo $nama;
```

### Tipe Data

Tipe data pada variabel PHP dapat berupa teks (string), angka (integer), benar/salah (boolean), dll.
Contohnya:

```
$umur = 25; // integer
$nama = "Ayu"; // string
$aktif = true; // boolean
```

<br></br>
## Kondisi 

### IF, ELSE, dan ELSEIF

Bentuk umum dari `if` adalah sebagai berikut:
```
if (kondisi) {
    // kode yang dijalankan jika kondisi benar
} else {
    // kode yang dijalankan jika kondisi salah
}
```

<br></br>
`if` tidak harus selalu berpasangan dengan `else`. Kamu bisa menggunakan `if` saja tanpa harus mencantumkan `else`. Sebagai contoh:
```
$umur = 17;

if ($umur >= 18) {
    return ('Kamu Belum Cukup Umur');
}

echo "Kamu punya akses!"
```

<br></br>
Jika kamu memiliki beberapa kondisi, kamu bisa menggunakan `elseif`. Sebagai contoh:
```
$nilai = 75;

if ($nilai >= 90) {
    echo "Nilai A";
} elseif ($nilai >= 80) {
    echo "Nilai B";
} elseif ($nilai >= 70) {
    echo "Nilai C";
} else {
    echo "Nilai D";
}
```

### SWITCH, CASE

`switch case` juga termasuk dalam struktur kondisi di PHP, akan tetapi lebih cocok dipakai saat kamu punya banyak pilihan yang pasti nilainya.

Jika `if...else` cocok untuk kondisi beragam dan fleksibel, `switch case` cocok untuk kondisi yang nilainya tetap seperti angka atau string tertentu.

Contoh `switch case`:
```
$nilai = "B";

switch ($nilai) {
    case "A":
        echo "Sangat Baik";
        break;
    case "B":
        echo "Baik";
        break;
    case "C":
        echo "Cukup";
        break;
    default:
        echo "Nilai tidak dikenali";
}
```

<br></br>
## Perulangan (Loop)

Perulangan digunakan untuk menjalankan kode yang sama berulang kali, tanpa harus menulis ulang kodenya.

### Jenis-Jenis Perulangan

#### `for` Loop

Digunakan kalau kamu tahu berapa kali ingin mengulang. Contoh:
```
<?php
for ($i = 1; $i <= 5; $i++) {
    echo "Ini perulangan ke-$i <br>";
}
?>
```

#### `while` Loop

Digunakan ketika kamu tidak tahu pasti berapa kali harus mengulang, tapi tahu kondisinya. Contoh:
```
<?php
$i = 1;
while ($i <= 5) {
    echo "Angka: $i <br>";
    $i++;
}
?>
```

#### `do ... while` Loop

Mirip while, tapi kode dijalankan dulu minimal 1 kali, baru dicek kondisinya.
```
<?php
$i = 1;
do {
    echo "Nilai: $i <br>";
    $i++;
} while ($i <= 5);
?>
```

#### `foreach` 

Digunakan untuk mengulang isi dari array.
```
<?php
$buah = ["apel", "jeruk", "mangga"];

foreach ($buah as $item) {
    echo "Buah: $item <br>";
}
?>
```

<br></br>
## Function

Function adalah blok kode yang bisa kamu panggil berkali-kali. Daripada menulis ulang suatu kode, kamu bisa menuliskan kode yang ingin kamu gunakan berulang kali di dalam function, kemudian kamu cukup memanggil function itu aja. 

Berikut adalah bentuk dasar dari function:
```
function nama_fungsi() {
    // kode yang akan dijalankan
}

// Untuk memanggil function
nama_fungsi();
```

<br></br>
Contoh function sederhana:
```
function jumlah($a, $b) {
    return $a + $b;
}

$hasil = jumlah(5, 3);
echo $hasil;  // Output: 8
```

<br></br>
## MySQL

MySQL adalah tempat menyimpan data (seperti nama pengguna, email, dll).
Kalau kita analogikan, PHP itu adalah koki sedangkan MySQL itu lemari makanan. PHP akan "mengambil" dan "menyimpan" data dari/ke MySQL.

### Database

Database adalah sebuah tempat besar yang digunakan untuk menyimpan semua data. Dalam satu aplikasi biasanya punya satu database. Cara membuat database di MySQL:
```
CREATE DATABASE belajar_php;
```

### Tabel

Tabel memiliki struktur seperti lembar Excel: terdiri dari kolom dan baris. Tiap tabel dapat digunakan untuk menyimpan data tertentu (misalnya: tabel users  untuk simpan data pengguna). Cara membuat tabel di MySQL:
```
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nama VARCHAR(100),
    email VARCHAR(100),
    password VARCHAR(100)
);
```

### Kolom dan Tipe Data
Setiap kolom pasti mempunyai jenis data, contohnya:

- VARCHAR(100) = teks maksimal 100 karakter
- INT = angka bulat
- DATE = tanggal

### Foreign Key

Foreign key adalah kolom di satu tabel yang menghubungkan ke kolom PRIMARY KEY di tabel lain.
Analogi sederhananya seperti ini:

- Tabel users = daftar orang
- Tabel orders = daftar pesanan
- Di tabel `orders`, kita simpan user_id sebagai foreign key → agar tahu siapa yang mempunyai pesanan itu.

Contoh sederhana:

a. Membuat Tabel `users`
```
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nama VARCHAR(100)
);
```

b. Membuat Tabel `orders` Dengan Foreign Key `user_id`
```
CREATE TABLE orders (
    id INT AUTO_INCREMENT PRIMARY KEY,
    nama_produk VARCHAR(100),
    user_id INT,
    FOREIGN KEY (user_id) REFERENCES users(id)
);
```

c. Menambahkan Data ke Dalam Tabel
- Menambahkan data pengguna
```
INSERT INTO users (nama) VALUES ('Ari');
-- Misalnya id-nya 1
```
- Menambahkan data pesanan
```
INSERT INTO orders (nama_produk, user_id) VALUES ('Laptop', 1);
-- Bisa, karena user dengan id 1 ada
```

#### Catatan

a. Pastikan kolom foreign key dan kolom yang dirujuk punya tipe data yang sama (INT, VARCHAR, dll).

b.  Kalau kamu mau menghapus user, tapi dia punya order, kamu bisa atur foreign key-nya supaya:
- Ikut terhapus (ON DELETE CASCADE)
- Dicegah untuk dihapus (default)

Contoh:
```
FOREIGN KEY (user_id) REFERENCES users(id) ON DELETE CASCADE
```

### Koneksi PHP ke MySQL

a. Aktifkan Web-Server Kalian (XAMPP, Laragon, dll)

b. Buat Database dan Tabel di MySQL
- Buka browser dan pergi ke alamat `http://localhost/phpmyadmin`
- Klik 'Database' → beri nama misalnya `belajar_php` → klik 'Create'.

c. Buat tabel bernama `users` dengan kolom sebagai berikut:
- id (INT, AUTO_INCREMENT, PRIMARY)
- nama (VARCHAR 100)
- email (VARCHAR 100)

d. Buat file `koneksi.php`

```
<?php
$host = "localhost";
$user = "root";
$pass = "";
$db   = "belajar_php";

// Membuat koneksi
$conn = mysqli_connect($host, $user, $pass, $db);

// Cek koneksi
if (!$conn) {
    die("Koneksi gagal: " . mysqli_connect_error());
}
?>
```

### Menyimpan Data ke Dalam Database

Buat file baru bernama `store.php` dengan isi sebagai berikut:
```
<?php
include 'koneksi.php';

$nama = "Fufu";
$email = "fufufafa@mail.com";

$sql = "INSERT INTO users (nama, email) VALUES ('$nama', '$email')";

if (mysqli_query($conn, $sql)) {
    echo "Data berhasil ditambahkan!";
} else {
    echo "Error: " . mysqli_error($conn);
}
?>
```

### Menampilkan Data yang Ada di Dalam Database

Buat file baru bernama `show.php` dengan isi sebagai berikut:
```
<?php
include 'koneksi.php';

$sql = "SELECT * FROM users";
$result = mysqli_query($conn, $sql);

while ($row = mysqli_fetch_assoc($result)) {
    echo "ID: " . $row['id'] . "<br>";
    echo "Nama: " . $row['nama'] . "<br>";
    echo "Email: " . $row['email'] . "<hr>";
}
?>
```

<br></br>
## Kontributor

- Addin Hadi Rizal
- Abraham Willem Hersubagyo
- Bani Rijal Barru Faza
- Mohammed Nasser


<br></br>
## Credits

Tutorial ini dikembangkan oleh Asisten Praktikum Pemrograman Website 2025. Segala tutorial serta instruksi yang dicantumkan pada repositori ini dirancang sedemikian rupa sehingga mahasiswa yang sedang mengambil mata kuliah Pemrograman Website dapat menyelesaikan tutorial saat sesi lab berlangsung.

