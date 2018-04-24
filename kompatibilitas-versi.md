# Kompatibilitas Versi

Buku ini mendeskripsikan Swif 4.0.3, versi default dari Swift yang termasuk di dalam Xcode 9.2. Kamu bisa menggunakan Xcode 9.2 untuk membangun target yang ditulis dengan Swift 4 atau Swift 3.

> Catatan
>
> Saat kompiler Swift 4 bekerja dengan Swift 3, dia akan mengidentifikasi versi bahasa sebagai 3.2. Hasilnya, kamu dapat menggunakan pengkondisian blok kompilasi seperti `#if swift(>=3.2)` untuk menulis kode yang kompatibel dengan banyak kompiler Swift.

Saat kamu menggunakan Xcode 9.2 untuk mengembangkan kode Swift 3, fungsi-fungsi baru dari Swift 4 kebanyakan sudah tersedia. Dengan demikian, fitur-fitur berikut ini hanya tersedia untuk kode Swift 4:

* Operasi-operasi substring menghasilkan sebuah instance dari tipe `Substring`, alih-alih `String`.
* Atribut`@objc` secara implisit ditambahkan di lebih sedikit tempat.
* Ekstensi untuk tipe pada file yang sama dapat mengakses anggota privat dari tipe tersebut.

Target yang ditulis menggunakan Swift 4 dapat bergantung pada target yang ditulis menggunakan Swift 3, dan sebaliknya. Ini berarti, jika kamu mempunyai proyek yang besar yang dibagi dalam banyak framework, kamu dapat memigrasi kode kamu dari Swift 3 ke Swift 4 satu per satu.

