Project Data Wrangling

Penyusun

Nama: 

Nagatan Alief Putra Silahen    (24031554086)

Khansa Nadhifa 		 (1314622032)

Analisis Kualitas Udara (PM2.5) dan Kaitannya dengan GDP Per Kapita serta Pertumbuhan Penduduk (2010–2019)

1. Pendahuluan

Project ini bertujuan untuk melakukan proses Data Wrangling dan analisis eksploratif terhadap hubungan antara PM2.5 (kualitas udara), GDP per kapita, dan jumlah penduduk di berbagai negara pada periode 2010–2019.
Melalui tahapan pengolahan data yang sistematis, penelitian ini difokuskan untuk melihat pola hubungan ekonomi, populasi, dan kualitas udara secara global.

Project ini dirancang sebagai bagian dari pemenuhan tugas mata kuliah Data Wrangling / Pengolahan Data, dengan alur kerja mulai dari cleaning, pre-processing, integrasi data, feature engineering, hingga exploratory data analysis (EDA).

2. Dataset yang Digunakan

Analisis ini menggunakan tiga dataset utama:

PM2.5 Air Pollution – berisi tingkat polusi udara partikel halus PM2.5 per negara.

GDP Per Capita (World Bank) – data tingkat pendapatan per kapita setiap negara.

Population Dataset – berisi jumlah penduduk tahunan setiap negara.

Seluruh dataset difokuskan pada tahun 2010–2019.

3. Tahapan Pengolahan Data
3.1 Data Cleaning

Pada tahap pembersihan data dilakukan beberapa hal, antara lain:

Menormalisasi nama kolom agar konsisten.

Menghapus kolom yang tidak relevan (misal kolom Unnamed).

Menyaring data berdasarkan tahun 2010–2019.

Menghapus entitas yang bukan negara (misalnya region atau group).

Mengonversi tipe data untuk memastikan akurasi proses selanjutnya.

File hasil cleaning disimpan dalam folder Data Cleaning.

3.2 Pre-Processing

Proses pre-processing dilakukan untuk menyiapkan dataset sebelum diintegrasikan.
Tahapan ini meliputi:

Mengubah kolom Year menjadi integer.

Memfilter data berdasarkan negara menggunakan Country Code tiga karakter.

Mengubah struktur GDP menjadi bentuk long format agar mudah digabungkan.

Hasil pre-processing disimpan dalam folder Pre-Processing.

3.3 Integrasi Data

Pada tahap ini dilakukan penggabungan dataset PM2.5, GDP per kapita, dan populasi berdasarkan kolom kunci:

Country_Code

Year

Tahap ini menghasilkan dataset terpadu yang akan digunakan untuk analisis lebih lanjut.
Hasil integrasi tersedia dalam folder Integrasi Data.

3.4 Feature Engineering

Tahapan ini bertujuan menghasilkan fitur-fitur baru yang dapat meningkatkan kualitas analisis, antara lain:

Selisih tahunan (YoY) untuk PM2.5, GDP per kapita, dan populasi.

Persentase perubahan dari setiap variabel tahunan.

Kategorisasi tingkat polusi menjadi: Low, Moderate, dan High.

Transformasi logaritmik untuk menstabilkan distribusi GDP dan populasi.

Hasil feature engineering disimpan dalam folder Future Engineering.

3.5 Exploratory Data Analysis (EDA)

Tahap EDA dilakukan untuk meninjau pola dan hubungan antar-variabel.
Visualisasi yang dihasilkan mencakup:

Tren PM2.5 untuk beberapa negara.

Korelasi GDP per kapita dengan PM2.5.

Korelasi populasi dengan PM2.5.

Boxplot kategori tingkat polusi.

Heatmap korelasi antar variabel utama.

10 negara dengan tingkat PM2.5 tertinggi dan terendah.

Semua hasil visualisasi disimpan dalam folder EDA (Visualisasi).

4. Hasil dan Temuan

Beberapa temuan awal dari analisis:

Negara dengan GDP per kapita tinggi cenderung memiliki tingkat PM2.5 lebih rendah, menunjukkan hubungan antara peningkatan pembangunan ekonomi dan kualitas lingkungan yang lebih baik.

Negara dengan jumlah penduduk besar sering menunjukkan tingkat PM2.5 lebih tinggi, meskipun faktor ini dipengaruhi juga oleh industrialisasi dan kebijakan lingkungan masing-masing negara.

Tren PM2.5 berbeda-beda antar negara: beberapa mengalami penurunan konsisten, sementara yang lain tetap tinggi.

5. Tools dan Library

Project ini dikembangkan menggunakan:

Python 3

Pandas

NumPy

Matplotlib

Seaborn

6. Cara Menjalankan Proyek

Jalankan file utama:

Projek Data Wrangling.ipynb

7. Penutup

Melalui proses Data Wrangling dan analisis visual, proyek ini berhasil menggambarkan hubungan antara kualitas udara, kondisi ekonomi, dan jumlah penduduk.
Diharapkan penelitian ini dapat menjadi referensi dalam memahami pentingnya sinergi antara pembangunan ekonomi dan keberlanjutan lingkungan.

Project ini dibuat sebagai bagian dari pemenuhan tugas mata kuliah Data Wrangling.
