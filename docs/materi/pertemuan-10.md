---
sidebar_label: "Pertemuan 10: Laravel 1 (MVC) Routes"
sidebar_position: 10
Path: docs/materi/pertemuan-10
---

# Pertemuan 10: Laravel 1 (MVC) Routes

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Pengenalan Laravel
- Laravel adalah framework di PHP untuk membuat Web atau API
- Laravel pertama kali dibuat oleh Taylor Otwell tahun 2011
- Laravel adalah framework yang open source dan gratis, sehingga kita bisa menggunakannya tanpa biaya dan juga bisa berkontribusi ke projectnya 

## Kenapa Laravel
- Saat ini Laravel adalah framework paling populer di PHP
- Banyak perusahaan yang sudah menggunakan Laravel sebagai framework pilihan ketika menggunakan PHP
- Laravel juga memiliki ekosistem yang sangat besar, terutama dari ekosistem teknologi pendukung, sehingga ketika menggunakan Laravel, kita bisa mengintegrasikan dengan teknologi pendukung nya dengan lebih mudah

## Instalasi Laravel

### [Herd For Windows](https://herd.laravel.com/windows):

**Step 1: Install Laravel Herd for Windows**

Sekarang kita akses situr resmi (https://herd.laravel.com/windows). Pada halaman web Laravel Herd Kita bisa lihat button _Download for Windows_. Untuk memulai proses download Laravel Herd installer, tekan button tersebut. Kita tunggu sampai proses download selesai. Setelah selesai kita bisa lihat ada file Herd-1.11.1-setup.exe (Versi laravel herd installer pada saat panduan ini ditulis).

**Step 2: Run Laravel Herd Installer**

Setelah laravel herd installer selesai kita download, kita run installler dengan cara run as adminstrator, lalu ikuti langkah-langkahnya sampai proses install selesai.

![run](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*dsZxEb_q66QjqdE5GAHC5w.png)

Catatan: Laravel herd perlu permission sebagai admin supaya installer dapat menambahkan HerdHelper service yang bertanggung jawab untuk memperbaharui file _hosts_, map direktori dan link project ke domain _.test_.

**Step3: Run Laravel Herd**

![lets](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/1%20tampilan%20awal%20setelah%20install.png)

Setelah proses instalasi selesai, selanjutnya kita bisa run langsung laravel herd yang sudah kita install. Ketika pertama kali laravel herd kita run, kita akan membuka windows untuk setup awal. Untuk melanjutkan, kita tekan button _Let's get started_ untuk memulai proses setup awal laravel herd.

Selanjutnya laravel herd akan mendownload php, node js dan tools lainnya.

![php](https://cdn.jsdelivr.net/gh/gungunpriatna/tes-repositori@master/how-to/install-tools/laravel-herd/2%20install%20php%208.3.png)

Setelah proses download selesai, selanjutnya akan masuk ke windows untuk aktivasi laraverd herd pro. Kita bisa tekan link _Skip for now_ untuk menyelesaikan proses setup laravel herd.

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

### [MAMP For MacOS](https://www.mamp.info/en/mac/)
### [MAMP For Windows](https://www.mamp.info/en/mamp/windows/)
### [Download Composser](https://getcomposer.org)

### Step" Kalau Pakai MAMP
- Step 1 Download MAMP
- Step 2 Download Composser
- Step 3 Instal [Laravel Installer] via Composser
```
composer global require laravel/installer
```
- Step 4 


