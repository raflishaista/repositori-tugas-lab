Apa perbedaan antara form POST dan form GET dalam Django?

POST dan GET adalah sama-sama merupakan HTTP request,yang didalam Django juga merupakan attribut dari HttpRequest, dimana keduanya memiliki fungsi berbeda, yaitu membaca dan mengambil data dari suatu server untuk GET, sedangkan mengirim data pada server untuk POST.

Apa perbedaan utama antara XML, JSON, dan HTML dalam konteks pengiriman data?

HTML dapat diibaratkan sebagai suatu amplop, dan XML dan HTML dapat diibaratkan sebagai surat dalam amplop tersebut. HTML merupakan protokol, dan XML serta JSON merupakan data format bagi data HTML, baik dalam request atau receive. Ini dapat dilihat dalam serializing, yang singkatnya mengkonversi suatu properti publik data ke format serial lain. Selain itu, XML dan HTML sama-sama merupakan markup language, namun JSON merupakan notasi. 

Mengapa JSON sering digunakan dalam pertukaran data antara aplikasi web modern?

Dalam aplikasi web modern, data dalam jumlah banyak perlu didisplay dan dikembalikan. JSON memiliki data format yang mudah untuk diparsing atau diurai, sehingga jika JSON digunakan, kode tambahan untuk parsing tidak diperlukan. Hal ini membuat JSON sangat membantu dalam pertukaran data dalam segi kecepatan, sehingga sering digunakan.

Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step 

Membuat input form untuk menambahkan objek model pada app sebelumnya.

Membuat file forms.py, dengan dibuat juga model dan field model tersebut yang digunakan untuk form, serta membuat dan mengubah juga fungsi untuk menerima data form. Selain itu, data url juga dimodifikasi, serta penambahan file display html untuk input form

Tambahkan 5 fungsi views untuk melihat objek yang sudah ditambahkan dalam format HTML, XML, JSON, XML by ID, dan JSON by ID.

Dengan mengimport HttpResponse dan seralizers, fungsi bagi setiap format ditambahkan, dengan serialization format yang berbeda, content type yang berbeda, dan parameter yang berbeda. 

Membuat routing URL untuk masing-masing views yang telah ditambahkan pada poin 2.

Mengimport fungsi yang telah ditambah, dan penambahan path untuk akses di penulisan url.

Mengakses kelima URL di poin 2 menggunakan Postman, membuat screenshot dari hasil akses URL pada Postman, dan menambahkannya ke dalam README.md.

HTML
<img width="1075" alt="html ss 2" src="https://github.com/raflishaista/tugas3/assets/124919851/2c7ae3e0-aecb-498a-8ade-cf7bf8278414">

XML
<img width="1072" alt="xml 2" src="https://github.com/raflishaista/tugas3/assets/124919851/f29f75fa-30e1-44a0-a69e-5269b8f3a539">


XML ID
<img width="1071" alt="xml id 2" src="https://github.com/raflishaista/tugas3/assets/124919851/c5b52ad7-7313-482d-891e-0516e5084f15">


JSON
<img width="1074" alt="json 2" src="https://github.com/raflishaista/tugas3/assets/124919851/bfab75fc-c39d-4dc0-b028-f273923a9960">

JSON ID
<img width="1076" alt="json id 2" src="https://github.com/raflishaista/tugas3/assets/124919851/0dfa04b7-efaa-4317-92f9-5f096511208a">



