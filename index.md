---
title: Adinda Febrianti - Data Specialist Portfolio
---

## Tentang
Halo, saya Adinda! Saya lulusan Program Studi Matematika, Institut Teknologi Bandung, dengan kelompok keahlian statistika. Saya memiliki passion besar untuk terus mengembangkan kemampuan analitik saya untuk menemukan informasi berbasis data. 

Berikut ini adalah resume saya [pdf](https://github.com/adndfebrianti26/Data-Analyst-Portofolio/blob/main/Adinda%20Febrianti-resume.pdf)

## Table of Contents
* [Tentang](#tentang)
* [Portfolio Projects](#portfolio-projects)
  * [Analisis Faktor Penyebab Kasus Celah Bibir dan Langit-Langit dengan Analisis Komponen Utama dan Generalized Linear Model](#analisis-faktor-penyebab-kasus-celah-bibir-dan-langit-langit-dengan-analisis-komponen-utama-dan-generalized-linear-model)
  * [Analisis Pergeseran Tingkat Pengangguran menggunakan Metode EWMA dan Shewhart](#analisis-pergeseran-tingkat-pengangguran-menggunakan-metode-ewma-dan-shewhart)
* [Pendidikan](#pendidikan)
* [Kontak](#kontak)

## Portfolio Projects
Di bagian ini, saya akan menampilkan proyek analisis data dan menjelaskan secara singkat rangkaian teknologi yang digunakan untuk menyelesaikan kasus tersebut.  

## Analisis Faktor Penyebab Kasus Celah Bibir dan Langit-Langit dengan Analisis Komponen Utama dan Generalized Linear Model
<p align="center"> <img src="https://github.com/adndfebrianti26/Data-Analyst-Portofolio/blob/main/Plot%20AKU-K%20Jawa%20Barat.png" width="500"> </p>

**Tujuan**: Identifikasi dimensi variabel penyebab kasus celah bibir dan langit menggunakan analisis komponen utama kategorikal, menentukan faktor yang berpengaruh secara signifikan terhadap jenis celah, dan menentukan apakah terdapat pengaruh perbedaan wilayah terhadap faktor penyebab kasus jenis celah. 

**Deskripsi**: Celah bibir dan langit-langit merupakan kelainan kongenital akibat gagalbya penyatuan jaringan wajah pada minggu ke-5 hingga minggu ke-9 kehamilan, yang berdampak pada kondisi fisik dan perkembangan kesehatan anak. Faktor penyebabnya bersifat kompleks dan saling berkaitan yang meliputi aspek genetik, orangtua, serta lingkungan, sehingga beresiko menimbulkan multikolinearitas antarvariabel. Dalam penelitian ini, digunakan data sekunder yang didapat dari penelitian di tahun 2023 di Jawa Barat dan Sulawesi Selatan. Data ini terdiri dari informasi pribadi penderita kasus mengenai jenis celah (variabel dependen) dan juga informasi nutrisi, lingkungan, dan juga orangtua penderita sebelum dan selama kehamilan. Distribusi jenis celah yang tidak normal, banyaknya faktor yang dipertimbangkan sebagai variabel independen, serta untuk mengetahui apa saja faktor yang berpengaruh secata signifikan digunakan Generalized Linear Model setelah diterapkan Analisis Komponen Utama Kategorikal(AKU-K) dan Bootstrapping. Bootstrapping digunakan dengan mempertimbangkan kondisi data yang imbalanced. 

**Skills**: data cleaning, data analysis, correlation matrices, hypothesis testing, data visualization.

**Teknologi**: Spreadsheet, SPSS, Rstudio, Minitab

**Hasil**: Proses dimulai dengan data cleaning menggunakan spreadsheet, kemudian dilakukan analisis komponen utama kategorikal adalah dengan menggunakan SPSS, hasilnya dilakukan bootstrapping menggunakan minitab, lalu Generalized Linear Model untuk melihat faktor yang berpengaruh secara signifikan menggunakan Rstudio. Hasilnya terdapat 4 variabel hasil leburan di wilayah Jawa Barat mencakup riwayat kesehatan ayah, riwayat kesehatan ibu, lingkungan ayah, dan lingkungan ibu. Sedangkan Sulawesi Selatan, berdasarkan hasil AKU-K terdapat 1 variabel hasil leburan yakni riwayat keguguran. Wilayah Jawa Barat memiliki variabel signifikan riwayat kesehatan ibu, masalah trimester pertama, rokok pasif ayah dan ibu, radiasi ayah dan ibu, olahraga ayah dan ibu, serta kafein ayah dan ibu. Wilayah Sulawesi Selatan memiliki variabel signifikan terhadap jenis celah diantaranya radiasi ibu, rokok pasif ibu, dan rokok pasif ayah. Kemudian pada data gabungan, variabel signifikan adalah wilayah, pemeriksaan kehamilan, masalah trimester pertama, dan beberapa faktor pola hidup orang tua. Sehingga, wilayah berpengaruh secara signifikan terhadap jenis celah.

## Analisis Pergeseran Tingkat Pengangguran menggunakan Metode EWMA dan Shewhart
![Median dan Mean Tingkat Pengangguran di Seluruh Benua Pada 1991-2021](https://github.com/adndfebrianti26/Data-Analyst-Portofolio/blob/main/Mean%20Median%20Dunia.png)
**Tujuan**: Menganalisis kestabilan tingkat pengangguran di beberapa negara Asia dan mendeteksi adanya pergeseran rata-rata dan hubungannya dengan krisis finansial yang terjadi.

**Deskripsi**: Krisis finansial Asia 1997 - 1998 merupakan krisis ekonomi besar yang melanda kawasan Asia, khususnya Asia Tenggara pada Juli 1997 hingga Mei 1998, dimulai dari jatuhnya mata uang Baht. Data yang digunakan dalam penelitian ini didapat dari Kaggle yang diambil dari data WorldBank. Data ini mencakup 235 negara dengan tahun tinjauan 1991-2021, dengan pembagian data training pada tahun 1991 - 1995 untuk penetapan nilai mu dan sigma dan data testing pada tahun 1996 - 2001 untuk melihat stabilisasi tingkat pengangguran. Metode yang digunakan adalah bagan kendali Shewhart yakni bagan kendali Xbar-R dan Xbar-S yang bergantung pada jumlah data yang terdapat di setiap daerah tinjauan, serta EWMA untuk mendeteksi pergeseran kecil yang terjadi. 

**Skills**: data cleaning, data analysis, data visualization.

**Teknologi**: Python

**Hasil**: Analisis bagan kendali Shewhart dan EWMA menunjukkan bahwa dari 41 negara yang ditinjau, terdapat 53,7% mengalami pergeseran naik, 9,8% mengalami pergeseran turun, dan 36,5% stabil. Hal ini menunjukkan dominasi kondisi tidak stabil dengan tren peningkatan pengangguran. Kemudian terjadi kenaikan struktural tingkat pengangguran. Dibandingkan benua lain yang mengalami penurunan rerata dan median. Di Asia justru menunjukkan bahwa efek krisis berkelanjutan. 

## Pendidikan
Institut Teknologi Bandung, Bandung :
Sarjana Matematika
2022 - 2026

## Kontak
* [LinkedIn: @AdindaFebrianti](https://linkedin.com/in/adinda-febrianti-370a44285)
* [Email: adndfebrianti26@gmail.com](mailto:adndfebrianti26@gmail.com)
