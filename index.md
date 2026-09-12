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
![Plot AKU-K Jawa Barat](Plot%20AKU-K%20Jawa%20Barat.png)

**Tujuan**: Identifikasi dimensi variabel penyebab kasus celah bibir dan langit menggunakan analisis komponen utama kategorikal, menentukan faktor yang berpengaruh secara signifikan terhadap jenis celah, dan menentukan apakah terdapat pengaruh perbedaan wilayah terhadap faktor penyebab kasus jenis celah. 

**Deskripsi**: Celah bibir dan langit-langit merupakan kelainan kongenital akibat gagalbya penyatuan jaringan wajah pada minggu ke-5 hingga minggu ke-9 kehamilan, yang berdampak pada kondisi fisik dan perkembangan kesehatan anak. Faktor penyebabnya bersifat kompleks dan saling berkaitan yang meliputi aspek genetik, orangtua, serta lingkungan, sehingga beresiko menimbulkan multikolinearitas antarvariabel. Dalam penelitian ini, digunakan data sekunder yang didapat dari penelitian di tahun 2023 di Jawa Barat dan Sulawesi Selatan. Data ini terdiri dari informasi pribadi penderita kasus mengenai jenis celah (variabel dependen) dan juga informasi nutrisi, lingkungan, dan juga orangtua penderita sebelum dan selama kehamilan. Distribusi jenis celah yang tidak normal, banyaknya faktor yang dipertimbangkan sebagai variabel independen, serta untuk mengetahui apa saja faktor yang berpengaruh secata signifikan digunakan Generalized Linear Model setelah diterapkan Analisis Komponen Utama Kategorikal(AKU-K) dan Bootstrapping. Bootstrapping digunakan dengan mempertimbangkan kondisi data yang imbalanced. 

**Skills**: data cleaning, data analysis, correlation matrices, hypothesis testing, data visualization.

**Teknologi**: Spreadsheet, SPSS, Rstudio, Minitab

**Hasil**: Proses dimulai dengan data cleaning menggunakan spreadsheet, kemudian dilakukan analisis komponen utama kategorikal adalah dengan menggunakan SPSS, hasilnya dilakukan bootstrapping menggunakan minitab, lalu Generalized Linear Model untuk melihat faktor yang berpengaruh secara signifikan menggunakan Rstudio. Hasilnya terdapat 4 variabel hasil leburan di wilayah Jawa Barat mencakup riwayat kesehatan ayah, riwayat kesehatan ibu, lingkungan ayah, dan lingkungan ibu. Sedangkan Sulawesi Selatan, berdasarkan hasil AKU-K terdapat 1 variabel hasil leburan yakni riwayat keguguran. Wilayah Jawa Barat memiliki variabel signifikan riwayat kesehatan ibu, masalah trimester pertama, rokok pasif ayah dan ibu, radiasi ayah dan ibu, olahraga ayah dan ibu, serta kafein ayah dan ibu. Wilayah Sulawesi Selatan memiliki variabel signifikan terhadap jenis celah diantaranya radiasi ibu, rokok pasif ibu, dan rokok pasif ayah. Kemudian pada data gabungan, variabel signifikan adalah wilayah, pemeriksaan kehamilan, masalah trimester pertama, dan beberapa faktor pola hidup orang tua. Sehingga, wilayah berpengaruh secara signifikan terhadap jenis celah.

<div style="border-radius:10px;overflow:hidden;border:1px solid #e0d5d5;margin-bottom:2rem;">

  <div style="background:linear-gradient(120deg,#4a0e0e,#7a1f1f);padding:1.25rem 1.5rem;">
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;margin-right:6px;">Python</span>
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;margin-right:6px;">SPC</span>
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;">EWMA</span>
    <h3 style="color:#fff;margin:10px 0 0;font-size:20px;">Pergeseran tingkat pengangguran pasca krisis finansial Asia</h3>
  </div>

  <div style="padding:1.25rem 1.5rem;background:#fff;">

    <div style="display:flex;gap:12px;margin-bottom:1.25rem;">
      <div style="flex:1;background:#f7f2f2;border-radius:8px;padding:12px;">
        <p style="font-size:12px;color:#6b6b6b;margin:0 0 4px;">Pergeseran naik</p>
        <p style="font-size:22px;font-weight:bold;color:#7a1f1f;margin:0;">53.7%</p>
      </div>
      <div style="flex:1;background:#f7f2f2;border-radius:8px;padding:12px;">
        <p style="font-size:12px;color:#6b6b6b;margin:0 0 4px;">Negara dianalisis</p>
        <p style="font-size:22px;font-weight:bold;color:#7a1f1f;margin:0;">41</p>
      </div>
      <div style="flex:1;background:#f7f2f2;border-radius:8px;padding:12px;">
        <p style="font-size:12px;color:#6b6b6b;margin:0 0 4px;">Stabil</p>
        <p style="font-size:22px;font-weight:bold;color:#7a1f1f;margin:0;">36.5%</p>
      </div>
    </div>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Insight utama</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Dari 41 negara Asia yang ditinjau, 53,7% mengalami pergeseran naik tingkat pengangguran pasca krisis finansial 1997-1998 — berbeda dari benua lain yang justru menunjukkan penurunan rerata dan median, menandakan efek krisis di Asia bersifat berkelanjutan.</p>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Problem</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Mendeteksi apakah krisis finansial Asia 1997-1998 meninggalkan pergeseran struktural pada tingkat pengangguran jangka panjang, dan seberapa stabil kondisi pengangguran pasca krisis tersebut.</p>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Approach</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Data 235 negara dari WorldBank (via Kaggle), periode 1991-2021, data training 1991-1995 untuk menetapkan nilai mu dan sigma, data testing 1996-2001 untuk melihat stabilisasi. Menerapkan bagan kendali Shewhart (Xbar-R/Xbar-S) dan EWMA — teknik Statistical Process Control yang lebih umum dipakai di manufaktur/QC, kombinasi yang jarang dieksplorasi di analisis data makroekonomi.</p>

    <img src="Mean%20Median%20Dunia.png" alt="Median dan Mean Tingkat Pengangguran di Seluruh Benua Pada 1991-2021" style="width:100%;border-radius:8px;margin-top:8px;">

  </div>
</div>

## Pendidikan
Institut Teknologi Bandung, Bandung :
Sarjana Matematika
2022 - 2026

## Kontak
* [LinkedIn: @AdindaFebrianti](https://linkedin.com/in/adinda-febrianti-370a44285)
* [Email: adndfebrianti26@gmail.com](mailto:adndfebrianti26@gmail.com)
