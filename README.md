# TransJakarta Users Analysis - April 2023

## Introduction
Repositori ini berisi data dan analisis terkait PT. Transjakarta, sebuah perusahaan transportasi umum di Jakarta, Indonesia. Analisis bertujuan untuk mengoptimalkan kinerja armada Transjakarta dan aspek operasionalnya berdasarkan dataset yang tersedia. Peran analis data adalah memberikan rekomendasi untuk meningkatkan kualitas layanan dan efisiensi operasional.

## Backgorund
PT. Transjakarta mengoperasikan berbagai jenis layanan transportasi umum, termasuk BRT (Bus Rapid Transit), Non BRT, Royal Trans, Mikrotrans, Bus Wisata Terpadu, dan Transjabodetabek di wilayah Jakarta. Peningkatan terus-menerus melalui evaluasi bulanan sangat penting untuk memantau dan meningkatkan kinerja armada dan operasional Transjakarta, mengatasi masalah seperti kepadatan penumpang, kualitas infrastruktur, fasilitas ramah lansia, dan keselamatan perempuan.

## Goals
Tujuan dari analisis ini ingin mengetahui bagaimana karakteristik pengguna Transjakarta pada bulan April 2023. Selain itu, dari hasil analisis diharapkan dapat memberikan rekomendasi yang dapat diimplementasikan guna meningkatkan pengalaman transportasi bagi pengguna TransJakarta. Sehingga diharapkan nantinya dapat menempatkan Transjakarta sebagai pilihan moda transportasi utama yang digunakan pengguna.

## Data Understanding
- Dataset ini memiliki 22 kolom dan 37,900 baris.
- Rentang dari 1 April 2023 hingga 30 April 2023.
- Beberapa kolom memiliki missing value, yang akan diatasi dalam proses pembersihan data.
- Jenis data sebagian besar bersifat kategoris, dan beberapa kolom memerlukan konversi jenis data waktu.

## Data Cleaning
a. Duplikasi Data
Tidak ditemukan duplikasi data dalam dataset.

b. Missing Value
Sekitar 6% data mengandung nilai yang hilang. Nilai-nilai yang hilang terutama terdapat pada kolom-kolom yang terkait dengan koridor, halte, dan timestamp. Missing value diisi melalui mapping dan logika berdasarkan kolom-kolom tertentu. Apabila sudah tidak ada informasi yang dapat dipetakan, maka baris yang memiliki missing value akan dihilangkan untuk analisis.

c. Data Outlier
- Tidak ada anomali atau pencilan signifikan yang terdeteksi dalam data.

d. Normal Distribution
- Distribusi kolom numerik dalam dataset ini tidak berdistribusi normal

e. Data Formatting and Categorization
- Modifikasi Data Waktu
Kolom timestamp 'tapInTime' dan 'tapOutTime' diubah ke tipe data yang sesuai dan dibagi menjadi jam, hari, dan minggu untuk analisis lebih mendalam.
- Kategori payAmount menjadi 3 kelompok berdasarkan moda Transportasi yaitu JakLingko, Transjakarta dan Royal Trans
- Kategori umur pengguna menjadi 4 kelompok yaitu anak-anak, remaja, dewasa dan lansia

Dataset kini bersih dan siap untuk analisis lebih lanjut.

## Data Analysis
Dalam laporan ini, kami menyajikan analisis data penumpang Transjakarta dengan tujuan mengatasi tantangan-tantangan tertentu dan meningkatkan layanan secara keseluruhan. 
a. Penggunaan tipe moda Transjakarta
b. Profil pengguna TransJakarta berdasarkan jenis kelamin dan umur pengguna
c. Kartu bank pembayaran pengguna Transjakarta
d. Pola perjalanan pengguna
e. Waktu jam sibuk penggunaan Transjakarta
f. Pola penggunaan Transjakarta di waktu sibuk
g. Pola penggunaan Transjakarta di akhir pekan dan libur lebaran

## Conclusions
Kesimpulan dari analisis data bulanan untuk mengoptimalkan kinerja armada dan rute/halte Transjakarta adalah sebagai berikut:
1. Preferensi moda transportasi umum di Jakarta didominasi oleh Transjakarta, menunjukkan kecenderungan Masyarakat memilih opsi ekonomis dan efektif.
2. Mayoritas pengguna Transjakarta menggunakan kartu uang elektronik Bank DKI sebagai metode pembayaran, mencerminkan tingginya adopsi teknologi pembayaran non-tunai.
3. Proporsi penumpang wanita relatif seimbang dengan penumpang pria, tetapi perlu dipertimbangkan kembali perlunya armada khusus wanita di beberapa wilayah.
4. Wilayah penggunaan Transjakarta terpusat di Jakarta Pusat dan Jakarta Selatan, dengan tiga koridor utama Cibubur-Balai Kota, Ciputat - CSW, dan Harmoni - Jakarta International Stadium.
5. Jam sibuk terjadi pada pagi (5 pagi hingga 9 pagi) dan sore hari (4 sore hingga 8 malam), dengan tingkat penggunaan tertinggi pada Hari Senin.
6. Koridor 1T (Cibubur-Balai Kota) merupakan koridor terpadat, menunjukkan perlunya revitalisasi dan perluasan pada halte-halte strategis.
7. Penggunaan Transjakarta pada akhir pekan menurun, namun tiga koridor utama tetap diperlukan, terutama pada hari libur Lebaran dengan fokus pada koridor menuju terminal utama

## Recommendations

1. Optimalisasi Armada dan Fasilitas TransJakarta: Peningkatan armada pada koridor padat perlu disertai pengalihan dari koridor sepi, sambil memastikan ketersediaan armada sesuai dengan jumlah pengguna pada jam sibuk untuk meningkatkan efisiensi operasional. Revitalisasi halte, peningkatan fasilitas lansia, dan kampanye edukasi mendukung pengalaman perjalanan yang lebih baik.
2. Jam Operasional: Penyesuaian jam operasional armada pada jam sibuk, terutama pada hari Senin, adalah langkah strategis untuk menjaga kualitas pelayanan, mencegah overcrowding, dan memenuhi kebutuhan pengguna.
3. Penggunaan TransJakarta di Akhir Pekan dan Liburan: Pengalihan armada pada tempat yang sering dikunjungi di akhir pekan dan hari libur meningkatkan efisiensi layanan. Meratakan alokasi armada bus wisata membantu mengurangi waktu tunggu penumpang.
4. Evaluasi dan Adaptasi: Melalui umpan balik pengguna, evaluasi dan adaptasi strategi terimplementasi untuk perbaikan berkelanjutan dalam layanan TransJakarta.

Untuk dapat melihat representasi visualisasi dari analisis, juga dapat mengakses melalui dashboard Tableau pada link berikut:
(https://public.tableau.com/app/profile/yogiandrian/viz/TransJakartaUsersDashboard-Apr2023/Dashboard1)


