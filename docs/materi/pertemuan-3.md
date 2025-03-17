---
sidebar_label: "Pertemuan 3: Pengenalan dan Pendalaman CSS"
sidebar_position: 3
Path: docs/materi/pertemuan-3
---

# Pertemuan 3: Pengenalan dan Pendalaman CSS

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Pengantar Pengenalan CSS

Website tampak begitu membosankan dan “mengerikan” tanpa adanya CSS. CSS atau Cascading Style Sheet merupakan standar dari W3C untuk mengatur visualisasi berkas yang ditulis pada HTML. CSS hanya sebuah declarative language yang digunakan untuk mendeklarasikan suatu nilai yang nantinya digunakan untuk mengatur tampilan sebuah elemen HTML pada browser.

![css](https://assets.cdn.dicoding.com/original/academy/dos:84f592e1c421791ca590bfdaddc2691820231130101940.png)

### Keuntungan dan Cara CSS Bekerja

Dengan menerapkan CSS, tampilan website kita akan lebih menarik. Berikut adalah beberapa keuntungan yang didapatkan ketika kita menerapkan CSS.

- Dapat mengontrol dan menerapkan layout secara presisi.
  Dengan menggunakan CSS kita bisa membuat sebuah website seperti dokumen cetak dengan desain yang menarik dan presisi.

- Menghindari pekerjaan yang berulang-ulang dalam menerapkan styling.
  Kita dapat menetapkan styling pada beberapa berkas HTML hanya dengan menggunakan satu berkas CSS.

- Didukung banyak browser.
  Seluruh browser saat ini minimal sudah mendukung CSS versi 2. Untuk browser yang populer, seperti Chrome dan Firefox, sudah mendukung CSS versi 3.

### Menulis Aturan Styling

Pada penggunaan CSS, ada dua bagian dalam sebuah rule. Pertama adalah identitas elemen atau elemen yang akan menerapkan rule (singkatnya kita akan sebut selector). Kedua adalah deklarasi atau instruksi yang akan diterapkan pada sebuah selector.

![style](https://assets.cdn.dicoding.com/original/academy/dos:d62420ba96cd1b764eab1ad1f644e42b20231130101852.jpeg)

### Melampirkan Styling pada Dokumen HTML

Berikut adalah cara melampirkan styling pada dokumen HTML.

**External Style Sheet**

External Style Sheet adalah berkas terpisah yang di dalamnya hanya ada CSS rules. Berkas ini harus berekstensi **.css**, dan akan dihubungkan dengan dokumen HTML. Cara ini merupakan yang paling powerful dalam menerapkan styling. Dengan cara ini, satu berkas styling (.css) dapat digunakan oleh banyak berkas HTML.

```
<head>
  <meta charset="UTF-8" />
  <title>Judul Dokumen</title>

  <!-- Impor berkas CSS Anda -->
  <link rel="stylesheet" href="style.css">
</head>
```

**Embedded Style Sheet**

Embedded Style Sheet adalah kumpulan rules yang dituliskan dalam berkas HTML dengan menggunakan elemen `<style>`. Penulisan rules harus dituliskan dalam elemen `<style>` dan biasanya ditempatkan dalam `<head>` pada berkas HTML.

```
<head>
  <meta charset="UTF-8" />
  <title>Judul Dokumen</title>

  <style>
    h1 {
      color: green;
    }
  </style>
</head>
```

**Inline Style**

Inline Style adalah styling yang diterapkan pada elemen HTML dengan menggunakan atribut style. Contohnya seperti berikut

```
<nama-elemen style="color: green">Konten dari Elemen HTML</nama-elemen>
```

Untuk menambahkan styling properties lainnya (multiple properties), kita tuliskan dengan menggunakan semicolon (;) sebagai pemisah antar styling properties-nya.

## CSS Conception

Sebelum membahas styling lebih detail, ada beberapa konsepsi dalam CSS yang harus kita pahami.

## Inheritance

Styling HTML bersifat inheritance yang berarti dapat mewarisi properti style “tertentu” dari suatu elemen ke elemen-elemen di dalamnya (child-elements).

Contohnya, CSS rules yang ditetapkan untuk elemen `<body>` akan diterapkan pada seluruh child-elements secara otomatis. Contoh lainnya, CSS rules yang diterapkan pada elemen `<footer>` dengan properti `color: white` akan diterapkan pada seluruh elemen yang ada di dalamnya. Hal ini menjadi alasan memahami struktur dokumen itu penting.

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8" />
  <title>CSS Inheritance Example</title>

  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header>
    <h1>Inheritance di CSS</h1>
  </header>
  <main>
    <h2>Lorem Ipsum</h2>

    <article>
      <h3>Lorem, ipsum dolor.</h3>
      <p>
        Pellentesque venenatis mi sit amet erat tincidunt auctor. Curabitur tincidunt tellus ac
        convallis dictum. Morbi luctus leo eget leo luctus elementum. Cras at ligula eu elit
        blandit venenatis.
      </p>
    </article>
  </main>
  <footer>
    <p>Hak Cipta &copy; 2023</p>
  </footer>
</body>
</html>
```

```
body {
  font-family: sans-serif;
}

footer {
  color: white;
}
```

Berikut adalah hasil penerapan contoh studi kasus di atas.
![hasil](https://assets.cdn.dicoding.com/original/academy/dos:5d3f2decf2f8867f95bb3811cde1fce420230620091211.jpeg)

### Group Selector

Jika beberapa selector yang berbeda memiliki penerapan properti-propeti yang sama, kita dapat menggabungkannya menggunakan group selector. Hal ini dapat meminimalkan penulisan kode yang berulang.

```
h2 {
  color: #00A2C6;
}

h3 {
  color: #00A2C6;
}
```

Jika terdapat kasus seperti di atas, kita dapat menuliskan dua selector sekaligus dalam satu struktur rule. Gunakan tanda koma (,) untuk memisahkan tiap selector-nya.

Silakan perhatikan contoh kasus berikut.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <h2>Judul dengan Heading 2</h2>
    <h3>Judul dengan Heading 3</h3>
  </body>
</html>
```

```
h2, h3 {
  color: #00A2C6;
}
```

## Rule Order

Sesuai dengan namanya, cascading artinya “mengalir”. Demikian halnya dengan alur kerja CSS dalam membaca kode, mengalir dari atas ke bawah. Oleh karena itu, kita harus memperhatikan urutan dalam penulisan rules, terutama saat terjadi sebuah konflik. Konflik dapat terjadi karena kita menerapkan beberapa styling pada satu dokumen HTML dan menimpa styling yang telah diterapkan sebelumnya, baik disadari maupun tidak.

Contohnya, apa yang akan ditampilkan oleh browser ketika eksternal css mengharuskan elemen `<p>` menampilkan warna merah, tetapi pada embedded css `<p>` harus menampilkan warna biru? Kembali pada alur kerja CSS yang membaca dari atas ke bawah sehingga warna yang akan diterapkan adalah warna yang paling akhir didefinisikan.

Untuk lebih jelasnya, kita bisa lihat contoh berikut.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css">

    <style>
      p {
        color: blue;
      }
    </style>
  </head>
  <body>
    <p>
      Sesuai dengan namanya cascading yang artinya <q>mengalir</q>, alur kerja CSS dalam membaca
      kode pun seperti itu. Mengalir dari atas ke bawah sehingga kita harus memperhatikan urutan
      dalam penulisan rules <i>styling</i>.
    </p>
  </body>
</html>
```

```
p {
  color: red;
}
```

Namun, kita bisa membuat sebuah **property styling** agar dianggap penting oleh browser untuk diterapkan dan urutan tidak diperhatikan. Kita bisa menambahkan keyword !important pada akhir nilai propertinya.

```
p {
  color: red !important;
}
```

Gunakan !important ketika memang benar-benar dibutuhkan saja. Sebaiknya kita pahami aturan urutan pada CSS dengan baik sehingga meminimalisir penggunaan tanda tersebut.

Berikut adalah catatan yang sudah kita pelajari sejauh ini tentang **styling**.

- **Rule**: Sebuah aturan styling yang harus diterapkan pada elemen HTML. Dalam sebuah rule, ada selector dan deklarasi properti styling.

- **Selector**: Bagian yang mengidentifikasi target elemen untuk menetapkan sebuah rule.

- **Declaration**: Sebuah bagian dari rule yang terdiri dari pasangan properti dan nilainya.

- **External Style Sheet**: Berkas terpisah yang di dalamnya hanya ada satu atau lebih rules yang akan digunakan pada website.

- **Embedded Style Sheet**: Kumpulan rules yang dituliskan dalam berkas HTML dengan menggunakan elemen `<style>`.

- **Inline Style**: Styling yang diterapkan pada elemen HTML dengan menggunakan atribut style.

## Pengantar Pendalaman CSS

Nah, kita akan berkenalan lebih dalam dan jauh lagi tentang CSS pada modul ini. Kita akan belajar beberapa hal, seperti mengenal berbagai macam tipe selector, formatting text, pewarnaan, box model, positioning, hingga penyusunan layout pada website menggunakan teknik floating.

## Selector Dasar: Type Selector, dan Class Selector

Ada banyak jenis selector untuk menargetkan aturan ke elemen tertentu dalam dokumen HTML. Pada modul sebelumnya, kita sudah mengetahui salah satu cara dasar dalam menggunakan selector. Sekarang, mari kita bahas lebih detail mengenai macam macam selector yang ada.

Pada modul sebelumnya, kita sudah mengetahui pengertian selector dan cara menggunakannya. Hal yang kita gunakan tersebut merupakan basic selector. Sebenarnya, ada beberapa macam lagi dari basic selector sebagai berikut.

- Type Selector
- Class Selector
- ID Selector
- Attribute Selector
- Universal Selector

Mari kita bahas satu per satu tipe basic selector yang ada.

### Type Selector

Type Selector menggunakan nama elemen sebagai target untuk diterapkannya rule. Dalam kata lain, ketika menggunakan selector ini tentu rule akan diterapkan pada seluruh elemen target yang ada pada dokumen HTML. Contohnya sebagai berikut.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <span>
      Ini merupakan sebuah teks yang berada pada elemen span. Seharusnya elemen
      ini ditampilkan dengan warna teks merah.
    </span>
    <p>
      Ini merupakan sebuah teks yang berada pada elemen paragraf, teks ini tidak
      seharusnya tidak akan terpengaruh oleh rule.
    </p>
    <span>
      Ini merupakan sebuah teks yang berada pada elemen span lainnya. Seharusnya
      elemen ini ditampilkan dengan warna teks merah juga.
    </span>
  </body>
</html>
```

```
/* Semua elemen span */
span {
  color: red;
}
```

Jika berkas tersebut dibuka pada browser, teks yang berada pada setiap elemen `<span>` akan berwarna merah.

### Class Selector

Class selector menetapkan target elemen berdasarkan nilai dari atribut **class** yang diterapkan pada elemennya. Untuk penulisan selector-nya diawali dengan tanda titik (.) dan dilanjutkan dengan nama class-nya. Contohnya berikut.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p class="red">Paragraf dengan teks berwarna merah</p>
    <p class="skyblue-bg">Paragraf dengan background berwarna biru langit</p>
    <p class="fancy">Paragraf dengan gaya fancy</p>
    <p>
      Paragraf yang menampilkan teks dengan warna standar tanpa menerapkan
      styling
    </p>
  </body>
</html>
```

```
.red {
  color: red;
}

.skyblue-bg {
  background-color: skyblue;
}

.fancy {
  font-weight: bold;
  text-shadow: 4px 4px 3px #77f;
}
```

## Selector Dasar: ID Selector, Attribute Selector, dan Universal Selector

CSS memiliki banyak variasi untuk menuliskan selector. Tidak hanya dua tipe selector dasar sebelumnya, tetapi ada tiga selector dasar lainnya yang dapat kita gunakan. Mari kita pelajari mereka.

### ID Selector

ID selector menetapkan target elemen berdasarkan nilai dari atribut **id** yang diterapkan pada elemennya. Mirip dengan class, atribut **id** dapat diterapkan pada seluruh elemen HTML dan kebanyakan atribut ini digunakan untuk memberikan sebuah arti pada _generic element_, seperti `<div`> dan `<span>`. Namun, atribut id ini tidak bersifat _shareable_. Artinya, nilai id harus unik dan digunakan pada satu elemen saja.

Untuk menetapkan selector dengan menggunakan id, kita gunakan tanda _octothorpe_ (#) atau lebih familiar disebut dengan _hash_. Berikut contohnya.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div id="special">
      <p>Ini merupakan konten di dalam sebuah div yang diberi id special.</p>
    </div>
    <div>
      <p>Ini merupakan konten di dalam sebuah div biasa.</p>
    </div>
  </body>
</html>
```

```
#special {
  background-color: skyblue;
}
```

> Hal yang harus ditekankan lagi adalah id ini bersifat unik. Jika ingin menerapkan sebuah rule pada banyak elemen, sebaiknya gunakan atribut class dibandingkan dengan id.

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Judul Dokumen</title>
    <style>
      #special {
        background-color: skyblue;
      }
    </style>
  </head>
  <body>
    <div id="special">
      <p>Ini merupakan konten di dalam sebuah div yang diberi id special.</p>
    </div>

    <!-- ini merupakan contoh yang salah dalam penerapan id -->
    <div id="special">
      <p>Ini merupakan konten di dalam sebuah div biasa.</p>
    </div>
  </body>
</html>
```

### Attribute Selector

Attribute selector merupakan cara menetapkan target elemen berdasarkan sebuah atribut yang digunakan atau bahkan bisa lebih spesifik dengan nilainya. Contohnya sebagai berikut.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Attribute Selector</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <ul>
      <li><a href="#internal">Internal link</a></li>
      <li><a href="http://example.com">Example link</a></li>
      <li><a href="#InSensitive">Insensitive internal link</a></li>
      <li><a href="http://example.org">Example org link</a></li>
    </ul>
  </body>
</html>
```

```
ul {
  font-size: 18px;
}

/* <a> element yang menerapkan href attribute */
a[href] {
  color: blue;
}

/* <a> element yang menerapkan nilai pada href dengan awalan "#" */
a[href^='#'] {
  background-color: gold;
}

/* <a> element yang menerapkan nilai pada href yang mengandung teks "example" */
a[href*='example'] {
  background-color: silver;
}

/* <a> element yang menerapkan nilai pada href yang mengandung teks "insensitive" tidak mementingkan huruf kapital*/
a[href*='insensitive' i] {
  color: cyan;
}

/* <a> element yang menerapkan nilai pada href dengan akhiran ".org" */
a[href$='.org'] {
  color: red;
}
```

### Universal Selector

Universal selector digunakan untuk diterapkan pada seluruh elemen. Namun, selector ini juga bisa secara spesifik menargetkan sebuah elemen dengan menggabungkannya bersama selector yang lain. Berikut contohnya.

```
<!DOCTYPE html>
<html lang="id">
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p>
      Ini merupakan paragraf biasa atau tidak menerapkan atribut apapun. Maka
      teks pada paragraf ini akan berwarna hijau
    </p>
    <p lang="en-us">
      This is an English paragraph contains en-us value of lang attribute, so
      this text will be green and italic.
    </p>

    <h1>Ini merupakan sebuah header biasa</h1>
    <h1 lang="en-us">This is an English Header</h1>

    <p class="warning">
      Perhatikan paragraf ini! Paragraf ini merupakan paragraf yang memiliki
      kelas bernilai warning, sehingga teks dari paragraf ini akan berwarna
      merah
    </p>

    <div id="content">
      <p>
        Ini merupakan sebuah teks di dalam sebuah div yang memiliki id bernilai
        "content", seharusnya paragraf ini dibungkus dalam border yang memiliki
        padding 20px
      </p>
    </div>
  </body>
</html>
```

```
/* Menargetkan seluruh tipe elemen */
* {
  color: green;
}

/* Menargetkan seluruh tipe elemen yang mengandung nilai "en" pada atribut lang */
*[lang^='en'] {
  font-style: italic;
}

/* Menargetkan seluruh tipe elemen yang memiliki nilai "warning" pada atribut class */
*.warning {
  color: red;
}

/* Menargetkan seluruh tipe elemen yang memiliki nilai "content" pada atribut id */
*#content {
  border: 1px solid blue;
  padding: 20px;
}
```

## Box Model

![box](https://assets.cdn.dicoding.com/original/academy/dos:9bea45b1dd455e025be015826f5c998920230620195613.jpeg)
Setiap elemen yang dibuat pada HTML akan menciptakan sebuah kotak untuk menampung kontennya. Layaknya bentuk kotak pada umumnya, ada beberapa nilai atau komponen padanya.

- Lebar dan tinggi pada kotak (konten).
- Ruang kosong antara konten dengan border (padding).
- Garis tepi (border).
- Jarak dari elemen lain (margin).

Pada CSS, kita dapat mengatur nilai-nilai tersebut. Inilah yang disebut dengan box model.

## Apa itu Box Element

![boxelement](https://assets.cdn.dicoding.com/original/academy/dos:1f4b7794e421dbef4fa88ea7a007a52320230621113053.jpeg)
Sebagaimana yang kita lihat pada gambar di atas, setiap elemen pada HTML, baik block-level maupun inline-level, akan menghasilkan kotak elemen.

Berikut adalah penjelasan dari gambar di atas.

- **Content**: konten dari elemen itu sendiri.
- **Padding**: area yang menjadi jarak antara border elemen dengan konten yang ditampilkan.
- **Border**: garis yang mencakup konten beserta padding.
- **Margin**: area jarak di luar border.
- **Edge of Element**: batas dari suatu elemen.

## Box Model: Box Dimensions

Konsep pertama yang akan kita bahas pada box model adalah dimensi dari elemen. Tidak hanya dimensi, kita juga akan membahas beberapa hal yang berkaitan dengan konten seperti overflow content dan box-sizing. Apa itu mereka dan bagaimana penerapannya? Mari kita pelajari bersama.

### Dimension

Standarnya, sebuah box yang dihasilkan tiap elemen selalu cukup untuk menampung konten. Namun, kita dapat mengatur nilai dimensi dari box tersebut dengan properti width dan height.

Cara yang paling banyak digunakan dalam menentukan dimensi kotak adalah menggunakan piksel, persentase, atau em. Secara tradisional, piksel merupakan cara yang paling populer karena kita dapat merancang dan mengontrol ukuran secara akurat.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="box">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Natus officiis perspiciatis quidem
        ratione? Distinctio eos ex expedita iusto necessitatibus velit, veritatis. Aliquid, debitis
        dignissimos in iusto magnam nulla sed tempora.
      </p>
    </div>
  </body>
</html>
```

```
.box {
  height: 300px;
  width: 300px;
  background-color: #11c5c6;
}

p {
  height: 75%;
  width: 75%;
  background-color: #fbdd1c;
}
```

### Limiting Dimension

Beberapa website yang ada sekarang menampilkan layout yang dapat melebar dan menyempit mengikuti ukuran layar pengguna. Pada prinsip tampilan tersebut, mungkin kita memerlukan sebuah limitasi ukuran yang harus ditetapkan agar konten selalu ditampilkan secara proporsional. Untuk melakukannya kita manfaatkan properti min-width dan max-width.

- **min-width**: menetapkan nilai lebar minimal yang harus dimiliki elemen.
- **max-width**: menetapkan nilai lebar maksimal yang harus dimiliki elemen.

Keduanya merupakan properti yang sangat membantu untuk memastikan konten halaman dapat terbaca oleh pengguna (terutama ketika pengguna menggunakan ponsel). Misalnya, kita dapat menggunakan properti max-width untuk memastikan bahwa baris teks yang muncul tidak terlalu lebar.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="content">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Cupiditate eius explicabo fuga
        iusto magni minus odit praesentium, quasi quisquam quos repellat suscipit tempora tenetur?
        Assumenda cum laborum officiis quos ratione.
      </p>
    </div>
  </body>
</html>
```

```
.content {
  max-width: 800px;
  height: 400px;

  margin-left: auto;
  margin-right: auto;
  background-color: deeppink;
}

p {
  font-size: 1.5em;
  font-weight: bold;
}
```

### Overflowing Content

Dimensi box yang dihasilkan elemen selalu cukup untuk menampung konten, tetapi hal ini tidak berlaku jika kita tetapkan secara manual panjang dan lebarnya. Tak jarang terjadi overflow ketika kita menerapkan ukuran pada elemen dengan konten di dalamnya yang begitu banyak.

Contohnya berikut.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab accusantium amet corporis
        cupiditate dignissimos error expedita explicabo facere facilis, ipsam itaque libero modi
        officiis optio perspiciatis provident quam sequi voluptatem.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. At aut corporis facere harum
        inventore iure, quisquam recusandae reprehenderit veritatis voluptatum. Ducimus
        exercitationem illo nam sapiente suscipit, tenetur ullam ut voluptas!
      </p>
    </div>
  </body>
</html>
```

```
div {
  height: 200px;
  width: 200px;
  background-color: lightgreen;
}
```

Untuk menangani kasus seperti ini kita bisa gunakan properti overflow, properti ini dapat bernilai berikut.

- **visible**

Visible merupakan nilai default pada properti ini. Konten yang tidak tertampung (overflow) akan tetap ditampilkan seperti pada standarnya.

- **hidden**

Jika terjadi overflow, konten yang tidak tertampung akan disembunyikan.

- **scroll**

Memunculkan scroll bar pada pinggir elemen sehingga konten yang tidak tertampung akan ditampilkan dengan scroll bar. Jika menggunakan nilai ini, scroll bar akan tetap muncul walaupun konten tidak terjadi overflow.

- **auto**

Sama seperti scroll, hanya jika tidak terjadi overflow, nilai visible yang akan diterapkan.
Berikut adalah contoh penerapan seluruh nilai properti ini.
![contoh](https://assets.cdn.dicoding.com/original/academy/dos:32488b4765fd265f0177016adf2a819020230620200341.jpeg)

### Box-Sizing

Sebelum CSS3, ukuran lebar dan panjang elemen mengacu pada konten elemen (content-box). Itu berarti ukuran elemen seluruhnya merupakan nilai panjang (width) dan lebar (height) yang kita spesifikasikan ditambah dengan nilai padding dan border yang diterapkan pada elemen.

Dengan menggunakan properti box-sizing, kita dapat menentukannya berdasarkan border box, di mana ukuran elemen sudah termasuk content, padding dan border. Dengan metode ini, hasil elemen yang ditampilkan (termasuk padding dan border) akan memiliki dimensi yang sama persis seperti yang kita tentukan.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="content"></div>
    <p>
      Elemen menerapkan <code>box-sizing: content-box;</code> Ukuran box secara keseluruhan akan
      menjadi 260px lebar, 260px tinggi; 260 = 200 + 20 + 20 + 10 + 10
    </p>
    <br />
    <div class="box"></div>
    <p>
      Elemen menerapkan <code>box-sizing: border-box;</code> Ukuran box akan tetap 200px lebar,
      200px tinggi meskipun menerapkan padding dan border
    </p>
  </body>
</html>
```

```
div {
  height: 200px;
  width: 200px;
  background-color: lightgreen;
  border: 10px solid cornflowerblue;
  padding: 20px;
}

.content {
  box-sizing: content-box;
}

.box {
  box-sizing: border-box;
}
```

### Box Model: Border

Border merupakan sebuah garis yang mengelilingi area konten dan padding (opsional). Kita bisa mengatur tipe, ketebalan, serta warna garis yang ditampilkan sesuai dengan yang kita inginkan. Kita juga bisa mengatur dalam menampilkan sebagian atau keseluruhan garis pada elemen. Mari kita eksplorasi properties yang dapat mengatur border.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="box"></div>
  </body>
</html>
```

```
.box {
  border-top-style: solid;
  border-right-style: dotted;
  border-bottom-style: groove;
  border-left-style: double;

  border-width: 4px;
  border-color: red;
  width: 200px;
  height: 50px;
}
```

### Box Model: Padding

Padding merupakan jarak antara area konten dan border. Padding banyak diterapkan pada elemen jika elemen tersebut menerapkan warna latar atau pun border. Padding memberikan sedikit ruang sehingga konten di dalam elemen dapat lebih nyaman untuk ditampilkan.

Berikut adalah contoh implementasi dari padding.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur beatae commodi
      dignissimos eaque fugiat inventore maiores neque nisi sint.
    </p>
    <p class="example">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet assumenda blanditiis cum
      dignissimos enim esse excepturi illum inventore maiores minima, nemo nisi obcaecati officia
      pariatur qui quibusdam sed. Ab, dolorum?
    </p>
  </body>
</html>
```

```
p {
  border: 4px solid #00a2c6;
  width: 350px;
}

p.example {
  padding: 10px;
}
```

### Box Model: Margin

Seperti padding, margin merupakan ruang atau jarak pada sebuah elemen. Namun, jarak tersebut terletak diluar dari konten dan border element. Margin digunakan untuk menjaga elemen agar tidak bertabrakan satu sama lain atau dari tepi jendela browser.

**Sebelum menerapkan padding:**
![padding1](https://assets.cdn.dicoding.com/original/academy/dos:db9f92eced1cd01d2ad30ba59676a7ef20230620201826.jpeg)
**Sesudah pakai padding:**
![padding2](https://assets.cdn.dicoding.com/original/academy/dos:28b2f07315ee457125628ac60fda7f7e20230620201846.jpeg)

### Box Model: Centering Content

Jika kita ingin membuat sebuah kotak berada tepat pada tengah sebuah halaman atau di dalam elemen induknya, margin kanan dan kiri bisa diatur dengan nilai auto. Untuk membuat kotak berada di tengah kita juga harus menentukan lebar dari kotak tersebut (menggunakan properti width). Jika tidak, kotak akan mengambil lebar penuh pada halaman atau induk elemen.

Setelah kita menentukan lebar kotak dan mengatur margin kiri dan kanan menjadi auto, secara otomatis browser akan memberi jarak yang sama di setiap sisi horizontal kotak sehingga membuat kotak berada di tengah halaman.

Berikut contohnya.

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Judul Dokumen</title>

    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="box">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aspernatur
        autem commodi dignissimos dolores ea, eaque, earum esse harum illo in
        incidunt molestias nam non qui recusandae sunt ullam veniam vero!
      </p>
    </div>

    <div class="box center">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi ea,
        id. Aliquid consectetur dolorum exercitationem ipsam, necessitatibus
        nostrum pariatur sunt! Accusantium architecto at dolorem itaque quisquam
        quod soluta sunt voluptatum.
      </p>
    </div>
  </body>
</html>
```

```
.box {
  width: 50%;
  border: 4px solid darkblue;
  padding: 20px;
  margin-bottom: 20px;
}

.box.center {
  margin: 0 auto;
}
```

## Flexbox

### Apa itu Flexbox?

Flexbox (Flexible Box Layout) adalah teknik CSS yang mempermudah pengaturan layout elemen secara fleksibel. Dengan Flexbox, kamu bisa menyusun elemen secara horizontal atau vertikal tanpa perlu repot pakai float atau position.

### Cara Menggunakan Flexbox

Untuk mengaktifkan Flexbox, cukup tambahkan display: flex; pada elemen pembungkus (container).
Contoh:

```
<!DOCTYPE html>
<html>
<head>
    <style>
        .container {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 200px;
            background-color: lightgray;
        }
        .box {
            width: 100px;
            height: 100px;
            background-color: coral;
            text-align: center;
            line-height: 100px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="box">1</div>
        <div class="box">2</div>
        <div class="box">3</div>
    </div>
</body>
</html>
```

### Properti Penting dalam Flexbox

| **_Properti_**  | **_Kegunaan_**                                                          |
| --------------- | ----------------------------------------------------------------------- |
| display: flex;  | Mengaktifkan Flexbox                                                    |
| justify-content | Mengatur posisi elemen secara horizontal                                |
| align-items     | Mengatur posisi elemen secara vertikal                                  |
| flex-direction  | Menentukan susunan elemen (baris/kolom)                                 |
| flex-wrap       | Mengatur apakah elemen tetap dalam satu baris atau pindah ke baris baru |

## CSS Grid

### Apa itu CSS Grid?

CSS Grid adalah teknik layout yang lebih kuat daripada Flexbox karena bisa mengatur baris dan kolom secara bersamaan.

### Cara Menggunakan CSS Grid

Untuk menggunakan Grid, cukup tambahkan display: grid; pada elemen pembungkus, lalu atur jumlah kolom dengan grid-template-columns.
Contoh:

```
<!DOCTYPE html>
<html>
<head>
    <style>
        .container {
            display: grid;
            grid-template-columns: 1fr 1fr 1fr;
            gap: 10px;
            background-color: lightblue;
            padding: 10px;
        }
        .box {
            background-color: coral;
            text-align: center;
            padding: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="box">1</div>
        <div class="box">2</div>
        <div class="box">3</div>
        <div class="box">4</div>
        <div class="box">5</div>
        <div class="box">6</div>
    </div>
</body>
</html>
```

### Properti Penting dalam CSS Grid

| **_Properti_**        | **_Fungsi_**                             |
| --------------------- | ---------------------------------------- |
| display: grid;        | Mengaktifkan Grid                        |
| grid-template-columns | Menentukan jumlah kolom                  |
| grid-template-rows    | Menentukan jumlah baris                  |
| gap                   | Jarak antar elemen                       |
| justify-items         | Mengatur posisi elemen secara horizontal |
| align-items           | Mengatur posisi elemen secara vertikal   |

## Kesimpulan

- CSS adalah bahasa untuk menghias website.
- Ada 3 cara menulis CSS: inline, internal, dan eksternal.
- Flexbox dan Grid dapat mempermudah pengaturan layout halaman.
- Dengan Flexbox dan Grid, elemen bisa lebih rapi, sejajar, dan mudah diatur.
- Box Model sebuah kotak untuk menampung kontennya.

## Kontributor

- Addin Hadi Rizal
- Abraham Willem Hersubagyo
- Bani Rijal Barru Faza
- Mohammed Nasser

## Credits

Tutorial ini dikembangkan oleh Asisten Praktikum Pemrograman Website 2025. Segala tutorial serta instruksi yang dicantumkan pada repositori ini dirancang sedemikian rupa sehingga mahasiswa yang sedang mengambil mata kuliah Pemrograman Website dapat menyelesaikan tutorial saat sesi lab berlangsung.
