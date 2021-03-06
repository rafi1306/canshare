## Laporan Akhir Projek

- Nama sistem, Paralel, Kelompok, Nama Asisten Praktikum
  * Nama Sistem : Canshare (Cancer Donation dan Consultation) 
  * Kelompok : 8 
  * Paralel : Kelas P3
  * Nama Asisten Praktikum :
    * Qorry Atul Chairunnisa (G64170014)
    * Indah Puspita (G64170035)
    
- Nama Anggota:
1. I Ketut Gede Arta Putra (G24180034) as Designer UI/UX
2. Rafi Adiapratama (G24180035) as Back end
3. Eryana Nurwenda Az-Zahra (G24180055) as Front end
4. Athirotul Wardah MY (G24180058) as Analyst
 
- Deskripsi Singkat
  * Canshare: Cancer Donation and Consultation merupakan sebuah platform yang mewadahi para donatur yang ingin berdonasi bagi penderita kanker. Hampir sama seperti platform-platform donasi yang sudah ada, tetapi platform Canshare ini dikhususkan untuk pengguna yang ingin berdonasi kepada penderita kanker saja dan ditargetkan kepada pengguna (donatur dan penderita kanker) yang khususnya berada di Indonesia. Tidak hanya itu, Canshare juga mempunyai fitur bagi penderita kanker untuk berkonsultasi kepada dokter mengenai berbagai hal tentang penyakit kanker. Canshare berbentuk sebuah aplikasi berbasis web yang dengan mudah dapat diakses oleh siapapun, dimanapun, dan kapanpun. Aplikasi ini diharapkan dapat membantu dan meringankan biaya pengobatan bagi penderita kanker yang membutuhkan, selain itu diharapkan memudahkan donatur ataupun aktivis yang ingin membantu penderita kanker.

- User analysis
  * User story
1. Sebagai user, agar dapat berdonasi dan berbagi cerita di web CanShare, saya dapat melakukan registrasi akun menggunakan email
2. Sebagai seorang admin, agar dapat me-validasikan akun user yang mendaftar, saya dapat menyetujui akun tersebut dapat terdaftar atau tidak
3. Sebagai seorang user yang memiliki akun, agar dapat melakukan konsultasi dengan dokter spesialis, saya dapat melihat biodata dokter spesialis pada laman “konsultasi”
4. Sebagai seorang dokter spesialis, agar dapat menampilkan profil diri, saya dapat melakukan registrasi akun menggunakan email
5. Sebagai seorang dokter spesialis yang memiliki akun, agar dapat mengenalkan diri, saya dapat menampilkan profil serta kontak saya pada laman “konsultasi” lalu “profil dokter”
6. Sebagai seorang user yang memiliki akun, agar dapat membagikan postingan, saya dapat langsung menulis postingan pada laman beranda
7. Sebagai seorang user, agar dapat mengajukan donasi, saya dapat langsung melengkapi data pada laman donasi

- Spesifikasi teknis lingkungan pengembangan
  * Perangkat Keras
    * Processor : Quad-Core 3.2 gigahertz (GHz)
    * Graphics Card : DirectX 12 dengan VRAM 2GB GDDR5
    * RAM : 8 GB
  * Perangkat Lunak
    * Framework : PHP, Tailwind CSS
    * Database : MySQL
    * Server : Apache
    * Text Editor/IDE : Visual Studio Code
  * Lainnya
    * Version Control dan Collaboration Platform : Github
    * Teknologi : HTML, CSS, Javascript, dan PHP

- Hasil dan pembahasan
  * Use case diagram
    * ![RPL-use case diagram (1)](https://user-images.githubusercontent.com/78951884/121375750-2981fb00-c96b-11eb-8026-cb5a169f77a2.png)
  * Activity diagram
    * Memposting cerita
      *![RPL-act-bercerita](https://user-images.githubusercontent.com/78951884/121376326-a1502580-c96b-11eb-921d-875019acf7ba.png)
    * Mengajukan donasi
      *![RPL-act diagram-mengajukan](https://user-images.githubusercontent.com/78951884/121378815-b9c13f80-c96d-11eb-9819-44ac20ef51c4.png)
    * Melakukan donasi
      *![RPL-act-berdonasi](https://user-images.githubusercontent.com/78951884/121376754-f8ee9100-c96b-11eb-89e2-f05b8972cf5c.png)
    * Melakukan konsultasi
      *![RPL-act-konsultasi](https://user-images.githubusercontent.com/78951884/121378303-47505f80-c96d-11eb-97e1-7c1cf3ea3942.png)
  * Class diagram
    * ![canshare-Class diagram](https://user-images.githubusercontent.com/78951884/121569768-5574ad80-ca4b-11eb-88c4-2ee8e576576c.png)
  * Entity Relationship Diagram
    * ![canshare-ERD](https://user-images.githubusercontent.com/78951884/121046736-44743400-c7e0-11eb-8ad2-ef940497be4c.png)
  * Arsitektur sistem
     1. MySQL (Database)
        -  Ringkasan: Untuk mengelola data, kami memutuskan untuk menggunakan mySQL.
        -  Masalah: Data yang digunakan kemungkinan akan sangat banyak dikarenakan fitur cerita yang dapat digunakan oleh pengguna (penderita kanker) sehingga terjadi update terus menerus. Oleh karena itu dibutuhkan penyimpanan yang memadai dan sistem data yang terstruktur agar tidak terjadi error ataupun overload.
        -  Batasan: Fasilitas pemrograman tidak lengkap seperti looping atau percabangan, namun fitur-fitur lain yang dimiliki cukup untuk pengembangan software kami.
        -  Opsi: Beberapa pilihan aplikasi pengelola data base yang pernah kami gunakan adalah MySQL dan MongoDB, akan tetapi MongoDB ketika dipasangkan PHP (salah satu bahasa pemrograman yang kami gunakan) harus merestart server meskipun dalam penggunaannya lebih mudah karena tidak membutuhkan relasi atau skema untuk setiap tabel. MySQL lebih kompatibel dengan bahasa PHP, tidak rumit, serta mendukung record dengan panjang tetap atau bervariasi.
        -  Rasional: kami memilih MySQL karena pengalaman yang dimiliki dalam menggunakannya serta fitur yang memadai dan sesuai kebutuhan pengembangan.
    2. Visual Studio Code (Text Editor)
        -  Ringkasan: Untuk text editor, kami memutuskan untuk menggunakan Visual Studio Code.
        -  Masalah: Aplikasi berbasis website membutuhkan desain yang menarik terutama dalam hal warna. Visual Studio Code memfasilitasi user untuk menambahkan warna latar dan dapat menampilkan kotak color picker sehingga dapat mengubah warna sesuai dengan apa yang diinginkan. Namun, Visual Studio Code tidak terlalu responsif dalam menjalankan command. Sehingga membutuhkan waktu yang cukup lama untuk menjalankan fitur-fitur yang tersedia.
        -  Batasan: Untuk proyek kali ini hanya dalam bentuk website saja. Visual Studio Code memiliki performa yang belum cukup baik dibandingkan text editor yang lain. Selain itu, Visual Studio Code juga memiliki shortcut key yang berbeda yaitu menggunakan ALT bukan CTRL.
        -  Opsi: Beberapa opsi untuk text editor adalah Visual Studio Code dan Sublime Text. Kedua opsi ini memiliki kelebihan dan kekurangannya masing-masing. Visual Studio Code memiliki banyak ekstensi yang memudahkan developer untuk men-develop aplikasi.
        -  Rasional: Karena visual studio code merupakan aplikasi yang gratis dan banyak memiliki ekstensi jadi kami memutuskan untuk menggunakannya.
     * 3. HTML, CSS, PHP, JavaScript (Bahasa pemrograman)
         -  Ringkasan: Untuk membuat aplikasi web Canshare, kami memutuskan untuk menggunakan bahasa pemrograman HTML, CSS, PHP, dan JavaScript.
         -  Masalah: Pembuatan aplikasi web Canshare yang menggunakan HTML, CSS, PHP, dan Javascript membutuhkan waktu yang tidak sedikit untuk menguasai bahasa pemrograman tersebut, karena sebelumnya belum pernah mempelajarinya sebab dalam mata kuliah hanya mempelajari bahasa python. Namun masih terdapat waktu untuk mempelajari bahasa pemrograman tersebut hingga batas waktu pembuatan aplikasi Canshare.
         -  Batasan: HTML, CSS, PHP, dan Javascript merupakan pemrograman dasar untuk pembuatan aplikasi web yang saling berhubungan dan merupakan satu kesatuan, sehingga jika salah satu mengalami permasalahan, maka aplikasi web Canshare akan bermasalah.
         -  Opsi: Python, karena phyton mudah digunakan, dinamis dan semua anggota tim pernah mempelajarinya. Meskipun lebih dikenal sebagai bahasa program back-end, python juga bisa diterapkan pada front-end. Namun phyton tidak secepat dan seefektif bahasa program lainnya dalam hal statis.
         -  Rasional: HTML, CSS, PHP, dan Javascript dipilih karena lebih memungkinkan untuk digunakan dan juga merupakan bahasa pemrograman yang lebih umum dan sering digunakan oleh pengembang dan pembuat aplikasi web, sehingga banyak komunitas yang bisa membantu ketika terjadi permasalahan.

  * Fungsi utama yang dikembangkan
    * Donasi
      - Pengguna memungkinkan untuk berdonasi yang ditujukan kepada penderita kanker.
    * Konsultasi dokter
      - Pengguna dapat berkonsultasi kepada dokter tentang masalah kesehatan terutama penyakit kanker, baik pasien maupun non-pasien.
    * Berbagi cerita
      - Pengguna yang memiliki pengalaman dan telah bertahan hidup melawan kanker dapat menceritakannya lalu membagikannya ke khalayak umum.

  * Fungsi CRUD
    * ![WhatsApp Image 2021-06-11 at 12 36 53 AM](https://user-images.githubusercontent.com/78951884/121610196-aa321b80-ca7f-11eb-942a-558cc9c30bcd.jpeg)

- Hasil implementasi
  ![WhatsApp Image 2021-06-11 at 09 10 30](https://user-images.githubusercontent.com/79292082/121616374-60ecc680-ca95-11eb-96be-feee4906dae9.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 30 (1)](https://user-images.githubusercontent.com/79292082/121616392-677b3e00-ca95-11eb-99b5-87eff7c96575.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 30 (2)](https://user-images.githubusercontent.com/79292082/121616398-6a762e80-ca95-11eb-9c95-2bfd25f4189f.jpeg) 
  ![WhatsApp Image 2021-06-11 at 09 10 31](https://user-images.githubusercontent.com/79292082/121616415-73ff9680-ca95-11eb-96e1-de8275c569d0.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 31 (1)](https://user-images.githubusercontent.com/79292082/121616420-76fa8700-ca95-11eb-8aa4-bf3495f85645.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 31 (2)](https://user-images.githubusercontent.com/79292082/121616434-7f52c200-ca95-11eb-8aa0-fcff0f07b771.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 32](https://user-images.githubusercontent.com/79292082/121616443-837edf80-ca95-11eb-9083-a6a3bcd10d7e.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 32 (1)](https://user-images.githubusercontent.com/79292082/121616456-87126680-ca95-11eb-896c-b05eea23dfa0.jpeg)
  ![WhatsApp Image 2021-06-11 at 09 10 32 (2)](https://user-images.githubusercontent.com/79292082/121616469-8b3e8400-ca95-11eb-9abe-8542bcffe965.jpeg)
  
- Testing (Test cases)
  * ![WhatsApp Image 2021-06-11 at 6 46 17 AM](https://user-images.githubusercontent.com/78951884/121610859-29741f00-ca81-11eb-9af7-83cd226e94c3.jpeg) 

- Saran untuk pengembangan selanjutnya
   * Pokok ide sebaiknya dimatangkan lebih cepat di awal
   * Membuat fitur ajukan donasi yang lebih terpusat dalam web
   * Mengembangkan fitur agar dapat melakukan konsultasi langsung dalam web
   * Memperbaiki manajemen dalam implementasi

