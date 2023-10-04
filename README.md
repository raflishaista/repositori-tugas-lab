 Jelaskan manfaat dari setiap element selector dan kapan waktu yang tepat untuk menggunakannya.
 Element selector bermanfaat ketika ada ketika suatu tag yang sama digunakan berkali-kali di suatu file html. Dengan element selector, tag tersebut dapat diberi atribut dimana semua elemen yang menggunakan tag tersebut akan mendapatkan atribut semuanya, jika memiliki tag yang sama atau id yang sama. Hal ini akan mengurangi repetisi dan pencarian dari tag atau id yang digunakan.
 
 Jelaskan HTML5 Tag yang kamu ketahui.
 <a> anchor untuk penggunaan hyperlink, <body> untuk mengelola isi atau body dari file, <button> menspesifikasi dan untuk pengelolaan tombol, <br> untuk adanya suatu lompatan pemisah, <th> table header sebagai ehad pada table, <td> table data untuk mengelola isi dari tabel, <th> untuk mengelola baris dari table.
 
 Jelaskan perbedaan antara margin dan padding.
 Margin adalah ruang yang berada di luar suatu elemen, yang menjaga jarak dengan margin dari elemen lain. Sedangkan, padding adalah ruang dan posisi antara isi dari elemen dan elemen itu sendiri, sehingga menenetukan bagaimana elemen terlihat dan mempoisikan dirinya didalam container atau "bungkus" seperti halaman.
 
 Jelaskan perbedaan antara framework CSS Tailwind dan Bootstrap. Kapan sebaiknya kita menggunakan Bootstrap daripada Tailwind, dan sebaliknya?
 Perbedaannya bisa dilihat di cara kerja dan pembangunan, seperti Tailwind yang menggabungkan kelas-kelas utilitas yang telah didefinisikan sebelumnya sedangkan Bootstrap yang menggunakan gaya dan komponen yang telah didefinisikan yang sudah ada sebelumnya. Tailwind lebih baik digunakan bagi individu yang sudah mempunyai pengalaman dalam utilitas tersebut, dan Boostrap untuk pemula yang dapat membangun sebuah halaman dengan cepat.
 
 Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

 Kustomisasi desain pada templat HTML yang telah dibuat pada Tugas 4 dengan menggunakan CSS atau CSS framework (seperti Bootstrap, Tailwind, Bulma) dengan ketentuan sebagai berikut

 Kustomisasi halaman login, register, dan tambah inventori semenarik mungkin.

 Pertama-tama, dengan menggunakan Boostrap, Navbar ditambahkan pada base.html, sehingga dapat diinherit oleh setiap halamana yang termasuk login, register, dan tambah inventori sehingga navbar terlihat pada halaman tersebut. Kemudian, pada navbar ditambahkan tombol-tombol yang dapat menuju ke fungsi lain seperti login dan logout. Untuk kustomisasi pada halaman tersebut sendiri, ditambahkannya tag style di awal halaman, dan menambahkan element selector untuk tag seperti h1 dan button untuk merubah-rubah warna tulisan dan warna tombol.

 Kustomisasi halaman daftar inventori menjadi lebih berwarna maupun menggunakan apporach lain seperti menggunakan Card.

 Sama seperti sebelumnya, dengan navbar sudah terambil dari base.html, serta merubah berbagai tag seperti warna font, warna tulisan di table data, dan warna background. Sebagai tambahan, tombol di table juga diganti warna background dan tulisan.
