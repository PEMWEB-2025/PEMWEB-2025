---
sidebar_label: "Pertemuan 4: Pengenalan Javascript dan DOM"
sidebar_position: 4
Path: docs/materi/pertemuan-4
---

# Pertemuan 4: Pengenalan Javascript dan DOM

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Apa Itu Javascript
Javascript adalah bahasa pemrograman yang digunakan untuk membuat website menjadi lebih interaktif. Misalnya: tombol yang bisa diklik, gambar yang bisa berganti ketika diinteraksi, atau form yang merespon ketika kita mengetik.

## Cara Mengimplementasikan Javascript
### 1. Langsung di File HTML Dengan Menggunakan Tag `<script>`
```
<html>
<head>
  <title>Belajar Javascript</title>
</head>
<body>
  <h1>Hello World</h1>

  <script>
    alert("Halo, ini modal popup dari Javascript");
  </script>
</body>
</html>
```

### 2. Di File Terpisah
File `script.js`:
```
const text = "Halo, ini modal popup dari Javascript";
alert(text);
```

File `index.html`:
```
<html>
<head>
  <title>Belajar Javascript</title>
</head>
<body>
  <h1>Hello World</h1>

  <script src="script.js"></script>
</body>
</html>
```

## Variabel & Tipe Data
### Variabel
#### `var` dan `let`
Sifatnya mutable atau dapat diubah isinya. Contoh:
```
let angka1 = 5;
const angka2 = 2;

angka1 += angka2;

console.log(angka1);

// Output = 7
```

#### `const`
Sifatnya immutable atau tidak dapat diubah isinya. Contoh:
```
let angka1 = 5;
const angka2 = 2;

angka2 += angka1;

console.log(angka1);

// Output = Error
```

Walaupun bersifat immutable, `const` dapat digunakan pada array atau object. Contoh:
```
const buah = ['apel', 'jeruk']
buah.push('mangga')
console.log(buah)         // Output ['apel', 'jeruk', 'mangga']

buah = ['pisang']         
console.log(buah)         // Error
```

### Tipe Data
Tipe data pada Javascript:
- String
```
let text = "Halo";
```
- Number
```
let angka1 = 3;
const angka2 = 4.21;
```
- Boolean
```
let isAngka = true;
```
- Undefined
```
let result;
```
- Null
```
let result = null;
```

## Operator & Percabangan
### Operator
#### Operator Aritmatika
```
let a = 1;
let b = 2;
let hasil = a + b;
```

#### Operator Perbandingan
```
5 == '5'    // true (nilai sama)
5 === '5'   // false (tipe data beda)
```

#### Operator Logika
```
true && false   // false
true || false   // true
!true           // false
```

### Percabangan
```
let nilai = 80;
const kkm = 75;

if (nilai >= kkm) {
  console.log('Anda lulus');
} else {
  console.log('Maaf, tidak lulus');
}
```