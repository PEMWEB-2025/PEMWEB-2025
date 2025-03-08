---
sidebar_label: "Pertemuan 1: Dasar-Dasar HTML"
sidebar_position: 3
Path: docs/pertemuan-1
---

# Pertemuan 1: Dasar-Dasar HTML

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Apa itu HTML?

<br/>
<img src="https://emaillistvalidation.com/blog/content/images/2023/09/HTML5_logo_and_wordmark.svg.png" height="200" width="auto" />
<br/><br/>

HTML (HyperText Markup Language) adalah bahasa dasar untuk membuat halaman web. HTML digunakan untuk menyusun elemen-elemen dalam sebuah halaman agar dapat ditampilkan di browser.

## Struktur Dasar HTML

Setiap halaman web yang dibuat dengan HTML memiliki struktur dasar seperti berikut:

``` 
<!DOCTYPE html>
<html>
<head>
    <title>Judul Halaman</title>
</head>
<body>
    <h1>Selamat Datang!</h1>
    <p>Ini adalah paragraf pertama dalam HTML.</p>
</body>
</html>
```

Keterangan:
- `<!DOCTYPE html>` → Menandakan bahwa ini adalah dokumen HTML.

- `<html>` → Elemen utama yang membungkus seluruh isi halaman.

- `<head>` → Bagian kepala yang berisi informasi meta dan judul halaman.

- `<title>` → Menentukan judul yang muncul di tab browser.

- `<body>` → Bagian utama tempat konten halaman web ditampilkan.

## Elemen dan Tag Dasar dalam HTML
| **Elemen** | **Tag HTML** | **Kegunaan** |
| ---------- | ------------ | ------------ |
| Heading | `<h1>` - `<h6>` | Membuat judul atau heading |
| Paragraf | `<p>` | Membuat sebuah paragraf |
| Divisi | `<div>` | Membuat sebuah divisi atau wadah untuk mengelompokkan elemen lain |
| Gambar | `<img src="gambar.jpg">` | Menampilkan gambar |
| Tautan / Link | `<a href="url">` | Membuat teks hyperlink |
| Daftar Berurutan | `<ol>` | Membuat sebuah daftar dengan nomor |
| Daftar Tidak Berurutan | `<ul>` | Membuat sebuah daftar dengan *bullet* |
| Item | `<li>` | Membuat item di dalam tag `<ul>` atau `<ol>` |
| Garis Horizontal | `<hr>` | Membuat sebuah garis horizontal |
| Baris Baru | `<br>` | Membuat sebuah baris baru |

## Contoh Penggunaan Tag Dasar HTML
```
<!DOCTYPE html>
<html>
<head>
    <title>Belajar HTML</title>
</head>
<body>
    <h1>Judul Utama</h1>
    <h2>Judul Kedua</h2>
    <p>Ini adalah sebuah paragraf yang menjelaskan sesuatu.</p>
    
    <a href="https://www.google.com">Kunjungi Google</a>
    
    <img src="gambar.jpg" alt="Gambar Contoh">
    
    <h3>Daftar Belanja</h3>
    <ul>
        <li>Apel</li>
        <li>Pisang</li>
        <li>Jeruk</li>
    </ul>
    
    <h3>Langkah-langkah Memasak</h3>
    <ol>
        <li>Siapkan bahan.</li>
        <li>Panaskan wajan.</li>
        <li>Masak hingga matang.</li>
    </ol>
</body>
</html>
```

## Apa Itu Semantic HTML?

Semantic Web adalah konsep pengembangan web yang memungkinkan data dalam suatu halaman web dapat dipahami tidak hanya oleh manusia tetapi juga oleh mesin (komputer). Ini dilakukan dengan menggunakan markup dan metadata yang memberikan konteks tambahan terhadap konten, sehingga mesin dapat mengerti makna dari informasi tersebut.

## Semantic VS Non-Semantic HTML

<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--7rtr6qdB--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/n8f7yj3bjy7rcu03hfsa.png" height="400" width="auto" />

## Kesimpulan

- HTML adalah bahasa dasar untuk membuat halaman web.

- Struktur HTML terdiri dari `<html>`, `<head>`, dan `<body>`.

- Elemen HTML menggunakan tag untuk menampilkan berbagai jenis konten.

- Dengan HTML, kita bisa membuat teks, gambar, tautan, dan daftar dengan mudah.

- Semantic HTML memungkinkan data di dalam web dipahami oleh mesin / komputer.

![HTML Meme - 1](/img/1/gambar-1.jpg)

## Referensi Tambahan
- [HTML Tutorial (W3School)](https://www.w3schools.com/html/)
- [HTML Tutorial (GeeksforGeeks)](https://www.geeksforgeeks.org/html-tutorial/)

## Kontributor

- Addin Hadi Rizal
- Abraham Willem Hersubagyo
- Bani Rijal Barru Faza
- Mohammed Nasser

## Credits

Tutorial ini dikembangkan oleh Asisten Praktikum Pemrograman Website 2025. Segala tutorial serta instruksi yang dicantumkan pada repositori ini dirancang sedemikian rupa sehingga mahasiswa yang sedang mengambil mata kuliah Pemrograman Website dapat menyelesaikan tutorial saat sesi lab berlangsung.