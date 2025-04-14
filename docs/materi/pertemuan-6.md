---
sidebar_label: "Pertemuan 6: AJAX"
sidebar_position: 5
Path: docs/materi/pertemuan-6
---

# Pertemuan 5: AJAX

Pemrograman Website — diselenggarakan oleh Fakultas Teknologi Informasi dan Sains Data Universitas Sebelas Maret, Semester Genap 2024/2025

---

## Apa itu AJAX?

AJAX (Asynchronous JavaScript and XML) adalah suatu cara/teknik untuk mengirim dan menerima data dari server tanpa merefresh halaman web. AJAX bisa digunakan pada halaman web untuk mengambil(fetch) data di background dan meng-update bagian dari halaman secara dinamis.

### Kenapa Menggunakan AJAX?

- Untuk memperbarui bagian dari halaman web tanpa me-refresh seluruh halaman.
- Untuk mengambil data dari server dan menampilkannya secara dinamis.
- Untuk mengirim data ke server tanpa mereload halaman.

### Konsep Dasar AJAX

- Asynchronous: browser tidak menunggu sampai request selesai — halaman tetap interaktif.
- HTTP Request: AJAX bekerja dengan mengirim request HTTP seperti GET atau POST ke server.
- JavaScript & JSON: Umumnya, data yang direturn oleh server berformat JSON.

### Bagaimana AJAX Bekerja?

Biasanya alur kerja AJAX seperti berikut:

- User melakukan sesuatu (misalnya: klik tombol).
- Request AJAX dikirim ke server.
- Server memproses request dan mereturn data.
- Response AJAX ditangani oleh JavaScript (misalnya: menampilkan data ke halaman).

## Teknik Modern AJAX

fetch() adalah API JavaScript modern untuk membuat request AJAX. fetch() lebih sederhana karena menggunakan Promises, yang memudahkan penanganan asynchronous operation.

Contoh Dasar Menggunakan Fetch:

```javascript
fetch("https://jsonplaceholder.typicode.com/posts") // Mengambil data dari API
  .then((response) => response.json()) // Mengonversi respons menjadi format JSON
  .then((data) => console.log(data)) // Mengolah data
  .catch((error) => console.error("Error:", error)); // Menangani error
```

- response.json(): Mengonversi response menjadi format JSON (digunakan saat respons API berupa JSON).

- response.text(): Digunakan untuk file teks biasa.

- .then() : Digunakan untuk merangkai promise ketika menangani data setelah permintaan selesai.

## Fetch Local File (XML atau Teks)

Untuk mengambil/fetch file lokal (seperti XML, file teks, dll.), perlu menjalankan kode di server lokal (misalnya menggunakan Node.js, Python, atau Live Server di VS Code). Browser tidak mengizinkan pembacaan file lokal langsung karena alasan keamanan.

Contoh Mengambil Local File Fetch:

```javascript
fetch("example.txt") // Path ke file teks lokal
  .then((response) => response.text()) // Membaca respons sebagai teks
  .then((text) => console.log(text)) // Menampilkan konten
  .catch((error) => console.error("Error:", error)); //Error Handling
```

3. Mengirim Permintaan POST dengan fetch()

Anda bisa mengirim permintaan POST untuk mengirimkan data (seperti JSON, data form) ke server.
Contoh Mengirim Data JSON dengan fetch():

```javascript
const data = {
  username: "Addin",
  email: "Addin@sidoarjo.com",
};

fetch("https://example.com/submit", {
  method: "POST",
  headers: {
    "Content-Type": "application/json", // Memberitahu server bahwa data dalam format JSON
  },
  body: JSON.stringify(data), // Mengonversi objek JavaScript menjadi JSON
})
  .then((response) => response.json())
  .then((data) => console.log("Success:", data))
  .catch((error) => console.error("Error:", error));
```

## AJAX dan jQuery

### Menggunakan GET

Dengan menggunakan jQuery, akan sangat mudah dan ringkas ketika melakukan request AJAX GET.

```javascript
  <button id="getData">Ambil Data</button>

  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <script>
    $('#getData').on('click', function() {
      $.ajax({
        url: 'https://jsonplaceholder.typicode.com/posts',
        method: 'GET',
        success: function(data) {
          console.log('Data berhasil diambil:', data);
        },
        error: function(error) {
          console.error('Terjadi kesalahan:', error);
        }
      });
    });
  </script>
```

- $.ajax(): Mengirim request GET dengan contoh url jsonplaceholder.

### Menggunakan POST

```javascript
<button id="sendData">Send Data</button>

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
  $('#sendData').on('click', function() {
    var jsonData = {
      username: 'addin',
      email: 'addin@sidoarjo.com'
    };

    $.ajax({
      url: 'https://example.com/submit',    // URL server
      type: 'POST',                         // Metode POST
      contentType: 'application/json',      // Mengirim data dalam format JSON
      data: JSON.stringify(jsonData),       // Mengonversi data menjadi string JSON
      success: function(response) {
        console.log('Success:', response);  // Menangani response berhasil
      },
      error: function(error) {
        console.error('Error:', error);     // Menangani error
      }
    });
  });
</script>
```

- contentType: 'application/json': Memberitahu server bahwa data yang dikirim adalah JSON.
- JSON.stringify(jsonData): Mengonversi objek JavaScript menjadi string JSON.

### Menggunakan Form

jQuery mempermudah penggunaan AJAX, terutama ketika Anda perlu menangani masalah kompatibilitas antar-browser. Berikut adalah cara mengirim permintaan POST dan data form menggunakan jQuery.
Mengirim Data Form Menggunakan POST (Tanpa JSON):

```javascript
<form id="FormSederhana">
  <input type="text" id="username" name="username" placeholder="Username">
  <input type="email" id="email" name="email" placeholder="Email">
  <button type="submit">Submit</button>
</form>

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script>
  $('#FormSederhana').on('submit', function(event) {
    event.preventDefault();                 // agar ketika form disubmit tidak refresh

    var formData = $(this).serialize();     // parsing data form

    $.ajax({
      url: 'https://example.com/submit',    // URL server
      type: 'POST',                         // Metode POST
      data: formData,                       // Mengirim data form yang telah diparsing
      success: function(response) {
        console.log('Success:', response);  // Menangani response berhasil
      },
      error: function(error) {
        console.error('Error:', error);     // Menangani error
      }
    });
  });
</script>
```

- $(this).serialize(): Parsing data form menjadi string key=value (contoh username=addin&email=addin@sidoarjo.com).
- $.ajax(): Mengirim request POST dengan data dari form.

## Contoh Program Sederhana

Cobalah jalankan HTML sederhana ini untuk mencoba AJAX dan Jquery

```html
  <!DOCTYPE html>
  <html lang="id">
    <head>
      <meta charset="UTF-8" />
      <title>AJAX Demo</title>
      <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
      <style>
        .card {
          border: 1px solid #ccc;
          border-radius: 8px;
          padding: 16px;
          margin: 10px 0;
          background-color: #f9f9f9;
          box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
          max-width: 200px;
          height: 100%;
          overflow: scroll;
        }

        button {
          width: 100%;
          height: 100px;
          font-size: larger;
          font-weight: 400;
        }

        #postsContainer {
          display: flex;
          justify-content: center;
          align-items: center;
          gap: 10px;
          height: 350px;
          margin-top: 50px;
        }
      </style>
    </head>
    <body>
      <button id="loadPosts">Ambil Data</button>
      <div id="postsContainer"></div>

      <script>
        function shuffleArray(array) {
          return array.sort(() => Math.random() - 0.5);
        }

        $("#loadPosts").on("click", function () {
          $.ajax({
            url: "https://jsonplaceholder.typicode.com/posts",
            method: "GET",
            dataType: "json",
            success: function (data) {
              $("#postsContainer").empty();

              const shuffled = shuffleArray(data);
              const randomFive = shuffled.slice(0, 5);

              randomFive.forEach(function (post) {
                const card = `
                <div class="card">
                  <h3>${post.title}</h3>
                  <p>${post.body}</p>
                </div>
              `;
                $("#postsContainer").append(card);
              });
            },
            error: function () {
              $("#postsContainer").html("<p>Gagal mengambil data.</p>");
            },
          });
        });
      </script>
    </body>
  </html>

```

## Kontributor

- Addin Hadi Rizal
- Abraham Willem Hersubagyo
- Bani Rijal Barru Faza
- Mohammed Nasser

## Credits

Tutorial ini dikembangkan oleh Asisten Praktikum Pemrograman Website 2025. Segala tutorial serta instruksi yang dicantumkan pada repositori ini dirancang sedemikian rupa sehingga mahasiswa yang sedang mengambil mata kuliah Pemrograman Website dapat menyelesaikan tutorial saat sesi lab berlangsung.
