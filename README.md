Jelaskan perbedaan antara asynchronous programming dengan synchronous programming.
Perbedaan utama kedua apporach programming tersebut terletak pada cara merekea mengerjakan tugas. Pada synchronous programming, jika suatu task atau tugas ingin dijalankan, jika ada task yang belum selesai dan sedang dijalankan, task baru tidak bisa dikerjakan, namun harus menunggu task sebelumnya selesai, sehingga setiap task dapat disebut bergantung pada task lain.. Karena ini, synchronous merupakan blocking architecture, yang hanya mengirim server satu request pada setiap waktu. Asynchronous merupakan non-blocking architecture, dimana setiap task tidak ebrgantung dengan task lain dan dapat berjalan dengan sendiri tanpa menunggu task lain. Asynchronous juga multi thread yang berarti task tersebut berjalan di parallel, sedangan synchronous single thread.

Dalam penerapan JavaScript dan AJAX, terdapat penerapan paradigma event-driven programming. Jelaskan maksud dari paradigma tersebut dan sebutkan salah satu contoh penerapannya pada tugas ini.
Event driven intinya merupakan programming yang dapat bereaksi terhadap aksi dari pengguna, seperti klik dan aksi lainnya. Ketika user melakukan aksi, sebuah event terjadi yang dapat dideteksi oleh kode, kemudian kode tersebut menjalankan fungsi dan merubah page. Salah satu penerapannya adalah menambahnya card/tabel pada produk ketika sebuah fungsi menambah produk diselesaikan.

Jelaskan penerapan asynchronous programming pada AJAX.
Dengan AJAX, asynchronous programming memungkinkan user untuk dapat berinteraksi dengan halaman walaupun ketika data sedang loading. Ajax membuat ini dapat terjadi dengan menukar data dengan web server dibalik permukaan, yang memungkinkan bagian-bagian dari sebuah web page diupdate tanpa mereload semua halaman. Ajax mengimplementasinya dengan fungsi-fungsinya, seperti request. dengan parameter sesuai, yang memungkinkan JavaScript untuk mengirim request tapi tidak menunggu jawaban, sehingga dapat melakukan task lain dan memproses ketika hjlaman masih bisa direspond.

Pada PBP kali ini, penerapan AJAX dilakukan dengan menggunakan Fetch API daripada library jQuery. Bandingkanlah kedua teknologi tersebut dan tuliskan pendapat kamu teknologi manakah yang lebih baik untuk digunakan.
Keduanya kebanyakan dibandingkan pada kemampuan dalam memproses protokol, seperti request. Namun, keduanya ada perbedaan, seperti jquery yang merupakan sebuah library eksternal, dan Fetch yang merupakan API dan juga method baru pada jQuery.Walaupun jQuery lebih tua sehingga lebih aman digunakan karena lebih kompatibel dengan versi lama yang masih menggunakannya, Fetch dapat dibilang lebih baik untuk digunakan, karena dapat dibilang baru merupakan bagian integral bagi engine atau sistem JavaScript.

Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).
Mengubah tugas 5 yang telah dibuat sebelumnya menjadi menggunakan AJAX.

 AJAX GET

 Ubahlah kode cards data item agar dapat mendukung AJAX GET.
 Memindahkan cards yang pada awalnya berada di bagian utama HTML, menjadi sebuah fungsi untuk menampilkan cards secara asynchronous di dalam tag script.
 
 Lakukan pengambilan task menggunakan AJAX GET.
Menggunakan fetch yang mengambil suatu fungsi yang mengambil item berdasarkan user, yang lalu mengeluarkan response berupa JSON. Ini akan digunakan ketika merefresh cards item.
 
 AJAX POST

 Buatlah sebuah tombol yang membuka sebuah modal dengan form untuk menambahkan item.
 Menambahkan tombol dengan fungsi dari bootstrap, yang dapat mentoggle atau memunculkan dan menghilangkan tanpa mengubah halaman yang melakukan suatu fungsi untuk menambahkan item. Ada juga fungsi reset() untuk menghilangkan submisi sebelumnya.
 
 Buatlah fungsi view baru untuk menambahkan item baru ke dalam basis data.
 Di view, membuat fungsi create_ajax, yang mendeteksi sebuah request jika request POST, dimana akan mendeteksi semua bagian form dari request yang di get sesuai variabel yang dibutuhkan item, dan membuat item baru dari data tersebut dan menambahkannya. Jika sukses, akan mengembalikan response HTTP.

 Buatlah path /create-ajax/ yang mengarah ke fungsi view yang baru kamu buat.
 Di urls.py, mengimport fungsi view tersebut dan menghubungkannya di urls, dengan menambahkan path yang menuju /create-ajax/ dan menambahkan fungsi tersebut kepada path.

 Hubungkan form yang telah kamu buat di dalam modal kamu ke path /create-ajax/.
 Di kode bootstrap pada html, pertama membuat form yang menerima input, serta button untuk submit. Pada button tersebut, tambahkan suatu id. Lalu, pada kode script yang berada pada tag script, buat suatu fungsi yang dapat mengambil button tersebut melalui id, seperti .onclick, yang akan run suatu fungsi yang menambahkan data pada form sebagai item.

 Lakukan refresh pada halaman utama secara asinkronus untuk menampilkan daftar item terbaru tanpa reload halaman utama secara keseluruhan.
Membuat suatu fungsi yang merefresh card, baik dengan menimpa atau overwrite kumpulan card dengan kumpulan card baru yang menyertai card item yang sudah ditambahkan atau cara lain, kemudian memanggil fungsi tersebut pada fungsi menambah produk, sehingga ketika fungsi menambah produk dilakukan, refresh akan dilakukan secara otomatis.

 Melakukan perintah collectstatic.
Pada settings.py, menambahkan terlebih dahulu sebuah path root STATIC_ROOT sebagai folder untuk menyimpan static file, di dekat STATIC_URL. Kemudian, run py manage.py collectstatic, yang akan membuat folder tersebut dan mengisinya secara otomatis.

app:http://rafli-aditya-tugas.pbp.cs.ui.ac.id/
