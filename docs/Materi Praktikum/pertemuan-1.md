---
sidebar_label: "Pertemuan 1: Pengenalan dan Pendalaman HTML"
sidebar_position: 2
Path: docs/materi/pertemuan-1
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

Dokumen di atas sebetulnya akan membentuk sebuah hierarki elemen atau yang biasa disebut dengan DOM Tree (pohon DOM). Ini dapat Temen" analogikan seperti silsilah keluarga. Kurang lebih, berikut adalah DOM Tree yang terbentuk dari dokumen HTML di atas.

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

Elemen `<div>` merupakan sebuah wadah (container) yang bersifat umum untuk menampung beberapa konten. Elemen ini tidak akan memberikan efek apa pun pada konten atau layout sebelum menerapkan sebuah style menggunakan CSS.

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

Elemen `<span>` memberikan manfaat yang sama seperti `<div>`, bedanya elemen ini digunakan sebagai phrase elements dan tidak terdapat line breaks ketika menggunakannya. Sederhananya, `<span>` merupakan sebuah `<div>` yang digunakan dalam sebuah baris teks yang dapat diwadahi oleh paragraf, list, heading, atau lainnya.

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

### Tabel

Elemen `<table>` pada HTML merepresentasikan data tabular, yaitu informasi yang disajikan dalam sebuah tabel. Tabel sendiri disajikan dalam dua dimensi terdiri dari baris dan kolom (cell) yang berisikan sebuah data. Berikut adalah contoh data sepak bola yang disajikan dalam bentuk tabel.

![tabelBola](https://assets.cdn.dicoding.com/original/academy/dos:e4a8a8b68ba34879fc15a6103466a33f20230621104914.jpeg)

### Struktur Dasar Tabel

Tabel pada HTML disusun dari tiga buah elemen, yaitu `<table>`, `<tr>` dan `< td >` atau `<th>`. Elemen `<table>` digunakan untuk menandakan dimulainya dan diakhirinya sebuah konten tabel dan juga sebagai wadah untuk tabel itu sendiri. Kemudian elemen `<tr>` digunakan untuk membuat sebuah baris baru yang di dalamnya terdapat elemen `<td>` atau `<th>` sehingga menghasilkan sebuah sel.

![strukturtabel](https://assets.cdn.dicoding.com/original/academy/dos:b33bf8e2cbd3fa59d947b667b645599a20230621104914.jpeg)

### Spanning Cell

Dalam aplikasi seperti Microsoft Word, hal ini biasa kita kenal sebagai merging cell atau menggabungkan sebuah sel. Ini memang menjadi sebuah fitur dasar dalam membuat sebuah tabel sehingga pada HTML pun kita dapat melakukan hal tersebut. 

Pada HTML hal ini lebih dikenal sebagai spanning cell, yang artinya menjangkau atau merentangkan sebuah ukuran sel lebih dari ukuran yang biasanya. Kali ini kita belajar 2 jenis yaitu ada *Column Spans* dan *Row Spans*.

Untuk merentangkan sebuah kolom (column spanning) kita bisa menggunakan atribut colspan pada elemen `<td>` atau `<th>`. Berikut adalah contoh untuk penggunaan colspan sehingga sebuah header mencakup dua kolom.

#### Column Spans 
```
<table>
  <tr>
    <th>18:00</th>
    <th>19:00</th>
    <th>20:00</th>
  </tr>
  <tr>
    <td colspan="2">Avenger Infinity Wars</td>
    <td>It Chapter 2</td>
  </tr>
  <tr>
    <td>One Piece: Stampede</td>
    <td>Weathering With You</td>
    <td>Gundala</td>
  </tr>
  <tr>
    <td>Gundala</td>
    <td colspan="2">Avenger Infinity Wars</td>
  </tr>
</table>
```

#### Row Spans 

Untuk merentangkan sebuah baris (row spanning) kita dapat menggunakan atribut rowspan. Mirip seperti column spanning, tetapi atribut ini akan merentangkan sebuah sel ke bawah. Berikut contohnya.
```
<table border="1">
  <tr>
    <th rowspan="3">18:00</th>
    <td>Avenger Infinity Wars</td>
  </tr>
  <tr>
    <td>One Piece: Stampede</td>
  </tr>
  <tr>
    <td>Gundala</td>
  </tr>
</table>
```

## Input User
Hampir seluruh website memiliki elemen input. Data yang dimasukkan akan diproses untuk kebutuhan operasional website dalam menunjang pekerjaan manusia. Ada banyak sekali macam-macam input di dunia ini. Namun, jangan khawatir! HTML menyediakan beragam input yang dapat dimanfaatkan. Berikut daftarnya.

### Input Element

Elemen `<input>` merupakan elemen yang sangat sering dipakai untuk mendapatkan data dari user. Mengapa hal tersebut terjadi? Hal ini karena elemen input memiliki banyak sekali tipe-tipenya, mulai dari teks, password, email, search, file, dsb. Tidak hanya itu, dari sekian tipe input, masing-masingnya juga didukung oleh atribut khusus sehingga pembuatan formulir semakin powerful.
```
<div>
  Text:
  <input type="text" />
</div>
<div>
  Number:
  <input type="number" />
</div>
<div>
  Email:
  <input type="email" />
</div>
<div>
  Password:
  <input type="password" />
</div>
```

### Textarea Element
HTML memiliki elemen khusus yang memungkinkan user menuliskan teks dalam banyak baris. Kenalilah elemen `<textarea>`! Elemen ini berbeda dengan elemen input sebelumnya. Selain nama elemen yang menjadi pembeda, elemen textarea memiliki tag penutup agar dapat berfungsi dengan baik.
```
<textarea rows="6" cols="16">
Belajar
Dasar
Pemrograman
Web
</textarea>
```

### Label Element
Pembuatan elemen input sudah umum jika dijajarkan dengan elemen label. Ada banyak sekali keuntungan jika memberikan keterangan pada masing-masing elemen input. Beberapa keuntungan penerapan label untuk elemen input sebagai berikut.

Elemen input yang berasosiasi dengan elemen label akan memberikan kemampuan bagi screen reader untuk menjelaskan fungsi dari elemen input tersebut.
Memberikan kemampuan bagi browser untuk mengalihkan langsung pada elemen input saat elemen label yang berasosiasi dengannya ditekan atau klik.
```
<div>
  <label for="email">Email</label>
  <br>
  <input type="email" id="email" />
</div>
 
<div>
  <label for="password">Password</label>
  <br>
  <input type="password" id="password" />
</div>
```

## Atribute Pada Element Input
Selain banyaknya variasi elemen input, ada banyak atribut yang tersedia untuk memaksimalkan pembuatan formulir. Ada atribut yang bekerja untuk semua tipe input dan ada atribut yang hanya dikhususkan bagi satu tipe.

Berikut adalah contoh penerapan atribut placeholder dan required.
```
<div>
  <label for="email">Email</label>
  <br />
  <input type="email" id="email" placeholder="example@mail.com" required />
</div>

<div>
  <label for="password">Password</label>
  <br />
  <input type="password" id="password" placeholder="********" required />
</div>
```

> Elemen label tidak dapat digantikan oleh atribut placeholder. Kedua hal ini memiliki peranannya sendiri dalam membuat formulir. Placeholder berfungsi sebagai petunjuk user dalam mengisi data, bukan untuk memberi keterangan atau caption elemen input.

## Mengirim Data Formulir
![data](https://assets.cdn.dicoding.com/original/academy/dos:bdb23ce5cc1fdaeb0332561e1b77854f20230620071038.jpeg)
Ketika client membutuhkan resources guna menampilkan halaman web ke pengguna, ia akan mengirimkan request ke server tentang kebutuhan yang dimaksud. HTML, CSS, JavaScript, serta aset-aset lainnya merupakan resources yang akan dikirimkan dan di-render oleh browser sehingga tampillah halaman web yang utuh. Nah, hal tersebut merupakan proses yang serupa yang akan dilakukan oleh browser dan server.
![data](https://assets.cdn.dicoding.com/original/academy/dos:fad9aa23f47230b56c12252522f9870e20230620071038.jpeg)
Ada satu elemen yang berfungsi sebagai wrapper (pembungkus) dari keseluruhan kolom input atau formulir. Elemen yang dimaksud adalah `<form>`.
```
<form>
  <div>
    <label for="email">Email</label>
    <br />
    <input type="email" id="email" />
  </div>
 
  <div>
    <label for="password">Password</label>
    <br />
    <input type="password" id="password" />
  </div>
 
  <button type="submit">Submit</button>
</form>
```

## Special Character
Ada beberapa karakter spesial seperti copyright symbol (©) yang tidak termasuk ke dalam standar kelompok ASCII characters. ASCII characters hanya menyediakan karakter seperti huruf, nomor, dan beberapa simbol dasar lainnya.

HTML memerlukan sebuah “escaped” character untuk menampilkan karakter khusus. Ada dua cara untuk melakukannya, yakni menetapkan nilai numerik (numeric entity) atau menggunakan nama singkatan yang sudah ditetapkan untuk masing-masing karakternya (named entity). Semua referensi karakter dimulai dengan “&” dan diakhiri dengan “;”.
```
<p>Addin ganteng bangett &copy; 2025, UNS</p>
<!-- Juga bisa menggunakan &#169; -->
<p>Addin ganteng bangett &#169; 2025, UNS</p>
```
Tampilannya sama saja.

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