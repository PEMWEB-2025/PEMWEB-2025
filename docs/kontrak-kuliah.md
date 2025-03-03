---
sidebar_label: Kontrak Kuliah Praktikum
sidebar_position: 2
Path: docs/kontrak-kuliah
---

# Kontrak Kuliah: Praktikum Pemrograman Website

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Tujuan Pembelajaran

Setelah menyelesaikan tutorial ini, mahasiswa diharapkan untuk dapat:

- Mengetahui cara instalasi IDE dan extension untuk keperluan praktikum
- Mengetahui materi apa saja yang akan dipelajari selama praktikum pemweb
- Mengetahui aplikasi buat dapat akses web server

## Tutorial: Instalasi IDE

IDE (*Integrated Development Environment*) adalah perangkat lunak yang membantu para pengembang dalam menulis, mengedit, dan mengelola kode. Berikut adalah langkah-langkah untuk memasang IDE.

### Langkah 1: Pemilihan *Text Editor* atau IDE

Pilihlah *text editor* atau IDE yang sesuai dengan preferensimu. Beberapa pilihan populer yang dapat kamu pertimbangkan meliputi:

- [Vim](http://www.vim.org/download.php)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Sublime Text](https://www.sublimetext.com/)
- [PyCharm](https://www.jetbrains.com/pycharm/)

### Langkah 2: Proses Instalasi

1. Pergi ke situs web resmi IDE yang kamu pilih.
2. Ikuti petunjuk yang diberikan untuk mengunduh *installer* IDE.
3. Jalankan *installer* dan ikuti instruksi di layar untuk menyelesaikan proses instalasi.

### Langkah 3: Memulai Menggunakan IDE

1. Setelah proses instalasi selesai, buka IDE yang telah terinstal.
2. Eksplorasi antarmuka dan fitur yang disediakan oleh IDE untuk membantumu dalam pengembangan proyek.

**Catatan:**

- Pastikan kamu memilih IDE yang sesuai dengan jenis proyek yang akan dikerjakan.
- Jangan ragu untuk mengeksplorasi fitur-fitur IDE (contoh: *extensions* atau *plugin*) dan memanfaatkan sumber daya pendukung, seperti dokumentasi dan tutorial, untuk meningkatkan produktivitas dalam pengembangan perangkat lunak.

## Extension Yang Diperlukan

Sementara temen" mungkin butuh extension ini dan mungkin beberapa dari kalian sudah ada yang punya:
1. Code Runner, Extension ID -> **`formulahendry.code-runner`**
2. Live Server, Extension ID -> **`ritwickdey.LiveServer`**
3. HTML CSS Support, Extension ID -> **`ecmel.vscode-html-css`**
4. Auto Rename Tag, Extension ID -> **`formulahendry.auto-rename-tag`**

## Rencana Materi Pembelajaran
Berikut tabel Rencana Materi Pembelajaran : 

| **_Pertemuan_**    | **_Materi_**  |
|--------------------|---------------|
| **Pertemuan - 1**  | Kontrak Praktikum dan Instalasi Web Server |
| **Pertemuan - 2**  | HTML dan CSS |
| **Pertemuan - 3**  | Javascript |
| **Pertemuan - 4**  | JQuery |
| **Pertemuan - 5**  | Ajax |
| **Pertemuan - 6**  | PHP Native |
| **Pertemuan - 7**  | OOP (Object Oriented Programming) |
| **Pertemuan - 8**  | Form Validation |
| **Pertemuan - 9**  | Session & Cookie |
| **Pertemuan - 10** | Laravel 1 (MVC Routes) |
| **Pertemuan - 11** | Laravel 2 (Migration Seeder Factory) |
| **Pertemuan - 12** | Laravel 3 (Authentication) |
| **Pertemuan - 13** | Laravel 4 (Create, Read, Update, Delete) |
| **Pertemuan - 14** | Checking Tugas Besar dan Pengumpulan Akhir Tugas |

## Instalasi Web Server

### Langkah 1: Pemilihan App buat akses web server

Pilihlah *Aplikasi* yang sesuai dengan preferensimu:

**`Windows`** : 
1. [Laragon](https://laragon.org)
2. [Herd For Windows](https://herd.laravel.com/windows) 

**`MacOS`** : 
1. [Herd For MacOS](https://herd.laravel.com)

### Langkah 2: Install untuk Windows

### [Laragon](https://laragon.org):

**Step 1: Download Laragon**

![download](/img/1/download.png)

Langkah pertama adalah mengunduh installer Laragon dari situs web resmi. Buka (https://laragon.org/download/) dan pilih versi Laragon yang ingin teman" unduh kalau bisa pilih yang versi terbaru.

**Step 2: Run the Installer**

![install](https://miro.medium.com/v2/resize:fit:1018/format:webp/1*RN2MmAeEUjaMH3eWQ4mQZw.png)

Setelah unduhan selesai, jalankan penginstal dengan mengklik dua kali pada berkas yang diunduh. Penginstal akan memandu teman" melalui proses instalasi. Klik tombol "Next" untuk melanjutkan ke layar pemilihan bahasa.

**Step 3: Choose Installation Location**

![location](https://miro.medium.com/v2/resize:fit:1000/format:webp/1*eE4_s_9nY3QQpy4hpNHodw.png)

Pada langkah ini, Temen" perlu memilih lokasi tempat untuk menginstal Laragon. Kamu dapat memilih lokasi default atau memilih lokasi lain dengan mengklik tombol “Browse”.

**Step 4: Select Components**

![components](https://miro.medium.com/v2/resize:fit:992/format:webp/1*iCNwZZumHPaMqXfx5FVHIg.png)

Pada langkah ini, kamu dapat memilih komponen dan pengaturan yang ingin kamu instal dengan Laragon. Komponen default meliputi Apache, MySQL, dan PHP. Pilih juga opsi seperti auto start, pretty url (myapp.test) dan editor teks default.

**Step 5: Review the sections**

![review](https://miro.medium.com/v2/resize:fit:994/format:webp/1*klZyGyxr3KDOw5rmTADmsw.png)
![install](https://miro.medium.com/v2/resize:fit:996/format:webp/1*3wfrPonRRm0ha9oCxxS41Q.png)

Setelah kamu menyelesaikan semua langkah, layar akan menampilkan semua pilihan sebelumnya dan klik tombol **"Instal"** untuk memulai proses instalasi. Laragon sekarang akan terinstal di komputermu.

**Step 6: Launch Laragon**

![launch](https://miro.medium.com/v2/resize:fit:1350/format:webp/1*3wronPRrNtEefMOwVUvwIA.png)

Setelah instalasi selesai, klik tombol “Finish” untuk meluncurkan Laragon. Kini kamu dapat mulai menggunakan Laragon untuk mengembangkan aplikasi PHP mu. Klik tombol start all untuk memulai layanan seperti apache, nginx, redis, memcache, dan lainnya.

**Step 8: Make sure you enable ports**

![ports](https://miro.medium.com/v2/resize:fit:1066/format:webp/1*yRlQh1mfbpJE0yj0QnwDrA.png)

Klik ikon pengaturan ⚙️ dan pilih tab Layanan & Port, lalu aktifkan opsi dan port yang diperlukan. Untuk SSL, pastikan mengaktifkan port SSL 443 untuk Apache dan Nginx. Kalian bebas mau pakai web server apa aja mau itu Apache atau Nginx.

**Mengganti versi PHP atau NodeJS**

Kalian bisa download versi **ZIP** pada tiap" website resminya.

[PHP](https://www.php.net/downloads.php)
[NdeJS](https://nodejs.org/en/download)

Setelah mendownload versi zip nya masuk ke folder laragon kalian lalu copy paste file zip nya tadi dan taruh di folder php atau nodejs lalu extract file. Jika sudah file *ZIP* nya bisa dihapus. 

**`/laragon/bin/php/`**

**`/laragon/bin/nodejs/`**

### [Herd For Windows](https://herd.laravel.com/windows):

**Step 1: Install Laravel Herd for Windows**

Sekarang kita akses situr resmi (https://herd.laravel.com/windows). Pada halaman web Laravel Herd Kita bisa lihat button *Download for Windows*. Untuk memulai proses download Laravel Herd installer, tekan button tersebut. Kita tunggu sampai proses download selesai. Setelah selesai kita bisa lihat ada file Herd-1.11.1-setup.exe (Versi laravel herd installer pada saat panduan ini ditulis).

**Step 2: Run Laravel Herd Installer**

Setelah laravel herd installer selesai kita download, kita run installler dengan cara run as adminstrator, lalu ikuti langkah-langkahnya sampai proses install selesai.

![run](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*dsZxEb_q66QjqdE5GAHC5w.png)

Catatan: Laravel herd perlu permission sebagai admin supaya installer dapat menambahkan HerdHelper service yang bertanggung jawab untuk memperbaharui file *hosts*, map direktori dan link project ke domain *.test*.

**Step3: Run Laravel Herd**

![lets](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/1%20tampilan%20awal%20setelah%20install.png)

Setelah proses instalasi selesai, selanjutnya kita bisa run langsung laravel herd yang sudah kita install. Ketika pertama kali laravel herd kita run, kita akan membuka windows untuk setup awal. Untuk melanjutkan, kita tekan button *Let's get started* untuk memulai proses setup awal laravel herd.

Selanjutnya laravel herd akan mendownload php, node js dan tools lainnya.

![php](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/2%20install%20php%208.3.png)

Setelah proses download selesai, selanjutnya akan masuk ke windows untuk aktivasi laraverd herd pro. Kita bisa tekan link *Skip for now* untuk menyelesaikan proses setup laravel herd.

![skip](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/3.%20aktivasi%20laravel%20herd%20pro.png)

Selanjutnya kita bisa lihat windows setup completed. Kita bisa pilih tekan button Open Dashboard untuk membuka dashboard Laravel herd.

[open](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/4%20tampilan%20setup%20laravel%20herd%20selesai.png)

Kita bisa lihat tampilan dashboard laravel herd. Pada dashboard kita bisa lihat informasi seperti service yang aktif, menu untuk laravel herd pro, dan quick access dengan button ke halaman untuk mengelola project kita.

[dashboard](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/5%20tampilan%20dashboard%20laravel%20herd.png)

**Step 4: Cek versi php, laravel, composer dan nodejs**

Selanjutnya kita akan coba cek php, laravel, composer dan nodejs yang terinstall dengan run command berikut ini di command prompt windows atau Cmder.

```
php --version
laravel --version
composer --version
node --version
```

Ketika command di atas kita run akan tampil output berikut ini.

```
C:\Users\[nama user]>php --version
PHP 8.3.12 (cli) (built: Sep 24 2024 20:22:14) (NTS Visual C++ 2019 x64)
Copyright (c) The PHP Group
Zend Engine v4.3.12, Copyright (c) Zend Technologies
    with Zend OPcache v8.3.12, Copyright (c), by Zend Technologies

C:\Users\[nama user]>laravel --version
Laravel Installer 5.8.5

C:\Users\[nama user]>composer --version
Composer version 2.7.7 2024-06-10 22:11:12
PHP version 8.3.12 (C:\Users\InformatikaUMMI\.config\herd\bin\php83\php.exe)
Run the "diagnose" command to get more detailed diagnostics output.

C:\Users\[nama user]>node --version
v23.0.0
```

### [Herd For MacOS](https://herd.laravel.com):

**Step 1: Download the Aplicacion Herd for MacOS**

![mac](https://i.postimg.cc/G2Hftx1v/image.png)

Kalau untuk ini langsung aja ke websitenya langsung klik Download fow macos (https://herd.laravel.com) 

**Step 2: Buka aplikasi Herd nya**

Buka aplikasi Herd nya untuk mastiin kalau bener" sudah bisa jalan.

**Step 3: Cek Environment di Terminal**

Setelah proses pemasangan selesai, Kamu memiliki lingkungan pengembangan PHP dan Laravel yang berfungsi penuh. Ini berarti kamu dapat memiliki PHP, Laravel, dan komposer dari terminal Anda:

```
herd --version
php --version
laravel --version
composer --version
node --version
```

## Akhir Kata

Selamat, ya! Kamu sudah menyelesaikan tutorial tentang instalasi IDE dan instalasi Web Server dan memahami rencana pembelajaran untuk praktikum *PEMWEB* semester ini 🔥.

Ke depannya, kalau sedang mengerjakan tugas, jangan grogi sama banyaknya materi, ya. Santai saja, ini bukan lomba *sprint* kok; pelan-pelan saja, pasti bisa. Kode-kode itu tidak harus langsung masuk ke otak, tapi yang penting dimengerti, kan? Jadi, **jangan sampai asal *copy-paste* tanpa mengerti** ya, nanti jadi bingung sendiri. Kalau memang buntu, jangan malu untuk bertanya ke teman atau asisten dosen. Asisten dosen sudah pasti siap bantuin 🥹🫶🏻, kok. Jadi, semangat terus dan nikmati prosesnya. *Good luck!*

## Referensi Tambahan

- [About pull request merges](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/about-pull-request-merges)
- [Resolving a merge conflict on GitHub](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/resolving-a-merge-conflict-on-github)

## Kontributor

- Addin Hadi Rizal
- Abraham Willem Hersubagyo

## Credits

Tutorial ini dikembangkan oleh Asisten Praktikum Pemrograman Website 2025. Segala tutorial serta instruksi yang dicantumkan pada repositori ini dirancang sedemikian rupa sehingga mahasiswa yang sedang mengambil mata kuliah Pemrograman Website dapat menyelesaikan tutorial saat sesi lab berlangsung.

[GitHub]: https://github.com/