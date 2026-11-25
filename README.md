Jawaban Pertanyaan Tugas Poin 6 Minggu 2

1. Apa yang muncul di address bar setelah form dikirim, dan mengapa data form tampil di sana? Hubungkan dengan materi method HTTP di Minggu 1.
   - Setelah tombol kirim ditekan, address bar akan menampilkan URL tujuan, yaitu pesan.html yang diikuti oleh tanda tanya ?
     dan rangkaian parameter data formulir yang sudah dimasukan oleh pengguna sesuai dengan parameter name yang ada di html,
     contohnya: pesan.html?nama=Yusuf&whatsapp=08123&.... Hal ini terjadi karena kita menggunakan atribut method="get".
     Berdasarkan materi protokol HTTP, metode GET mengirimkan data ke browser dengan melampirkannya langsung pada bagian URL,
     sehingga data terlihat di address bar.

2. Pilih satu bagian halamanmu yang memakai element semantic. Kenapa kamu memilih element itu dan bukan `<div>`?
   - Saya memilih menggunakan element `<nav>` di dalam `<header>` untuk menampung tautan navigasi antarhalaman.
     Alasannya karena `<nav>` memiliki makna semantik yang jelas dan biasa digunakan untuk mendefinisikan blok navigasi utama situs web.
     Berbeda dengan `<div>` yang sifatnya lebih generik, penggunaan `<nav>` membantu mesin pencari dan
     screen reader untuk mengenali bagian tersebut sebagai menu navigasi web kita.

Jawaban Pertanyaan Tugas Poin 8 Minggu 3

https://ysfafaf2.github.io/kedai_kopi/

1. Sebutkan satu bagian yang kamu susun dengan Flexbox dan satu bagian dengan Grid. Mengapa pilihan itu cocok untuk kedua bagian tersebut?
   - Bagian yang disusun dengan Flexbox adalah area header/navigasi .header-inner dan .nav-list, karena
     elemen-elemennya berada dalam satu arah yang sama yaitu secara horizontal. Flebox disini digunakan untuk menyusun nama kedai
     dan daftar tautan navigasi, baik vertikal di layar kecil maupun horizontal sejajar di layar yang lebar. Selain itu, digunakan
     juga untuk mudah mengatur tata letaknya menggunakan justify-content, align-items, dan gap.
   - Bagian yang disusun dengan Grid adalah daftar kartu menu .menu-grid, karena tata letaknya bersifat dua dimensi, yaitu ada
     baris dan kolom dan perlu berubah dari 1 kolom di ponsel menjadi 2 kolom di lebar 600px dan 3 kolom di lebar 960px secara presisi.

2. Ceritakan satu aturan CSS yang awalnya tidak berlaku. Apa yang kamu lihat di panel Styles, dan bagaimana kamu memperbaikinya?
   - Awalnya aturan lebar kartu/input melebar melebihi kontainer karena padding dan border menambah ukuran total elemen. Di panel
     Styles pada DevTools, terlihat nilai box-sizing masih bawaan, yaitu content-box atau ada aturan yang tertimpa. Hal itu saya
     perbaiki dengan menambahkan box-sizing: border-box; secara global pada *, *::before, \*::after agar padding dan border dihitung
     di dalam lebar elemen.
