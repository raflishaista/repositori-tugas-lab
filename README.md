Apa itu Django UserCreationForm, dan jelaskan apa kelebihan dan kekurangannya?

UserCreationForm merupakan model built-in yang berasal dari class ModelForm. UserCreationForm digunakan untuk membuat user baru yang dapat menggunakan web, sehingga memiliki3 field yaitu username, password1, dan password2 untuk konfirmasi. Disini, kelebihan modul tersebut dapat terlihat, yaitu adanya field password2 untuk konfirmasi, sehingga pembuatan akun dapat meminimalisir kelemahan. Bagi kekurangannya, styling membutuhkan usaha yang lebih besar dibandingkan form lainnya.

Apa perbedaan antara autentikasi dan otorisasi dalam konteks Django, dan mengapa keduanya penting?
Autentikasi adalah pengecekan bahwa sebuah validasi memang apa saja yang "diklaim" atau diakui memang dari dirinya sendiri, sedangkan otorisasi adalah menentukan apa saja yang bisa diakses user. Keduanya penting karena merupakan bagian dari keamanan suatu proyek Django, dan dapat mempertahankan integritas proyek tersebut serta menjamin keamanan pengguna.

Apa itu cookies dalam konteks aplikasi web, dan bagaimana Django menggunakan cookies untuk mengelola data sesi pengguna?
Cookies adalah data kecil yang dikirim oleh web server pada sebuah browser, kemudian dikembalikan kembali oleh browser ketika ada request. Jadi, cookies merupakan data yang disimpan di browser untuk sementara. Django mengelola cookie pada pengelolaan server session, dimana ada handling untuk webserver secara otomatis 

Apakah penggunaan cookies aman secara default dalam pengembangan web, atau apakah ada risiko potensial yang harus diwaspadai?
Cookies sebenarnya hanya informasi dan bukan sebuah kode sehingga tidak bisa membaca/memproses/menghapus apapun dari platform/komputer. Namun, masih ada resiko dari cookie yang mudah diakses, sehingga harus diwaspadai untuk tidak menyimpan data sensitif sebagai cookie.

Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial).

Mengimplementasikan fungsi registrasi, login, dan logout untuk memungkinkan pengguna untuk mengakses aplikasi sebelumnya dengan lancar.

Pada views.py, membuat ketiga fungsi tersebut dengan parameter request yang akan diproses pada fungsi sesuai HTTP method yang dibutuhkan tiap fungsi (yang kebanyakan POST ). Autentikasi dan validasi form juga dibuat pada register dan login user, serta adanya pengelolaan cookie pada login user dan logout. Fungsi File markup HTML pada setiap fungsi juga dibuat.

Membuat dua akun pengguna dengan masing-masing tiga dummy data menggunakan model yang telah dibuat pada aplikasi sebelumnya untuk setiap akun di lokal.

Register dahulu dua akun yang dibuat, kemudian, login pada setiap akun dan membuat 3 dummy data berupa produk kartu.Ketika login ke akun satu lagi, dan jika data berbeda, maka sudah sukses.

Menghubungkan model Item dengan User.

Menambahkan suatu variabel pada models.py yang mengambil key dari satu tabel yang berupa data user, menambahkan deteksi dan pengambilan identitas user yang mengirim request dari proses login, kemudian menambahkan fungsi show_main suatu cara untuk mengakses data item dari user yang login dan juga nama dari user yang login.

Menampilkan detail informasi pengguna yang sedang logged in seperti username dan menerapkan cookies seperti last login pada halaman utama aplikasi.

Menambahkan cara pada fungsi yang mengelola variabel untuk dapat mengakses/mengambil nama dari user yang login. Untuk menunjukkan cookies, memberikan fungsi untuk merekam/set suatu data, menambahkan variabel yang bisa ditunjukkan yang mengambil dari data tersebut, dan juga menambahkan cara untuk menghapus data tersebut ketika logout jika dibutuhkan.