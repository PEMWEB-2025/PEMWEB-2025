---
sidebar_label: Latihan Praktikum 2
sidebar_position: 2
Path: docs/latihan/latihan-2
---
import CodeBlock from '@theme/CodeBlock';

# Tujuan

Pada Halaman Profil sebelumnya, kita sudah selesai menstrukturkan ulang konten-konten Kota Bandung dengan elemen-elemen HTML yang sesuai. Kali ini, kita akan beralih ke komponen lain, yaitu styling (CSS).

Kita akan membuat berkas CSS untuk menyediakan styling. Berkas ini akan dikelompokkan dengan folder terpisah. Berikut adalah struktur proyek akhir dari latihan ini.
![folder](https://assets.cdn.dicoding.com/original/academy/dos:1aab5885be8c46e604f62857fe51466a20231130094416.jpeg)

### Alur Latihan
Berikut adalah alur latihan kali ini.

- Membuka hasil latihan terakhir dengan VS Code.
- Membuat folder bernama “styles” untuk menyimpan berkas styling.
- Membuat berkas CSS bernama style.css dalam folder “styles”.

### Latihan Styling untuk Halaman Profil

Silakan ikuti dan simak beberapa langkah berikut untuk mengikuti latihan dengan baik.

1. Silakan buka proyek Halaman Profil terakhir dengan VS Code. 
2. Untuk menerapkan styling, kita akan menerapkannya pada folder terpisah. Silakan buka folder assets.
![folder1](https://assets.cdn.dicoding.com/original/academy/dos:4d17119411454e2719d9d199e3297e7720231130094525.jpeg)
3. Jika kamu sudah mengikuti latihan menampilkan gambar pada HTML, kamu akan menemukan folder image dalam folder assets. Nah, kita tambahkan folder lain dalam folder assets, yaitu folder bernama “styles”.

Silakan buat folder tersebut.
![folder2](https://assets.cdn.dicoding.com/original/academy/dos:690e9d7f37aeb941b1e03a4085dead8f20231130094545.jpeg)
4. Folder baru ini akan kita gunakan untuk menyimpan berkas CSS. Silakan buka folder tersebut dan buat berkas baru dengan nama “style.css”. Untuk membuat berkas styling, tentu kamu perlu menggunakan format **.css**–dibaca: dot css.
![folder3](https://assets.cdn.dicoding.com/original/academy/dos:576c9b57d10b46fc04eb9000c6390fd020231130094603.jpeg)
5. Sip! Folder styles dan berkas style.css sudah siap untuk dimanfaatkan. Kita akan menggunakan berkas ini untuk proses styling halaman ke depannya.

## Latihan: Menulis Rules pada Berkas CSS

### Alur Latihan

Berikut adalah alur latihan kali ini.

- Membuka hasil latihan terakhir dengan VS Code.
- Menulis kode styling pada berkas CSS yang telah dibuat dalam latihan sebelumnya.
- Mengubah penerapan styling pada selector h2 dan h3 agar menggunakan group selector.

### Latihan Menulis Rules pada Berkas CSS

1. Silakan buka proyek Halaman Profil terakhir dengan VS Code.
2. Untuk latihan awal, kita akan menuliskan rule styling pada beberapa elemen HTML yang tersedia dalam Halaman Profil. Kita akan mengubah tipe font pada halaman ini.

Tetapkanlah tipe font ‘sans-serif’ sebagai font yang digunakan pada seluruh elemen dalam elemen `<body>`. Silakan buka berkas styles.css dan tuliskan kode berikut padanya.

<CodeBlock className="no-copy">
{`
body {
  font-family: sans-serif;
}
`}
</CodeBlock>

3. Untuk styling kedua, kita tetapkan juga warna pada setiap elemen `<h2>` dan `<h3>` dengan menuliskan kode sebagai berikut.
<CodeBlock className="no-copy">
{`
body {
  font-family: sans-serif;
}
 
h2 {
  color: #00a2c6;
}
 
h3 {
  color: #00a2c6;
}
`}
</CodeBlock>

4. Styling yang terakhir adalah memberikan warna background, warna teks, dan padding pada elemen `<footer>`. Silakan tambahkan kode berikut dalam style.css.
<CodeBlock className="no-copy">
{`
footer {
  padding: 20px;
  color: white;
  background-color: #00a2c6;
}
`}
</CodeBlock>

5. Jadi, keseluruhan kode pada berkas style.css akan tampak seperti berikut.
<CodeBlock className="no-copy">
{`
body {
  font-family: sans-serif;
}
 
h2 {
  color: #00a2c6;
}
 
h3 {
  color: #00A2C6;
}
 
footer {
  padding: 20px;
  color: white;
  background-color: #00a2c6;
}
`}
</CodeBlock>

6. Terakhir, apakah Anda melihat ada kesamaan styling dalam dua selector berdasarkan kode di atas? Benar, ada styling yang sama. Nah, dalam rangka meringkaskan kode, kita akan menggabungkannya dengan teknik yang bernama group selector.

Wah, apa itu group selector? Tenang, kita akan membahas teknik ini pada materi berikutnya. Tentunya masih dalam modul yang sama. So, silakan sesuaikan seluruh isi kodenya hingga menjadi seperti berikut.

<CodeBlock className="no-copy">
{`
body {
  font-family: sans-serif;
}
 
h2, h3 {
  color: #00a2c6;
}
 
footer {
  padding: 20px;
  color: white;
  background-color: #00a2c6;
}
`}
</CodeBlock>