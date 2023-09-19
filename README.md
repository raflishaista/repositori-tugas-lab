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