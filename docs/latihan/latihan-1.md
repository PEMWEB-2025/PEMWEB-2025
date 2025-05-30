---
sidebar_label: Latihan Praktikum 1
sidebar_position: 1
Path: docs/latihan/latihan-1
---
import CodeBlock from '@theme/CodeBlock';

# Alur Latihan
Berikut adalah alur latihan kali ini.

1. Membuka code editor bawaan sistem operasi.
2. Menuliskan struktur konten (kode) halaman web pada code editor.
3. Menyimpan kode yang telah ditulis dalam bentuk HTML.
4. Menjalankan berkas HTML dalam browser (Google Chrome).

## Latihan: Membangun Halaman Web Pertama (Halaman Profil)

1. Membuat Folder Baru
Untuk tempatnya bebas diberi nama `WebDasar`
> Untuk folder dan filenya nanti harap disimpan karena bakal digunakan untuk latihan" selanjutnya.
2. Buka foldernya pada code editor kalian masiing" lalu buat file bernama `index.html`.
3. Pada file `index.html` buat code html sebagai berikut:
<CodeBlock className="no-copy">
{`<!DOCTYPE html>
<html>
  <head></head>
  <body>   
 
  </body>
</html>`}
</CodeBlock>

Pindahkan semua text dibawah ini kedalam elemen `<body>`
```
Bandung
Kota metropolitan terbesar di Provinsi Jawa Barat, sekaligus menjadi ibu kota provinsi tersebut.

Sejarah
Kata Bandung berasal dari kata bendung atau bendungan karena terbendungnya sungai Citarum oleh lava Gunung Tangkuban Parahu yang lalu membentuk telaga. Legenda yang diceritakan oleh orang-orang tua di Bandung mengatakan bahwa nama Bandung diambil dari sebuah kendaraan air yang terdiri dari dua perahu yang diikat berdampingan yang disebut perahu bandung yang digunakan oleh Bupati Bandung, R.A. Wiranatakusumah II, untuk melayari Ci Tarum dalam mencari tempat kedudukan kabupaten yang baru untuk menggantikan ibu kota yang lama di Dayeuhkolot.

Berdasarkan filosofi Sunda, kata Bandung juga berasal dari kalimat Nga-Bandung-an Banda Indung, yang merupakan kalimat sakral dan luhur karena mengandung nilai ajaran Sunda. Nga-Bandung-an artinya menyaksikan atau bersaksi. Banda adalah segala sesuatu yang berada di alam hidup yaitu di bumi dan atmosfer, baik makhluk hidup maupun benda mati. Sinonim dari banda adalah harta. Indung berarti Ibu atau Bumi, disebut juga sebagai Ibu Pertiwi tempat Banda berada.

Geografis
Kota Bandung dikelilingi oleh pegunungan, sehingga bentuk morfologi wilayahnya bagaikan sebuah mangkok raksasa, secara geografis kota ini terletak di tengah-tengah provinsi Jawa Barat, serta berada pada ketinggian ±768 m di atas permukaan laut, dengan titik tertinggi di berada di sebelah utara dengan ketinggian 1.050 meter di atas permukaan laut dan sebelah selatan merupakan kawasan rendah dengan ketinggian 675 meter di atas permukaan laut.

Kota Bandung dialiri dua sungai utama, yaitu Sungai Cikapundung dan Sungai Citarum beserta anak-anak sungainya yang pada umumnya mengalir ke arah selatan dan bertemu di Sungai Citarum. Dengan kondisi yang demikian, Bandung selatan sangat rentan terhadap masalah banjir terutama pada musim hujan.

Wisata
Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan utama dalam menikmati liburan akhir pekan terutama dari masyarakat yang berasal dari Jakarta sekitarnya. Selain menjadi kota wisata belanja, kota Bandung juga dikenal dengan sejumlah besar bangunan lama berarsitektur peninggalan Belanda.
 
 
Farm House Lembang
Berada di jalur utama Bandung-Lembang, Farm House menjadi objek wisata yang tidak pernah sepi pengunjung. Selain karena letaknya strategis, kawasan ini juga menghadirkan nuansa wisata khas Eropa. Semua itu diterapkan dalam bentuk spot swafoto Instagramable.
 
Observatorium Bosscha
Memiliki beberapa teleskop, antara lain, Refraktor Ganda Zeiss, Schmidt Bimasakti, Refraktor Bamberg, Cassegrain GOTO, dan Teleskop Surya. Refraktor Ganda Zeiss adalah jenis teleskop terbesar untuk meneropong bintang. Benda ini diletakkan pada atap kubah sehingga saat teropong digunakan, atap tersebut harus dibuka. Observatorium Bosscha boleh dikunjungi oleh siapa pun, tanpa tiket. Namun, bagi yang ingin menggunakan teleskop Zeiss, wajib mendaftarkan diri. Untuk instansi atau lembaga pendidikan, diberikan jadwal hari Selasa sampai Jumat. Sementara itu, kunjungan individu dibuka setiap hari Sabtu.
```
4. Selanjutnya, kita akan mengidentifikasi konten artikel ini. Carilah konten yang paling penting atau topik utama pembahasan dari artikel serta bungkus konten tersebut dengan elemen `<h1>`; lalu, konten yang merupakan pemaparan dari topik tersebut serta bungkus konten tersebut dengan elemen `<p>`; dan seterusnya.
![html1](https://assets.cdn.dicoding.com/original/academy/dos:c93d74986053663056fd03b38021eca520230614150618.jpeg)
5. Jika sudah, kita dapat memberi elemen heading dan elemen paragraf sesuai dengan hasil identifikasi. Jika diimplementasikan, hasil kode akan tampak seperti berikut.

<CodeBlock className="no-copy">
{`<!DOCTYPE html><html>
  <head></head>
  <body>
    <h1>Bandung</h1>
    <p>
      Kota metropolitan terbesar di Provinsi Jawa Barat, sekaligus menjadi ibu
      kota provinsi tersebut.
    </p>
 
 
    <h2>Sejarah</h2>
    <p>
      Kata Bandung berasal dari kata bendung atau bendungan karena terbendungnya
      sungai Citarum oleh lava Gunung Tangkuban Parahu yang lalu membentuk
      telaga. Legenda yang diceritakan oleh orang-orang tua di Bandung
      mengatakan bahwa nama Bandung diambil dari sebuah kendaraan air yang
      terdiri dari dua perahu yang diikat berdampingan yang disebut perahu
      bandung yang digunakan oleh Bupati Bandung, R.A. Wiranatakusumah II, untuk
      melayari Ci Tarum dalam mencari tempat kedudukan kabupaten yang baru untuk
      menggantikan ibu kota yang lama di Dayeuhkolot.
    </p>
    <p>
      Berdasarkan filosofi Sunda, kata Bandung juga berasal dari kalimat
      Nga-Bandung-an Banda Indung, yang merupakan kalimat sakral dan luhur
      karena mengandung nilai ajaran Sunda. Nga-Bandung-an artinya menyaksikan
      atau bersaksi. Banda adalah segala sesuatu yang berada di alam hidup yaitu
      di bumi dan atmosfer, baik makhluk hidup maupun benda mati. Sinonim dari
      banda adalah harta. Indung berarti Ibu atau Bumi, disebut juga sebagai Ibu
      Pertiwi tempat Banda berada.
    </p>
 
 
    <h2>Geografis</h2>
    <p>
      Kota Bandung dikelilingi oleh pegunungan, sehingga bentuk morfologi
      wilayahnya bagaikan sebuah mangkok raksasa, secara geografis kota ini
      terletak di tengah-tengah provinsi Jawa Barat, serta berada pada
      ketinggian ±768 m di atas permukaan laut, dengan titik tertinggi di berada
      di sebelah utara dengan ketinggian 1.050 meter di atas permukaan laut dan
      sebelah selatan merupakan kawasan rendah dengan ketinggian 675 meter di
      atas permukaan laut.
    </p>
    <p>
      Kota Bandung dialiri dua sungai utama, yaitu Sungai Cikapundung dan Sungai
      Citarum beserta anak-anak sungainya yang pada umumnya mengalir ke arah
      selatan dan bertemu di Sungai Citarum. Dengan kondisi yang demikian,
      Bandung selatan sangat rentan terhadap masalah banjir terutama pada musim
      hujan.
    </p>
 
 
    <h2>Wisata</h2>
    <p>
      Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan
      utama dalam menikmati liburan akhir pekan terutama dari masyarakat yang
      berasal dari Jakarta sekitarnya. Selain menjadi kota wisata belanja, kota
      Bandung juga dikenal dengan sejumlah besar bangunan lama berarsitektur
      peninggalan Belanda.
    </p>
 
    <h3>Farm House Lembang</h3>
    <p>
      Berada di jalur utama Bandung-Lembang, Farm House menjadi objek wisata
      yang tidak pernah sepi pengunjung. Selain karena letaknya strategis,
      kawasan ini juga menghadirkan nuansa wisata khas Eropa. Semua itu
      diterapkan dalam bentuk spot swafoto Instagramable.
    </p>
 
    <h3>Observatorium Bosscha</h3>
    <p>
      Memiliki beberapa teleskop, antara lain, Refraktor Ganda Zeiss, Schmidt
      Bimasakti, Refraktor Bamberg, Cassegrain GOTO, dan Teleskop Surya.
      Refraktor Ganda Zeiss adalah jenis teleskop terbesar untuk meneropong
      bintang. Benda ini diletakkan pada atap kubah sehingga saat teropong
      digunakan, atap tersebut harus dibuka. Observatorium Bosscha boleh
      dikunjungi oleh siapapun, tanpa tiket. Namun, bagi yang ingin menggunakan
      teleskop Zeiss, wajib mendaftarkan diri. Untuk instansi atau lembaga
      pendidikan, diberikan jadwal hari Selasa sampai Jumat. Sementara itu,
      kunjungan individu dibuka setiap hari Sabtu.
    </p>
  </body>
</html>`}
</CodeBlock>

6. Silakan save perubahan yang terjadi pada berkas HTML dan buka pada browser. Seharusnya, halaman web akan terlihat seperti berikut.
![HTML](/img/1/html1.png)
7. Kita belum selesai sampai di sini. Tidak hanya elemen `<body>`, untuk memperlengkap dokumen ini, kita akan melengkapi elemen dalam elemen `<head>`. Silakan tambahkan kode bercetak tebal berikut pada index.html.
<CodeBlock className="no-copy">
{`<!DOCTYPE html><html>
  <head>
    <meta charset="utf-8">
    <title>Halaman Profil Bandung</title>
  </head>
  <body>
    <!-- Kode lainnya disembunyikan... -->
  </body>
</html>`}
</CodeBlock>

8. Bedah Kode
Temen" juga dapat membuktikannya pada praktik latihan sebelumnya. Temen" dapat memeriksanya pada Developer Tools dari browser yang digunakan (Google Chrome). Bagi pengguna Google Chrome, Temen" bisa menekan tombol F12 dan membuka tab Elements.
![bedah](https://assets.cdn.dicoding.com/original/academy/dos:d7095bac468b184e3ea386f41199c99120230614150619.jpeg)

## Latihan: Menambahkan List pada Halaman Profil
> Tips:
>Pada langkah ini dan berikutnya, sebaiknya gunakanlah code editor yang disarankan pada pembahasan Requirement Tools agar proses penulisan dan pengelolaan berkas HTML dapat lebih cepat.
### Alur Latihan
Berikut adalah alur latihan kali ini.

1. Membuka hasil latihan terakhir dengan VSCode.
2. Menuliskan navigation list pada dokumen HTML.
3. Menjalankan dokumen HTML pada browser.

### Latihan Menambahkan List pada Halaman Profil
1. Silakan buka proyek Halaman Profil terakhir dengan VS Code.
2. Kita akan menambahkan daftar navigasi menggunakan elemen list. Silakan buka berkas index.html dan tambahkan elemen unordered list berikut di bawah dari elemen paragraf pertama pada berkas HTML.
<CodeBlock className="no-copy">
{`<!-- Kode lainnya disembunyikan... -->
 
<body>
  <h1>Bandung</h1>
  <p>
    Kota metropolitan terbesar di Provinsi Jawa Barat, sekaligus menjadi ibu kota provinsi 
    tersebut.
  </p>
 
  <ul>
    <li>Sejarah</li>
    <li>Geografis</li>
    <li>Wisata</li>
  </ul>
 
  <h2>Sejarah</h2>
  <!-- Kode lainnya disembunyikan... -->
</body>`}
</CodeBlock>

#### Referensi
1. [The Ordered List Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol)
2. [The Unordered List Element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

## Latihan: Menambahkan Gambar pada Halaman Profil

### Alur Latihan

Berikut adalah alur latihan kali ini.

1. Membuka hasil latihan terakhir dengan VSCode.
2. Mengunduh dan memindahkan aset-aset gambar yang telah disediakan pada proyek.
3. Menambahkan elemen gambar pada beberapa topik.
4. Menjalankan dokumen HTML pada browser.

### Latihan Menambahkan Gambar pada Halaman Profil

1. Silakan buka proyek Halaman Profil terakhir dengan VSCode.
2. Karena kita akan menampilkan elemen-elemen gambar, silakan unduh aset-aset gambar yang digunakan pada [halaman-profil-bandung-images.zip](https://raw.githubusercontent.com/dicodingacademy/a123-webdasar-labs/099-shared-files/halaman-profil-bandung-images.zip).
3. Jika sudah, silakan pindahkan berkas hasil unduhan pada halaman proyek. Pastikan berkas diletakkan sejajar dengan berkas index.html dan apabila belum di ekstract silahkan di extract all dulu pada folder `WebDasar`.
![html2](https://assets.cdn.dicoding.com/original/academy/dos:624feed93fba0096c3ff4c8c7e1c762020230619221922.jpeg)
4. Sebelum lanjut, pastikan isi folder assets → image ada empat buah berkas gambar. Berkas-berkas ini yang akan kita tampilkan dalam halaman web.
![file](https://assets.cdn.dicoding.com/original/academy/dos:939669300d45bda364f735391980776920230619222025.jpeg)
5. Pada folder WebDasar, kita sudah memiliki dua isi, yaitu folder bernama “halaman-profil-bandung-images” dan berkas index.html. Silakan ubah dulu nama folder “halaman-profil-bandung-images” menjadi “assets”. Tujuannya hanya untuk mempermudah pemanggilan folder saja ketika digunakan.
6. Jika aset gambar sudah siap, mari kita terapkan pembelajaran elemen `<img>` pada proyek ini. Silakan buka berkas index.html dan tambahkan elemen-elemen gambar di bawah elemen heading sesuai kontennya masing-masing. Kode yang perlu ditambahkan memiliki cetakan tebal.
<CodeBlock className="no-copy">
{`<!DOCTYPE html><html>
  <head>
    <!-- Kode disembunyikan... -->
  </head>
  <body>
    <!-- Kode disembunyikan... -->
 
    <h2>Sejarah</h2>
    <img src="assets/image/history.jpg" alt="Sejarah" />
 
    <!-- Kode disembunyikan... -->
 
    <h2>Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="Geografis" />
 
    <!-- Kode disembunyikan... -->
 
    <h3>Farm House Lembang</h3>
    <img src="assets/image/farm-house.jpg" alt="Farm house" />
    <p>
      <!-- Kode disembunyikan... -->
    </p>
 
    <h3>Observatorium Bosscha</h3>
    <img src="assets/image/bosscha.jpg" alt="Bosscha" />
    <p>
      <!-- Kode disembunyikan... -->
    </p>
  </body>
</html>`}
</CodeBlock>

7. Perhatikan penulisan nilai dari atribut `src`. Penulisannya sedikit berbeda dengan yang telah kita pelajari. Penulisan alamat gambar tidak menggunakan URL dari suatu domain (misalnya “https://www.example.com/image.jpg”). Namun, kita menggunakan relative URL di sini. URL yang merupakan lokasi sumber gambar yang relatif terhadap lokasi berkas index.html. Hal ini karena kita menggunakan gambar lokal yang ada dalam proyek pekerjaan kita sehingga penulisan path-nya mengarah ke lokasi dari berkas gambar tersebut.
8. Setelah menambahkan elemen gambar, halaman akan tampak seperti gambar berikut.
![hasilgamabr](https://assets.cdn.dicoding.com/original/academy/dos:543dc29992d23cc9b16086bab9b67f2e20230619222210.jpeg)
> Kalau kalian ingin mengubah ukuran gambar tinggal tambah atribute width atau height 

> Tips: Jangan menambahkan atribute width atau height secara bersamaan tambahkan saja salah satu atribute

## Latihan: Menerapkan Elemen Anchor pada Halaman Profil

### Alur Latihan
Berikut adalah alur latihan kali ini.

1. Membuka hasil latihan terakhir dengan VSCode.
2. Membuat elemen anchor dalam list item pada navigation list.
3. Memberikan atribut id pada setiap elemen `<h2>` sebagai topik pembahasan artikel.
4. Menyesuaikan nilai atribut href sesuai dengan id di setiap elemen `<h2>`. 
5. Menjalankan halaman web pada browser.

### Latihan Menerapkan Elemen Anchor pada Halaman Profil

1. Silakan buka proyek Halaman Profil terbaru.
2. Untuk menerapkan elemen anchor, tentu saja kita perlu memperbarui kode pada dokumen HTML. Jadi, silakan buka kembali berkas index.html dan tambahkan atau sesuaikan kodenya agar sesuai dengan kode bercetak tebal berikut.
<CodeBlock className="no-copy">
{`<!DOCTYPE html><html>
  <head>
    <meta charset="utf-8" />
    <title>Halaman Profil Bandung</title>
  </head>
  <body>
    <h1>Bandung</h1>
    <p>
      Kota metropolitan terbesar di Provinsi Jawa Barat, sekaligus menjadi ibu kota provinsi
      tersebut.
    </p>
 
    <ul>
      <li>
        <a href="#">Sejarah</a>
      </li>
      <li>
        <a href="#">Geografis</a>
      </li>
      <li>
        <a href="#">Wisata</a>
      </li>
    </ul>
 
    <h2>Sejarah</h2>
    <!-- Kode lainnya disembunyikan... -->
  </body>
</html>`}
</CodeBlock>

3. Setelah menambahkan elemen anchor pada list item, tampilan navigation list akan menjadi hyperlink dan tampak seperti gambar berikut.
![anchor](https://assets.cdn.dicoding.com/original/academy/dos:a9e5027017326bc891abb8a92fc8456f20230620052022.jpeg)
4. Namun, ketika salah satu item ditekan, tidak ada apa pun yang terjadi. Hal ini karena atribut href belum mengetahui topik yang akan diincar. Nilai href dapat berupa URL untuk mengarahkan ke halaman yang berbeda atau berupa anchor (tanda pagar (#)) yang diikuti dengan nama id dari elemen. Hal ini berguna untuk mengarahkan fokus pengguna pada elemen tersebut.

Oleh karena itu, mari kita berikan atribut id pada elemen-elemen yang akan menjadi target navigasi. Silakan sesuaikan kodenya dengan kode yang memiliki cetakan tebal berikut.
<CodeBlock className="no-copy">
{`<!DOCTYPE html><html>
  <!-- Kode lainnya disembunyikan... -->
  <body>
    <!-- Kode lainnya disembunyikan... -->
 
    <ul>
      <li>
        <a href="#sejarah">Sejarah</a>
      </li>
      <li>
        <a href="#geografis">Geografis</a>
      </li>
      <li>
        <a href="#wisata">Wisata</a>
      </li>
    </ul>
 
    <h2 id="sejarah">Sejarah</h2>
    <img src="assets/image/history.jpg" alt="Sejarah" />
    <!-- Kode lainnya disembunyikan... -->
 
    <h2 id="geografis">Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="Geografis" />
    <!-- Kode lainnya disembunyikan... -->
 
    <h2 id="wisata">Wisata</h2>
    <!-- Kode lainnya disembunyikan... -->
  </body>
</html>`}
</CodeBlock>

5. Sip! Seharusnya, navigasi sudah berfungsi dengan baik. Temen" bisa klik salah satu navigation item tersebut untuk menuju topik yang diinginkan sekarang.

## Latihan: Menetapkan Elemen Header, Main, dan Footer di Halaman Profil

### Alur Latihan

Berikut adalah alur latihan kali ini.

1. Membuka hasil latihan terakhir dengan VSCode.
2. Membungkus judul halaman beserta deskripsinya dan daftar navigasi dengan elemen header.
3. Membungkus teks hak cipta dengan elemen footer.
4. Membungkus konten utama dengan elemen main.
5. Menjalankan dokumen HTML pada browser.

### Latihan Menetapkan Elemen Header, Main, dan Footer di Halaman Profil
1. Silakan buka proyek Halaman Profil terbaru dengan VS Code.
2. Kita akan membagi konten yang ditampilkan pada halaman web. Tentu saja konten tersebut berada dalam elemen `<body>`. Pembagian ini terbagi menjadi tiga bagian besar, yaitu heading, main, dan footer.

Pertama kali, kelompokkanlah konten judul besar dan navigasi menggunakan elemen `<header>`.
<CodeBlock className="no-copy">
{`<body>
  <header>
    <h1>Bandung</h1>
    <p>
      Kota metropolitan terbesar di Provinsi Jawa Barat, sekaligus menjadi ibu kota provinsi 
      tersebut.
    </p>
    <ul>
      <li><a href="#sejarah">Sejarah</a></li>
      <li><a href="#geografis">Geografis</a></li>
      <li><a href="#wisata">Wisata</a></li>
    </ul>
  </header>
 
  <!-- Kode lainnya disembunyikan... -->
</body>`}
</CodeBlock>

3. Sebelumnya, kita telah membuat daftar navigasi menggunakan elemen list. Namun, browser tidak mengetahui bahwa elemen list tersebut merupakan navigation list karena ia hanyalah elemen yang menampilkan sebuah daftar barang saja. Oleh karena itu, kita akan memanfaatkan semantic element lainnya yang bernama `<nav>`. Silakan bungkus elemen list dengan elemen nav menjadi seperti berikut.
<CodeBlock className="no-copy">
{`<body>
  <header>
    <h1>Bandung</h1>
    <p>
      Kota metropolitan terbesar di Provinsi Jawa Barat, sekaligus menjadi ibu kota provinsi
      tersebut.
    </p>
 
    <nav>
      <ul>
        <li><a href="#sejarah">Sejarah</a></li>
        <li><a href="#geografis">Geografis</a></li>
        <li><a href="#wisata">Wisata</a></li>
      </ul>
    </nav>
  </header>
 
  <!-- Kode lainnya disembunyikan... -->
</body>`}
</CodeBlock>

4. Sudah selesai mengelompokkan konten kepala dengan elemen header. Kita akan masuk ke bagian konten kaki terlebih dahulu. Pada konten hak cipta (copyright)–biasanya berada di paling akhir dari konten body, pindahkan atau bungkus konten tersebut dalam elemen `<footer>`. Hasilnya seperti berikut.
<CodeBlock className="no-copy">
{`<body>
  <!-- Kode lainnya disembunyikan... -->
 
  <footer>
    <p>Belajar Dasar Pemrograman Web &#169; 2025, UNS</p>
  </footer>
</body>`}
</CodeBlock>

5. Dua konten sudah kita kelompokkan. Terakhir adalah konten pokok atau utama. Elemen apa yang akan kita gunakan untuk mengelompokkan konten tersebut? Tentu saja jawabannya adalah elemen `<main>`. Silakan bungkus seluruh isi elemen di antara elemen `<header>` dan `<footer>` dengan elemen `<main>`. Hasilnya seperti berikut.
<CodeBlock className="no-copy">
{`<body>
  <header>
    <!-- Kode lainnya disembunyikan... -->
  </header>
 
  <main>
    <h2 id="sejarah">Sejarah</h2>
    <img src="assets/image/history.jpg" alt="sejarah" />
    <p>
      Kata Bandung berasal dari kata bendung atau bendungan karena terbendungnya sungai Citarum 
      oleh lava Gunung Tangkuban Parahu yang lalu membentuk telaga. Legenda yang diceritakan oleh
      orang-orang tua di Bandung mengatakan bahwa nama Bandung diambil dari sebuah kendaraan air
      yang terdiri dari dua perahu yang diikat berdampingan yang disebut perahu bandung yang
      digunakan oleh Bupati Bandung, R.A. Wiranatakusumah II, untuk melayari Ci Tarum dalam mencari
      tempat kedudukan kabupaten yang baru untuk menggantikan ibu kota yang lama di Dayeuhkolot.
    </p>
 
    <p>
      Berdasarkan filosofi Sunda, kata Bandung juga berasal dari kalimat Nga-Bandung-an Banda
      Indung, yang merupakan kalimat sakral dan luhur karena mengandung nilai ajaran Sunda.
      Nga-Bandung-an artinya menyaksikan atau bersaksi. Banda adalah segala sesuatu yang berada di
      alam hidup yaitu di bumi dan atmosfer, baik makhluk hidup maupun benda mati. Sinonim dari
      banda adalah harta. Indung berarti Ibu atau Bumi, disebut juga sebagai Ibu Pertiwi tempat
      Banda berada.
    </p>
 
    <h2 id="geografis">Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="geografis" />
    <p>
      Kota Bandung dikelilingi oleh pegunungan, sehingga bentuk morfologi wilayahnya bagaikan sebuah
      mangkok raksasa,[9] secara geografis kota ini terletak di tengah-tengah provinsi Jawa Barat,
      serta berada pada ketinggian ±768 m di atas permukaan laut, dengan titik tertinggi di berada
      di sebelah utara dengan ketinggian 1.050 meter di atas permukaan laut dan sebelah selatan
      merupakan kawasan rendah dengan ketinggian 675 meter di atas permukaan laut.
    </p>
 
    <p>
      Kota Bandung dialiri dua sungai utama, yaitu Sungai Cikapundung dan Sungai Citarum beserta
      anak-anak sungainya yang pada umumnya mengalir ke arah selatan dan bertemu di Sungai Citarum.
      Dengan kondisi yang demikian, Bandung selatan sangat rentan terhadap masalah banjir terutama
      pada musim hujan.
    </p>
 
    <h2 id="wisata">Wisata</h2>
    <p>
      Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan utama dalam menikmati
      liburan akhir pekan terutama dari masyarakat yang berasal dari Jakarta sekitarnya. Selain
      menjadi kota wisata belanja, kota Bandung juga dikenal dengan sejumlah besar bangunan lama
      berarsitektur peninggalan Belanda.
    </p>
 
    <h3>Farm House Lembang</h3>
    <img src="assets/image/farm-house.jpg" alt="farm house" />
    <p>
      Berada di jalur utama Bandung-Lembang, Farm House menjadi objek wisata yang tidak pernah sepi
      pengunjung. Selain karena letaknya strategis, kawasan ini juga menghadirkan nuansa wisata khas
      Eropa. Semua itu diterapkan dalam bentuk spot swafoto Instagramable.
    </p>
 
    <h3>Observatorium Bosscha</h3>
    <img src="assets/image/bosscha.jpg" alt="bosscha" />
    <p>
      Memiliki beberapa teleskop, antara lain, Refraktor Ganda Zeiss, Schmidt Bimasakti, Refraktor
      Bamberg, Cassegrain GOTO, dan Teleskop Surya. Refraktor Ganda Zeiss adalah jenis teleskop
      terbesar untuk meneropong bintang. Benda ini diletakkan pada atap kubah sehingga saat teropong
      digunakan, atap tersebut harus dibuka. Observatorium Bosscha boleh dikunjungi oleh siapapun,
      tanpa tiket. Namun, bagi yang ingin menggunakan teleskop Zeiss, wajib mendaftarkan diri. Untuk
      instansi atau lembaga pendidikan, diberikan jadwal hari Selasa sampai Jumat. Sementara itu,
      kunjungan individu dibuka setiap hari Sabtu.
    </p>
 
    <h2>Kota Bandung</h2>
    <p>Kota Kembang Paris van Java</p>
    <figure>
      <img src="assets/image/bandung-badge.png" />
      <figcaption>Lambang</figcaption>
    </figure>
  </main>
 
  <footer>
    <!-- Kode lainnya disembunyikan... -->
  </footer>
</body>`}
</CodeBlock>

6. Alhasil, struktur body pada HTML menjadi seperti berikut.
![strukturhtml](https://lh6.googleusercontent.com/RjXGg2veYuClz4872Wl9HVTN65hm34BuLZTmYt09oaXpUdLna4NpuImPNd87_dW0UVL4mrkT5hw-ywC-qexPPudFLsrli2B6sUhydSA5sq_VDCiT3x_qvF7DuNw2jX6Z0cO7algvSS4dqIE__EMHkQU)

## Latihan: Menerapkan Elemen Div, Aside, Article, dan Section di Halaman Profil

### Alur Latihan

Berikut adalah alur latihan kali ini.

1. Membuka hasil latihan terakhir dengan VSCode.
2. Membagi konten utama dengan elemen `<article>`.
3. Membungkus konten wisata menjadi beberapa bagian.
4. Menjalankan dokumen HTML pada browser.

### Latihan Menerapkan Elemen Div, Aside, Article, dan Section di Halaman Profil
1. Silakan buka proyek Halaman Profil terakhir dengan VSCode.
2. Pengelompokan akan dimulai dari hierarki teratas. Dalam elemen `<main>`, kita akan bagi konten menjadi dua bagian, yaitu konten artikel yang dikelompokkan menggunakan `<div>` dan konten samping yang dikelompokkan menggunakan `<aside>`. Silakan sesuaikan kodenya menjadi kode bercetak tebal berikut.

<CodeBlock className="no-copy">
{`<main>
  <!-- Konten artikel -->
  <div>
    <h2 id="sejarah">Sejarah</h2>
    <img src="assets/image/history.jpg" alt="sejarah" />
    <p>
      Kata Bandung berasal dari kata bendung atau bendungan karena terbendungnya sungai Citarum oleh
      lava Gunung Tangkuban Parahu yang lalu membentuk telaga. Legenda yang diceritakan oleh
      orang-orang tua di Bandung mengatakan bahwa nama Bandung diambil dari sebuah kendaraan air
      yang terdiri dari dua perahu yang diikat berdampingan yang disebut perahu bandung yang
      digunakan oleh Bupati Bandung, R.A. Wiranatakusumah II, untuk melayari Ci Tarum dalam mencari
      tempat kedudukan kabupaten yang baru untuk menggantikan ibu kota yang lama di Dayeuhkolot.
    </p>
 
    <p>
      Berdasarkan filosofi Sunda, kata Bandung juga berasal dari kalimat Nga-Bandung-an Banda
      Indung, yang merupakan kalimat sakral dan luhur karena mengandung nilai ajaran Sunda.
      Nga-Bandung-an artinya menyaksikan atau bersaksi. Banda adalah segala sesuatu yang berada di
      alam hidup yaitu di bumi dan atmosfer, baik makhluk hidup maupun benda mati. Sinonim dari
      banda adalah harta. Indung berarti Ibu atau Bumi, disebut juga sebagai Ibu Pertiwi tempat
      Banda berada.
    </p>
 
    <h2 id="geografis">Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="geografis" />
    <p>
      Kota Bandung dikelilingi oleh pegunungan, sehingga bentuk morfologi wilayahnya bagaikan sebuah
      mangkok raksasa,[9] secara geografis kota ini terletak di tengah-tengah provinsi Jawa Barat,
      serta berada pada ketinggian ±768 m di atas permukaan laut, dengan titik tertinggi di berada
      di sebelah utara dengan ketinggian 1.050 meter di atas permukaan laut dan sebelah selatan
      merupakan kawasan rendah dengan ketinggian 675 meter di atas permukaan laut.
    </p>
 
    <p>
      Kota Bandung dialiri dua sungai utama, yaitu Sungai Cikapundung dan Sungai Citarum beserta
      anak-anak sungainya yang pada umumnya mengalir ke arah selatan dan bertemu di Sungai Citarum.
      Dengan kondisi yang demikian, Bandung selatan sangat rentan terhadap masalah banjir terutama
      pada musim hujan.
    </p>
 
    <h2 id="wisata">Wisata</h2>
    <p>
      Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan utama dalam menikmati
      liburan akhir pekan terutama dari masyarakat yang berasal dari Jakarta sekitarnya. Selain
      menjadi kota wisata belanja, kota Bandung juga dikenal dengan sejumlah besar bangunan lama
      berarsitektur peninggalan Belanda.
    </p>
 
    <h3>Farm House Lembang</h3>
    <img src="assets/image/farm-house.jpg" alt="farm house" />
    <p>
      Berada di jalur utama Bandung-Lembang, Farm House menjadi objek wisata yang tidak pernah sepi
      pengunjung. Selain karena letaknya strategis, kawasan ini juga menghadirkan nuansa wisata khas
      Eropa. Semua itu diterapkan dalam bentuk spot swafoto Instagramable.
    </p>
 
    <h3>Observatorium Bosscha</h3>
    <img src="assets/image/bosscha.jpg" alt="bosscha" />
    <p>
      Memiliki beberapa teleskop, antara lain, Refraktor Ganda Zeiss, Schmidt Bimasakti, Refraktor
      Bamberg, Cassegrain GOTO, dan Teleskop Surya. Refraktor Ganda Zeiss adalah jenis teleskop
      terbesar untuk meneropong bintang. Benda ini diletakkan pada atap kubah sehingga saat teropong
      digunakan, atap tersebut harus dibuka. Observatorium Bosscha boleh dikunjungi oleh siapapun,
      tanpa tiket. Namun, bagi yang ingin menggunakan teleskop Zeiss, wajib mendaftarkan diri. Untuk
      instansi atau lembaga pendidikan, diberikan jadwal hari Selasa sampai Jumat. Sementara itu,
      kunjungan individu dibuka setiap hari Sabtu.
    </p>
  </div>
 
 
  <!-- Konten samping -->
  <aside>
    <h2>Kota Bandung</h2>
    <p>Kota Kembang Paris van Java</p>
    <figure>
      <img src="assets/image/bandung-badge.png" />
      <figcaption>Lambang</figcaption>
    </figure>
  </aside>
</main>`}
</CodeBlock>

Dengan begitu, konten elemen `<main>` terbagi menjadi dua, yaitu elemen `<div>` dan `<aside>`. Selanjutnya, kita mulai kelompokkan konten lebih detail lagi pada elemen `<div>`. Jadi, silakan **fokus** saja pada elemen tersebut untuk langkah selanjutnya.

3. Dalam elemen ini (`<div>`), ada konten yang dapat digolongkan sebagai artikel. Artikel pertama memuat konten mengenai sejarah, berikutnya mengenai geografi, dan terakhir mengenai wisata. Dengan hasil identifikasi tersebut, kita memerlukan tiga buah elemen `<article>` untuk membungkus masing-masing konten tersebut. Masing-masing elemen `<article>` akan terdiri dari heading, gambar, dan paragraf.

<CodeBlock className="no-copy">
{`<div>
  <article>
    <h2 id="sejarah">Sejarah</h2>
    <img src="assets/image/history.jpg" alt="sejarah" />
    <p>
      Kata Bandung berasal dari kata bendung atau bendungan karena terbendungnya sungai Citarum oleh
      lava Gunung Tangkuban Parahu yang lalu membentuk telaga. Legenda yang diceritakan oleh
      orang-orang tua di Bandung mengatakan bahwa nama Bandung diambil dari sebuah kendaraan air
      yang terdiri dari dua perahu yang diikat berdampingan yang disebut perahu bandung yang
      digunakan oleh Bupati Bandung, R.A. Wiranatakusumah II, untuk melayari Ci Tarum dalam mencari
      tempat kedudukan kabupaten yang baru untuk menggantikan ibu kota yang lama di Dayeuhkolot.
    </p>
 
    <p>
      Berdasarkan filosofi Sunda, kata Bandung juga berasal dari kalimat Nga-Bandung-an Banda
      Indung, yang merupakan kalimat sakral dan luhur karena mengandung nilai ajaran Sunda.
      Nga-Bandung-an artinya menyaksikan atau bersaksi. Banda adalah segala sesuatu yang berada di
      alam hidup yaitu di bumi dan atmosfer, baik makhluk hidup maupun benda mati. Sinonim dari
      banda adalah harta. Indung berarti Ibu atau Bumi, disebut juga sebagai Ibu Pertiwi tempat
      Banda berada.
    </p>
  </article>
 
  <article>
    <h2 id="geografis">Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="geografis" />
    <p>
      Kota Bandung dikelilingi oleh pegunungan, sehingga bentuk morfologi wilayahnya bagaikan sebuah
      mangkok raksasa,[9] secara geografis kota ini terletak di tengah-tengah provinsi Jawa Barat,
      serta berada pada ketinggian ±768 m di atas permukaan laut, dengan titik tertinggi di berada
      di sebelah utara dengan ketinggian 1.050 meter di atas permukaan laut dan sebelah selatan
      merupakan kawasan rendah dengan ketinggian 675 meter di atas permukaan laut.
    </p>
 
    <p>
      Kota Bandung dialiri dua sungai utama, yaitu Sungai Cikapundung dan Sungai Citarum beserta
      anak-anak sungainya yang pada umumnya mengalir ke arah selatan dan bertemu di Sungai Citarum.
      Dengan kondisi yang demikian, Bandung selatan sangat rentan terhadap masalah banjir terutama
      pada musim hujan.
    </p>
  </article>
 
  <article>
    <h2 id="wisata">Wisata</h2>
    <p>
      Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan utama dalam menikmati
      liburan akhir pekan terutama dari masyarakat yang berasal dari Jakarta sekitarnya. Selain
      menjadi kota wisata belanja, kota Bandung juga dikenal dengan sejumlah besar bangunan lama
      berarsitektur peninggalan Belanda.
    </p>
 
    <h3>Farm House Lembang</h3>
    <img src="assets/image/farm-house.jpg" alt="farm house" />
    <p>
      Berada di jalur utama Bandung-Lembang, Farm House menjadi objek wisata yang tidak pernah sepi
      pengunjung. Selain karena letaknya strategis, kawasan ini juga menghadirkan nuansa wisata khas
      Eropa. Semua itu diterapkan dalam bentuk spot swafoto Instagramable.
    </p>
 
    <h3>Observatorium Bosscha</h3>
    <img src="assets/image/bosscha.jpg" alt="bosscha" />
    <p>
      Memiliki beberapa teleskop, antara lain, Refraktor Ganda Zeiss, Schmidt Bimasakti, Refraktor
      Bamberg, Cassegrain GOTO, dan Teleskop Surya. Refraktor Ganda Zeiss adalah jenis teleskop
      terbesar untuk meneropong bintang. Benda ini diletakkan pada atap kubah sehingga saat teropong
      digunakan, atap tersebut harus dibuka. Observatorium Bosscha boleh dikunjungi oleh siapapun,
      tanpa tiket. Namun, bagi yang ingin menggunakan teleskop Zeiss, wajib mendaftarkan diri. Untuk
      instansi atau lembaga pendidikan, diberikan jadwal hari Selasa sampai Jumat. Sementara itu,
      kunjungan individu dibuka setiap hari Sabtu.
    </p>
  </article>
</div>`}
</CodeBlock>

4. Penambahan elemen terakhir untuk elemen `<div>`. Kita akan mengelompokkan konten lagi dengan elemen `<section>`. Perhatikan pada elemen `<article>` terakhir (topik wisata), konten tersebut memiliki dua subjudul, yaitu wisata Farm House dan Observatorium Bosscha. Oleh karena itu, kita dapat mengelompokkan juga pada kedua konten ini dengan menggunakan elemen `<section>`.
<CodeBlock className="no-copy">
{`<div>
  <article>
    <h2 id="sejarah">Sejarah</h2>
    <img src="assets/image/history.jpg" alt="sejarah" />
    <p>
      Kata Bandung berasal dari kata bendung atau bendungan karena terbendungnya sungai Citarum oleh
      lava Gunung Tangkuban Parahu yang lalu membentuk telaga. Legenda yang diceritakan oleh
      orang-orang tua di Bandung mengatakan bahwa nama Bandung diambil dari sebuah kendaraan air
      yang terdiri dari dua perahu yang diikat berdampingan yang disebut perahu bandung yang
      digunakan oleh Bupati Bandung, R.A. Wiranatakusumah II, untuk melayari Ci Tarum dalam mencari
      tempat kedudukan kabupaten yang baru untuk menggantikan ibu kota yang lama di Dayeuhkolot.
    </p>
 
    <p>
      Berdasarkan filosofi Sunda, kata Bandung juga berasal dari kalimat Nga-Bandung-an Banda
      Indung, yang merupakan kalimat sakral dan luhur karena mengandung nilai ajaran Sunda.
      Nga-Bandung-an artinya menyaksikan atau bersaksi. Banda adalah segala sesuatu yang berada di
      alam hidup yaitu di bumi dan atmosfer, baik makhluk hidup maupun benda mati. Sinonim dari
      banda adalah harta. Indung berarti Ibu atau Bumi, disebut juga sebagai Ibu Pertiwi tempat
      Banda berada.
    </p>
  </article>
 
  <article>
    <h2 id="geografis">Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="geografis" />
    <p>
      Kota Bandung dikelilingi oleh pegunungan, sehingga bentuk morfologi wilayahnya bagaikan sebuah
      mangkok raksasa,[9] secara geografis kota ini terletak di tengah-tengah provinsi Jawa Barat,
      serta berada pada ketinggian ±768 m di atas permukaan laut, dengan titik tertinggi di berada
      di sebelah utara dengan ketinggian 1.050 meter di atas permukaan laut dan sebelah selatan
      merupakan kawasan rendah dengan ketinggian 675 meter di atas permukaan laut.
    </p>
 
    <p>
      Kota Bandung dialiri dua sungai utama, yaitu Sungai Cikapundung dan Sungai Citarum beserta
      anak-anak sungainya yang pada umumnya mengalir ke arah selatan dan bertemu di Sungai Citarum.
      Dengan kondisi yang demikian, Bandung selatan sangat rentan terhadap masalah banjir terutama
      pada musim hujan.
    </p>
  </article>
 
  <article>
    <h2 id="wisata">Wisata</h2>
    <p>
      Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan utama dalam menikmati
      liburan akhir pekan terutama dari masyarakat yang berasal dari Jakarta sekitarnya. Selain
      menjadi kota wisata belanja, kota Bandung juga dikenal dengan sejumlah besar bangunan lama
      berarsitektur peninggalan Belanda.
    </p>
 
    <section>
      <h3>Farm House Lembang</h3>
      <img src="assets/image/farm-house.jpg" alt="farm house" />
      <p>
        Berada di jalur utama Bandung-Lembang, Farm House menjadi objek wisata yang tidak pernah
        sepi pengunjung. Selain karena letaknya strategis, kawasan ini juga menghadirkan nuansa
        wisata khas Eropa. Semua itu diterapkan dalam bentuk spot swafoto Instagramable.
      </p>
    </section>
 
    <section>
      <h3>Observatorium Bosscha</h3>
      <img src="assets/image/bosscha.jpg" alt="bosscha" />
      <p>
        Memiliki beberapa teleskop, antara lain, Refraktor Ganda Zeiss, Schmidt Bimasakti, Refraktor
        Bamberg, Cassegrain GOTO, dan Teleskop Surya. Refraktor Ganda Zeiss adalah jenis teleskop
        terbesar untuk meneropong bintang. Benda ini diletakkan pada atap kubah sehingga saat
        teropong digunakan, atap tersebut harus dibuka. Observatorium Bosscha boleh dikunjungi oleh
        siapapun, tanpa tiket. Namun, bagi yang ingin menggunakan teleskop Zeiss, wajib mendaftarkan
        diri. Untuk instansi atau lembaga pendidikan, diberikan jadwal hari Selasa sampai Jumat.
        Sementara itu, kunjungan individu dibuka setiap hari Sabtu.
      </p>
    </section>
  </article>
</div>`}
</CodeBlock>

5. Mantap! Konten sudah terstruktur dengan lebih baik. Jika penasaran, kamu dapat menjalankan halaman ini jika ingin melihat hasilnya. Namun, tidak ada perubahan yang terlihat pada tampilannya. Nah, kamu bisa mencoba melihatnya pada Inspect Element pada tab Browser.
6. Itulah yang telah kita lakukan sampai langkah ini. Setelah penggolongan konten dilakukan, ada hal yang dapat kita tingkatkan. Sebelumnya, kita sudah menetapkan atribut id pada elemen `<h2>` sebagai target navigasi. Kita perlu memindahkan penamaan atau pemberian atribut id dari masing-masing elemen `<h2>` ke elemen `<article>`. Hal ini karena elemen `<article>` lebih merepresentasikan keseluruhan dari konten artikelnya.

Sebelum melakukannya, kita juga akan menambahkan atribut id pada elemen `<div>` sebagai pembungkus konten utama. Hal ini ditujukan untuk mempermudah proses layouting (penataan elemen) dengan styling.

Silakan sesuaikan kodenya dengan kode berikut.

<CodeBlock className="no-copy">
{`<div id="content">
  <article id="sejarah">
    <h2>Sejarah</h2>
    <img src="assets/image/history.jpg" alt="sejarah" />
    <!-- Kode lainnya disembunyikan... -->
  </article>
 
  <article id="geografis">
    <h2>Geografis</h2>
    <img src="assets/image/geografis.jpg" alt="geografis" />
 
    <!-- Kode lainnya disembunyikan -->
  </article>
 
  <article id="wisata">
    <h2>Wisata</h2>
    <p>
      Sejak dibukanya Jalan Tol Cipularang, kota Bandung telah menjadi tujuan utama dalam menikmati
      liburan akhir pekan terutama dari masyarakat yang berasal dari Jakarta sekitarnya. Selain
      menjadi kota wisata belanja, kota Bandung juga dikenal dengan sejumlah besar bangunan lama
      berarsitektur peninggalan Belanda.
    </p>
 
    <!-- Kode lainnya disembunyikan -->
  </article>
</div>`}
</CodeBlock>

7. Sip! Kita sudah selesai dengan elemen `<div>` yang sekarang memiliki atribut id. Sekarang, kita beralih ke elemen `<aside>.` Konten dalam elemen ini tidak terlalu kompleks dan banyak seperti elemen `<div id="content">`. Jadi, kita cukup mengelompokkannya dengan satu elemen `<article>` saat ini.

Silakan sesuaikan kode dalam elemen `<aside>` menjadi seperti kode berikut.
<CodeBlock className="no-copy">
{`<aside>
  <article>
    <h2>Kota Bandung</h2>
    <p>Kota Kembang Paris van Java</p>
    <figure>
      <img src="assets/image/bandung-badge.png" />
      <figcaption>Lambang</figcaption>
    </figure>
  </article>
</aside>`}
</CodeBlock>

8. Sekarang, konten sudah terorganisasi dengan baik. Sampai sejauh ini, seharusnya struktur pada elemen `<main>` akan tampak seperti diagram berikut.
![final](https://assets.cdn.dicoding.com/original/academy/dos:8f145a8eff3f255682004b734a0f41c720230620063103.jpeg)

## Latihan: Menerapkan Elemen Tabel pada Halaman Profil

### Alur Latihan

Berikut adalah alur latihan kali ini.

1. Membuka hasil latihan terakhir dengan VSCode.
2. Membungkus elemen-elemen yang ada saat ini dengan `<header>`.
3. Menambahkan konten-konten baru dengan elemen `<section>`.
4. Menampilkan konten-konten yang baru dengan elemen `<table>`.
5. Menjalankan dokumen HTML pada browser.

### Latihan Identifikasi Elemen pada Halaman Website
1. Silakan buka proyek Halaman Profil terakhir dengan VSCode. 
2. Sebelum kita menambahkan konten ke HTML, mari kita atur kembali struktur elemen dalam elemen `<aside>` tersebut. Saat ini, elemen `<aside>` memiliki struktur seperti berikut.
![aside](https://assets.cdn.dicoding.com/original/academy/dos:0ced0ed3101698a89c6b1e2aeac340e020230620064912.jpeg)
3. Kita perlu mengelompokkan kembali elemen yang ada di dalam elemen `<article>` karena akan menambahkan konten lain. Kelompokkan seluruh elemen yang ada pada elemen `<article>` saat ini sebagai header dan tambahkan elemen baru di bawah elemen header tersebut, yaitu `<section>`.

Pada elemen `<section>`, konten tabel akan ditempatkan. Silakan buka kembali berkas index.html dan sesuaikan struktur elemen `<aside> `seperti berikut.
<CodeBlock className="no-copy">
{`<aside>
  <article>
    <header>
      <h2>Kota Bandung</h2>
      <p>Kota Kembang Paris van Java</p>
      <figure>
        <img src="assets/image/bandung-badge.png" />
        <figcaption>Lambang</figcaption>
      </figure>
    </header>
 
    <section>
      <!-- Konten-konten baru -->
    </section>
  </article>
</aside>`}
</CodeBlock>

4. Struktur elemen pada elemen `<aside>` akan menjadi seperti bagan berikut.
![aside](https://assets.cdn.dicoding.com/original/academy/dos:15b1015b7f081601b2fb261fa1f2e5ee20230620065016.jpeg)
5. Sip, lanjut! Pada elemen `<section>`, kita masukkan konten berikut padanya.
```
Informasi Lainnya


Negara

Indonesia


Hari jadi
25 September 1810


Luas Total

167.67 km2


Bahasa Daerah

Sunda


Kode Telepon

+62 22
```
6. Itulah konten yang akan ditampilkan dalam `<aside>`. Sesuaikan konten tersebut dengan menerapkan elemen yang tepat, salah satunya gunakan elemen tabel untuk menampung sebagian kontennya. Silakan sesuaikan kodenya dengan kode bercetak tebal berikut.
<CodeBlock className="no-copy">
{`<aside>
  <article>
    <header>
      <!-- Kode lainnya disembunyikan... -->
    </header>
 
    <section>
      <h3>Informasi Lainnya</h3>
 
      <table>
        <tr>
          <th>Negara</th>
          <td>Indonesia</td>
        </tr>
        <tr>
          <th>Hari jadi</th>
          <td>25 September 1810</td>
        </tr>
        <tr>
          <th>Luas Total</th>
          <td>167.67 km<sup>2</sup></td>
        </tr>
        <tr>
          <th>Bahasa Daerah</th>
          <td>Sunda</td>
        </tr>
        <tr>
          <th>Kode Telepon</th>
          <td>+62 22</td>
        </tr>
      </table>
    </section>
  </article>
</aside>`}
</CodeBlock>

7. Hasilnya akan seperti berikut setelah dijalankan.
![HTML Meme - 1](/img/1/finalHTML.png)
