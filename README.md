
Software Requirements Specification

for
<Web Smart Parking System Berbasis IoT>

Version 1.0 approved
Prepared by 

< 22091397076 - Albiona Qalbu Shoukhi >

< 22091397077 – Ageng Kurniawan >

< 22091397087 – Danar Adrian  Ridho Nugroho>


D4 Manajemen Informatika 2022 C
< 09 September 2023 > 

1.	Pendahuluan

1.1	Tujuan Penulisan Dokumen
Dokumen ini bertujuan untuk menyediakan spesifikasi persyaratan web yang lebih rinci untuk proyek Smart Parking System. Tujuan utamanya adalah untuk mengidentifikasi dan menjelaskan persyaratan fungsional dan nonfungsional yang harus dipenuhi oleh sistem.

1.2	Konvensi Dokumen

Konvensi Dokumen diisi dengan istilah dan singkatan yang akan digunakan pada dokumen ini, dan pengertiannya akan dijelaskan dengan bahasa yang sederhana dan bisa dimengerti oleh client.

•	IoT : IoT atau Internet of Things adalah sebuah konsep di mana berbagai perangkat bersensor saling terhubung melalui internet untuk mengumpulkan dan mentransfer data.

•	TensorFlow : sebuah framework berbasis Python yang digunakan di pembelajaran mesin untuk mengembangkan dan membuat neural netwrok.

•	Framework : . Framework ini adalah open-source, dan bisa digunakan untuk beragam tugas yang bervariasi selain untuk membangun neural network.

•	HTML :

•	CSS :

•	JavaScript :

•	Scikit-learn : Scikit-learn dianggap sebagai salah satu library bahasa pemerograman terbaik untuk bekerja dengan data yang kompleks.

•	Machine Learning : teknologi yang dikembangkan untuk mengadopsi kemampuan belajar manusia pada komputer.

•	Raspberry Pi : sebuah komputer papan tunggal (single-board computer) atau SBC seukuran kartu kredit yang dapat digunakan untuk menjalankan program perkantoran, permainan komputer, dan sebagai pemutar media hingga video beresolusi tinggi.

•	Linux-based OS : sistem operasi yang menggunakan kernel Linux sebagai inti dan disertakan aplikasi dan module pendukung lain agar berfungsi dan bisa digunakan secara utuh layaknya sistem operasi pada umumnya.
•	Router dan switch : Router dan switch adalah perangkat jaringan yang digunakan untuk menghubungkan beberapa perangkat dalam jaringan komputer.

•	Server : sistem komputer yang memberikan fasilitas berupa sumber daya untuk pusat penyimpanan data dan juga layanan khusus.

•	Database : kumpulan data yang terorganisir dan saling terhubung sehingga dapat diakses dengan mudah.

•	Hardware : komponen fisik pada komputer yang berfungsi untuk melakukan proses input, proses, dan output.

•	Software : program atau aplikasi yang diinstal pada perangkat keras.

•	Arduino : platform elektronik open-source yang digunakan untuk membuat berbagai jenis proyek dan perangkat elektronik, seperti robot, sistem kendali otomatis, dan alat ukur.

•	Mikrokontroler/SBC : Mikrokontroler atau SBC (Single Board Computer) adalah sebuah komputer kecil yang terdiri dari satu papan sirkuit yang memuat semua komponen yang dibutuhkan untuk menjalankan sistem operasi dan aplikasi.

1.3	Audien yang Dituju dan Pembaca yang Disarankan

Dokumen ini ditujukan untuk pengembang web, manajer proyek, pengguna, dan pihak terkait lainnya yang terlibat dalam pengembangan dan penggunaan Smart Parking System. Disarankan untuk membaca dokumen ini secara keseluruhan untuk memahami persyaratan sistem secara menyeluruh.

1.4	Lingkup Produk

•	Deskripsi Umum :

o	Proyek ini bertujuan untuk mengembangkan sebuah sistem parkir pintar yang memanfaatkan teknologi IoT, Machine Learning, dan Webcam untuk meningkatkan efisiensi dan pengelolaan parkir.

o	Sistem ini akan memantau dan mengelola tempat parkir secara real-time, memberikan informasi tentang ketersediaan tempat parkir kepada pengguna, serta memungkinkan pengguna untuk melakukan reservasi tempat parkir.




•	Fungsi Produk :
o	Mendeteksi dan melacak ketersediaan tempat parkir menggunakan data dari sensor dan kamera CCTV.
o	Menampilkan informasi ketersediaan tempat parkir kepada pengguna melalui aplikasi atau layar informasi yang terpasang di area parkir.
o	Memungkinkan pengguna untuk melakukan reservasi tempat parkir melalui aplikasi atau sistem online.
o	Mengintegrasikan sistem pembayaran parkir secara otomatis.
•	Karakteristik Pengguna :
o	Pengguna utama sistem ini adalah pengemudi yang mencari tempat parkir.
o	Pengguna lainnya termasuk administrator parkir, operator sistem, dan pemilik tempat parkir.
•	Lingkungan Operasi :
o	Sistem ini akan beroperasi di area parkir umum atau area parkir yang telah ditentukan.
o	Membutuhkan konektivitas internet untuk mentransfer data dan informasi antara perangkat dan server.


1.5	Refrensi

•	(PDF) IoT -Parking Lot Detection Based on Image Processing | I Made Edy Listartha - Academia.edu
•	Sistem Informasi Parkir Pintar berbasis Web dan IoT | Prosiding Seminar Nasional Teknik Elektro UIN Sunan Gunung Djati Bandung (uinsgd.ac.id)
•	https://ejournal.ubhara.ac.id/jeecs/article/download/47/38
•	IoT-based Smart Parking System Development - MobiDev
•	Machine Learning and IoT based Real Time Parking System: Challenges and Implementation by Ravi Kumar Gupta, Geeta Rani :: SSRN
•	Smart parking system using IoT - Mokosmart.com
•	Smart Parking with Prediction of Available Spots: A Proposed Approach (ijsr.net)
2.	Deskripsi Keseluruhan

2.1	Deskripsi Produk 

Smart Parking System adalah sebuah produk berbasis teknologi yang dirancang untuk mengoptimalkan penggunaan tempat parkir dengan menggunakan Internet of Things (IoT), machine learning, dan webcam. Produk ini menggabungkan teknologi canggih untuk memberikan solusi parkir yang efisien, nyaman, dan terhubung secara digital.
Dengan menggunakan perangkat keras seperti sensor IoT, kamera webcam, dan sistem komputasi yang terintegrasi, Smart Parking System dapat mendeteksi ketersediaan tempat parkir secara real-time. Data ketersediaan parkir kemudian diproses melalui algoritma machine learning yang cerdas untuk memberikan informasi akurat kepada pengguna.

2.2	Fungsi Produk 

•	Memantau dan mengelola slot parkir yang tersedia.
•	Menyediakan informasi real-time tentang ketersediaan parkir kepada pengguna.
•	Mengatur reservasi dan pembayaran parkir.
•	Membantu pengguna menemukan tempat parkir yang tersedia dengan cepat dan efisien.
•	Menyediakan laporan dan analisis mengenai penggunaan parkir.
2.3	Penggolongan Karakterik Pengguna
<Identifikasi berbagai golongan pengguna yang terkait dengan produk yang dikembangkan>

Tabel 1 Karakteristik Pengguna

Kategori Pengguna	Tugas	Hak Akses ke web	Kemampuan yang harus dimiliki
Driver	Mencari tempat parkir	Membaca informasi parkir	Menggunakan aplikasi smart parking, melakukan pembayaran
Parking Attendant	Memantau slot parkir	Mengakses data parkir. Mengoperasikan sistem smart parking, memberikan bantuan kepada pengemudi
System Administrator	Mengelola pengaturan sistem	Mengakses pengaturan sistem	Memahami konfigurasi sistem smart parking, melakukan pemeliharaan perangkat keras, melatih model machine learning

