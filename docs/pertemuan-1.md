---
sidebar_label: "Pertemuan 1: Dasar-Dasar HTML"
sidebar_position: 3
Path: docs/pertemuan-1
---

# Pertemuan 1: Dasar-Dasar HTML

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Apa itu HTML?

![html](https://assets.cdn.dicoding.com/original/academy/dos:3456ae4a1c774455d6ad47b7c432b26120230614143148.png)

HTML (HyperText Markup Language) adalah bahasa dasar untuk membuat halaman web. HTML digunakan untuk menyusun elemen-elemen dalam sebuah halaman agar dapat ditampilkan di browser.

## Anatomi Elemen HTML

Elemen HTML adalah salah satu bagian dari HTML dalam membangun halaman web. Elemen ini digunakan untuk mendefinisikan elemen-elemen yang ditampilkan dalam halaman web. Ada beberapa hal untuk membangun elemen HTML itu sendiri. Secara garis besar, berikut adalah bagan dari anatomi elemen HTML.

![anatomiHTML](https://assets.cdn.dicoding.com/original/academy/dos:9e25d269df3a01c7295ef7ff6b73d08520230623095734.png)

Berikut adalah pembahasan dari masing-masing bagian dari bagan di atas.

| **_Item_**    | **_Keterangan_**                                            |
| ------------------ | ------------------------------------------------------- |
| Tag Pembuka | Berisi nama tag dari elemen yang akan dibuat dan dibungkus dengan angle bracket < >. Contohnya adalah (< p >) untuk membuat elemen paragraf yang menggunakan p sebagai nama elemennya--singkatan dari dalam bahasa inggris (paragraph). |
| Konten | Konten dari elemen. Contohnya teks sebagai konten dari elemen paragraf. |
| Tag Penutup | Masih sama seperti tag pembuka, kecuali terdapat garis miring sebelum nama elemennya. Ini menandakan akhir dari elemen HTML. Biasanya, kesalahan bagi web programmer pemula adalah melupakan tag ini sehingga menyebabkan elemen tidak valid. |

## Atribute di Elemen HTML

Dalam membuat elemen HTML, ada satu hal yang dapat dilakukan, yaitu memberi atribut. Atribut dapat memberi informasi-informasi tambahan untuk elemen HTML. Informasi ini tidak akan tampil dalam halaman web, tetapi ia dapat menentukan perilaku elemen biasanya. Berikut adalah anatomi dari atribut elemen untuk memperjelas pemahaman kamu.

![atribute](https://assets.cdn.dicoding.com/original/academy/dos:9da1d4c308191bbbff10a6435920afa220230623095750.png)


## Anatomi Dokumen HTML

Pada dasarnya, dokumen HTML memerlukan struktur dasar untuk menampilkan halaman web dengan baik. Halaman web seharusnya memiliki susunan elemen HTML yang tampak seperti berikut.

![dokumen](https://assets.cdn.dicoding.com/original/academy/dos:97b9889c49bad9e09a265a3c9ea1d33120230621104355.jpeg)

Keterangan:
- `<!DOCTYPE html>` → Menandakan bahwa ini adalah dokumen HTML.

- `<html>` → Elemen utama yang membungkus seluruh isi halaman.

- `<head>` → Bagian kepala yang berisi informasi meta dan judul halaman.

- `<title>` → Menentukan judul yang muncul di tab browser.

- `<body>` → Bagian utama tempat konten halaman web ditampilkan.

Dokumen di atas sebetulnya akan membentuk sebuah hierarki elemen atau yang biasa disebut dengan DOM Tree (pohon DOM). Ini dapat Anda analogikan seperti silsilah keluarga. Kurang lebih, berikut adalah DOM Tree yang terbentuk dari dokumen HTML di atas.

![domHTML](https://assets.cdn.dicoding.com/original/academy/dos:0f3821d245d66fccb2a3e6e48c11095d20230623095802.png)

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

## Semantic HTML: Mengorganisasikan Halaman Konten

Website memiliki hierarki konten yang sama seperti dokumen sehari-hari yang kita baca, majalah, dan koran contohnya. Jadi, hierarki pada sebuah website merupakan hal yang penting. Tentu elemen yang terdapat pada HTML perlu kita kelompokkan menjadi beberapa bagian.

![semantic-html](https://assets.cdn.dicoding.com/original/academy/dos:9655a1733f47246eff401284ad842edd20230621104914.jpeg)

Kita dapat menggunakan beberapa elemen dalam HTML untuk mengelompokkan sebuah elemen dengan jelas dan memiliki arti (semantic meaning). Elemen-elemen ini memiliki nama sesuai dengan fungsi atau peran dari elemen tersebut.

![semantic](https://assets.cdn.dicoding.com/original/academy/dos:31844c42be86e3b00e7a9598555c53ba20230621104914.jpeg)

## Semantic VS Non-Semantic HTML

<img src="https://res.cloudinary.com/practicaldev/image/fetch/s--7rtr6qdB--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/n8f7yj3bjy7rcu03hfsa.png" height="400" width="auto" />

## Generic Elements

HTML menyediakan dua tipe elemen umum (generic element) yang bisa kita kustomisasi untuk menggambarkan konten kita dengan tepat, yaitu div dan span. Elemen ini akan terlibat jika tidak ada semantic element sesuai di HTML.

### Div

Elemen < div > merupakan sebuah wadah (container) yang bersifat umum untuk menampung beberapa konten. Elemen ini tidak akan memberikan efek apa pun pada konten atau layout sebelum menerapkan sebuah style menggunakan CSS.

```
<!DOCTYPE html>
<html>
  <head>
    <title>Div Element</title>
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <div class="shadowbox">
      <p>
        Paragraf ini berada di dalam elemen div, tetapi ia akan ditampilkan sama seperti paragraf
        biasanya. Elemen ini lebih sering digunakan untuk mengelompokkan sebuah konten sehingga
        dapat memudahkan styling dengan menggunakan atribut class atau id.
      </p>
    </div>
  </body>
</html>
```

### Span 

Elemen < span > memberikan manfaat yang sama seperti < div >, bedanya elemen ini digunakan sebagai phrase elements dan tidak terdapat line breaks ketika menggunakannya. Sederhananya, < span > merupakan sebuah < div > yang digunakan dalam sebuah baris teks yang dapat diwadahi oleh paragraf, list, heading, atau lainnya.

```
<style>
  .phone {
    font-weight: bold;
  }
</style>

<ul>
  <li>Agil: <span class="phone">08123xxx</span></li>
  <li>Widy: <span class="phone">08222xxx</span></li>
  <li>Gilang: <span class="phone">08333xxx</span></li>
</ul>
```

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
- [HTML Semantics](https://www.w3schools.com/html/html5_semantic_elements.asp)

## Kontributor

- Addin Hadi Rizal
- Abraham Willem Hersubagyo
- Bani Rijal Barru Faza
- Mohammed Nasser

## Credits

Tutorial ini dikembangkan oleh Asisten Praktikum Pemrograman Website 2025. Segala tutorial serta instruksi yang dicantumkan pada repositori ini dirancang sedemikian rupa sehingga mahasiswa yang sedang mengambil mata kuliah Pemrograman Website dapat menyelesaikan tutorial saat sesi lab berlangsung.