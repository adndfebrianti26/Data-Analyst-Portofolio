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

<div style="border-radius:10px;overflow:hidden;border:1px solid #e0d5d5;margin-bottom:2rem;">

  <div style="background:linear-gradient(120deg,#4a0e0e,#7a1f1f);padding:1.25rem 1.5rem;">
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;margin-right:6px;">SPSS</span>
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;margin-right:6px;">RStudio</span>
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;margin-right:6px;">Minitab</span>
    <span style="display:inline-block;font-size:13px;padding:4px 12px;border-radius:20px;background:rgba(255,255,255,0.15);color:#fff;">CATPCA</span>
    <h3 style="color:#fff;margin:10px 0 0;font-size:20px;">Faktor penyebab celah bibir dan langit-langit</h3>
  </div>

  <div style="padding:1.25rem 1.5rem;background:#fff;">

    <div style="display:flex;gap:12px;margin-bottom:1.25rem;">
      <div style="flex:1;background:#f7f2f2;border-radius:8px;padding:12px;">
        <p style="font-size:12px;color:#6b6b6b;margin:0 0 4px;">Total sampel</p>
        <p style="font-size:22px;font-weight:bold;color:#7a1f1f;margin:0;">133</p>
      </div>
      <div style="flex:1;background:#f7f2f2;border-radius:8px;padding:12px;">
        <p style="font-size:12px;color:#6b6b6b;margin:0 0 4px;">Variabel awal</p>
        <p style="font-size:22px;font-weight:bold;color:#7a1f1f;margin:0;">28</p>
      </div>
      <div style="flex:1;background:#f7f2f2;border-radius:8px;padding:12px;">
        <p style="font-size:12px;color:#6b6b6b;margin:0 0 4px;">Variabel signifikan</p>
        <p style="font-size:22px;font-weight:bold;color:#7a1f1f;margin:0;">10</p>
      </div>
    </div>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Insight utama</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Pola faktor risiko celah bibir dan langit-langit berbeda signifikan antar wilayah — paparan radiasi dan rokok mendominasi di Jawa Barat, sementara riwayat keguguran dan pendidikan orang tua lebih berpengaruh di Sulawesi Selatan. Perbedaan ini membuktikan wilayah bukan sekadar variabel kontrol, tapi faktor signifikan tersendiri terhadap jenis celah.</p>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Masalah</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Mengidentifikasi dimensi variabel penyebab kasus celah bibir dan langit-langit, menentukan faktor yang berpengaruh secara signifikan di Jawa Barat dan Sulawesi Selatan, dan mengetahui apakah perbedaan wilayah turut memengaruhi faktor penyebabnya.</p>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Pendekatan</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Data sekunder dari penelitian 2023 di Jawa Barat dan Sulawesi Selatan, mencakup faktor genetik, orang tua, dan lingkungan. Karena banyaknya faktor yang saling berkorelasi (rawan multikolinearitas) dan jenis celah yang tidak terdistribusi normal, digunakan Analisis Komponen Utama Kategorikal (CATPCA) untuk reduksi dimensi, dilanjutkan Generalized Linear Model (distribusi binomial, fungsi logit) dengan bootstrapping untuk menangani data yang tidak seimbang.</p>

    <img src="Hasil%20Jawa%20Barat%20Korelasi.png" alt="Heatmap korelasi antar variabel penyebab celah bibir dan langit-langit di Jawa Barat" style="width:100%;border-radius:8px;margin-bottom:16px;">

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Hasil reduksi dimensi</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 12px;">Di Jawa Barat, 21 variabel awal tereduksi menjadi 2 dimensi utama yang menjelaskan 77% variansi — variabel dengan loading tertinggi adalah paparan radiasi ibu, sementara riwayat kesehatan dan lingkungan orang tua melebur menjadi dua variabel gabungan baru.</p>
    <img src="Component%20Loadings%20Jawa%20Barat.png" alt="Component loadings plot hasil CATPCA di Jawa Barat" style="width:100%;border-radius:8px;">

  </div>
</div>

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

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Masalah</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Mendeteksi apakah krisis finansial Asia 1997-1998 meninggalkan pergeseran struktural pada tingkat pengangguran jangka panjang, dan seberapa stabil kondisi pengangguran pasca krisis tersebut.</p>

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Pendekatan</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 16px;">Data 235 negara dari WorldBank (via Kaggle), periode 1991-2021, data training 1991-1995 untuk menetapkan nilai mu dan sigma, data testing 1996-2001 untuk melihat stabilisasi. Menerapkan bagan kendali Shewhart (Xbar-R/Xbar-S) dan EWMA — teknik Statistical Process Control yang lebih umum dipakai di manufaktur/QC, kombinasi yang jarang dieksplorasi di analisis data makroekonomi.</p>

    <img src="Mean%20Median%20Dunia.png" alt="Median dan Mean Tingkat Pengangguran di Seluruh Benua Pada 1991-2021" style="width:100%;border-radius:8px;margin-bottom:16px;">

    <p style="font-size:14px;font-weight:bold;color:#7a1f1f;margin:0 0 6px;">Contoh pergeseran ekstrem: Yaman</p>
    <p style="font-size:14px;color:#333;line-height:1.6;margin:0 0 12px;">Yaman menunjukkan tingkat pengangguran naik konsisten setiap tahun hingga melewati batas kendali (UCL) — salah satu kasus pergeseran paling jelas dari seluruh negara yang dianalisis.</p>
    <img src="Chart%20Yaman.png" alt="Bagan kendali Shewhart dan EWMA untuk Yaman" style="width:100%;border-radius:8px;">

  </div>
</div>

## Pendidikan
Institut Teknologi Bandung, Bandung :
Sarjana Matematika
2022 - 2026

## Kontak
* [LinkedIn: @AdindaFebrianti](https://linkedin.com/in/adinda-febrianti-370a44285)
* [Email: adndfebrianti26@gmail.com](mailto:adndfebrianti26@gmail.com)
