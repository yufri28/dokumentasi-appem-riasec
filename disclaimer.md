# 📘 Dokumentasi Sistem APPEM RIASEC — Panduan untuk Guru BK

> **APPEM RIASEC** (*Aplikasi Peminatan berbasis RIASEC*) adalah sistem berbasis web yang membantu sekolah dalam proses penentuan paket mata pelajaran (mapel) pilihan siswa secara objektif, berdasarkan data ilmiah — bukan sekadar preferensi atau pilihan subjektif siswa semata.

---

## 📌 Daftar Isi

1. [Apa itu APPEM RIASEC?](#1-apa-itu-appem-riasec)
2. [Mengapa Pilihan Siswa Bukan Satu-satunya Penentu?](#2-mengapa-pilihan-siswa-bukan-satu-satunya-penentu)
3. [Alur Penentuan Rekomendasi Sistem](#3-alur-penentuan-rekomendasi-sistem)
4. [Penjelasan Setiap Tahap](#4-penjelasan-setiap-tahap)
5. [Peran Guru BK dalam Sistem Ini](#5-peran-guru-bk-dalam-sistem-ini)
6. [Fitur Analisa Kesesuaian Paket](#6-fitur-analisa-kesesuaian-paket)
7. [Pertanyaan yang Sering Ditanyakan (FAQ)](#7-pertanyaan-yang-sering-ditanyakan-faq)

---

## 1. Apa itu APPEM RIASEC?

**APPEM RIASEC** adalah sistem pendukung keputusan peminatan yang dirancang untuk membantu Guru BK dan pihak sekolah dalam:

- **Mengidentifikasi** tipe kepribadian dan minat dominan setiap siswa melalui tes RIASEC yang terstandarisasi.
- **Menganalisis** kesesuaian antara minat siswa, cita-cita, serta kemampuan akademiknya.
- **Menghasilkan rekomendasi** paket mata pelajaran yang paling sesuai dengan **potensi nyata** siswa, bukan semata pilihan atau keinginan sesaat.
- **Membantu Guru BK** mendeteksi lebih awal siswa yang mungkin memilih paket mapel yang tidak sesuai dengan potensinya, sehingga dapat dilakukan intervensi bimbingan sebelum terlambat.

> 💡 **Prinsip utama:** APPEM RIASEC bukan sistem pemilihan paket secara mandiri oleh siswa. Sistem ini adalah **alat bantu analisis berbasis data** yang menempatkan Guru BK sebagai pengambil keputusan akhir.

---

## 2. Mengapa Pilihan Siswa Bukan Satu-satunya Penentu?

Ini adalah poin penting yang **sering disalahpahami**.

Banyak yang mengira bahwa sistem ini akan langsung merekomendasikan paket yang sudah dipilih oleh siswa. **Anggapan ini keliru.**

### ❌ Kesalahpahaman Umum

> *"Sistem ini akan memvalidasi dan meneruskan apa yang sudah siswa pilih."*

### ✅ Yang Sebenarnya Terjadi

> *Pilihan siswa hanyalah **satu data titik** yang dicatat sistem. Rekomendasi akhir ditentukan berdasarkan **analisis tiga dimensi**: tipe kepribadian (RIASEC), kesesuaian dengan cita-cita, dan kekuatan akademik (nilai raport).*

### Mengapa Demikian?

Dalam praktik nyata, siswa seringkali memilih paket mapel karena alasan yang **tidak selalu mencerminkan potensi sesungguhnya**, seperti:

| Faktor Subjektif | Risiko |
|---|---|
| Mengikuti pilihan teman | Paket tidak sesuai minat/kemampuan |
| Terpengaruh tren atau gengsi | Motivasi belajar rendah di kemudian hari |
| Tekanan dari orang tua | Konflik internal, performa akademik menurun |
| Kurangnya informasi tentang paket | Siswa tidak tahu apa yang benar-benar ia minati |
| Pilihan impulsif/asal pilih | Penyesalan di tengah jalan |

APPEM RIASEC dirancang untuk **memfilter faktor-faktor subjektif ini** dengan menggunakan pendekatan ilmiah yang bersumber dari data yang tidak bisa dibuat-buat: hasil tes psikometrik RIASEC dan nilai akademik semester.

---

## 3. Alur Penentuan Rekomendasi Sistem

Berikut adalah alur kerja sistem APPEM RIASEC secara menyeluruh:

```
┌─────────────────────────────────────────────────────────────────────┐
│                   ALUR SISTEM APPEM RIASEC                          │
└─────────────────────────────────────────────────────────────────────┘

 [SISWA]                          [SISTEM]                  [GURU BK]
    │                                 │                          │
    │  1. Mengerjakan Tes RIASEC       │                          │
    │ ──────────────────────────────► │                          │
    │                                 │                          │
    │  2. Memilih Cita-cita            │                          │
    │ ──────────────────────────────► │                          │
    │                                 │                          │
    │  3. Memilih Paket Mapel Pilihan  │                          │
    │    (data minat, BUKAN penentu)  │                          │
    │ ──────────────────────────────► │                          │
    │                                 │                          │
    │                [TAHAP 1]        │                          │
    │                Sistem mencocokkan hasil RIASEC              │
    │                dengan daftar cita-cita siswa                │
    │                (menghasilkan skor kecocokan #1)             │
    │                                 │                          │
    │                [TAHAP 2]        │                          │
    │                Sistem mencocokkan hasil RIASEC              │
    │                dengan setiap paket mapel yang tersedia      │
    │                di sekolah (menghasilkan skor kecocokan #2)  │
    │                                 │                          │
    │                [TAHAP 3]        │                          │
    │                Sistem mengintegrasikan nilai akademik       │
    │                (raport semester) sebagai faktor penentu     │
    │                akhir — paket dengan skor tertinggi dari     │
    │                kombinasi ketiga dimensi menjadi hasil       │
    │                rekomendasi final                            │
    │                                 │                          │
    │                                 │  4. Menerima Hasil       │
    │                                 │     Rekomendasi Final    │
    │                                 │ ────────────────────────►│
    │                                 │                          │
    │                                 │  5. Guru BK menganalisa  │
    │                                 │     dan menentukan       │
    │                                 │     Finalisasi Paket     │
    │                                 │ ────────────────────────►│
    │                                 │                          │
    │  6. Menerima Paket Final         │                          │
    │ ◄─────────────────────────────────────────────────────────  │
    │                                 │                          │
```

---

## 4. Penjelasan Setiap Tahap

### 🔵 Tahap 1 — Pencocokan RIASEC vs Cita-cita

Pada tahap ini, sistem membaca hasil tes RIASEC siswa yang berisi enam dimensi kepribadian:

| Kode | Tipe | Karakteristik |
|------|------|--------------|
| **R** | Realistic | Praktis, suka bekerja dengan tangan, teknik, alam |
| **I** | Investigative | Analitis, suka meneliti, berpikir logis |
| **A** | Artistic | Kreatif, ekspresif, imajinatif |
| **S** | Social | Empatik, suka membantu orang lain, komunikatif |
| **E** | Enterprising | Kepemimpinan, persuasif, berorientasi bisnis |
| **C** | Conventional | Terstruktur, teliti, suka pekerjaan administratif |

Sistem kemudian **mencocokkan tiga kode teratas (Top 3)** dengan basis data cita-cita (profesi) yang telah dipetakan ke tipe RIASEC masing-masing. Misalnya, siswa dengan kode **IAR** akan sangat cocok dengan cita-cita seperti *ilmuwan*, *dokter*, atau *insinyur penelitian*.

> **Hasil Tahap 1:** Skor kecocokan antara kepribadian siswa dan arah karier yang dicita-citakannya.

---

### 🟢 Tahap 2 — Pencocokan RIASEC vs Paket Mapel

Setiap paket mapel yang tersedia di sekolah telah dipetakan ke satu atau lebih tipe RIASEC yang relevan. Pada tahap ini, sistem menghitung **seberapa besar kesesuaian** antara profil RIASEC siswa dengan karakteristik setiap paket mapel.

Contoh pemetaan:

| Paket Mapel | RIASEC yang Cocok |
|---|---|
| MIPA / Ilmu Alam | I, R |
| IPS / Ilmu Sosial | S, E |
| Bahasa & Sastra | A, S |
| Teknologi / Informatika | I, R, C |
| Seni / Vokasi Kreatif | A, R |

Sistem akan memberikan **nilai skor** untuk setiap paket berdasarkan kecocokan ini.

> **Hasil Tahap 2:** Rangking paket mapel dari yang paling cocok hingga paling tidak cocok berdasarkan kepribadian RIASEC siswa.

---

### 🟡 Tahap 3 — Integrasi Nilai Akademik (Raport)

Tahap ini adalah **lapisan verifikasi objektif terakhir**. Sistem membaca nilai raport semester siswa — khususnya pada mata pelajaran yang relevan dengan masing-masing paket mapel.

Logikanya sederhana: **kemampuan akademik yang sudah terbukti** adalah indikator yang lebih dapat diandalkan dibanding niat atau pilihan sesaat. Seorang siswa dengan nilai Biologi dan Kimia yang tinggi secara konsisten memiliki fondasi yang kuat untuk mengambil paket MIPA, terlepas dari apakah ia "merasa" ingin memilihnya atau tidak.

> **Hasil Tahap 3:** Rekomendasi paket mapel final yang merupakan **irisan terbaik** antara minat (RIASEC), arah karier (cita-cita), dan kemampuan akademik (nilai raport).

---

### 🏁 Hasil Akhir — Finalisasi oleh Guru BK

Rekomendasi dari sistem **bukan keputusan mutlak**. Rekomendasi ini diserahkan kepada **Guru BK** sebagai bahan pertimbangan utama. Guru BK tetap memiliki **otoritas penuh** untuk:

- Menerima rekomendasi sistem secara langsung.
- Melakukan penyesuaian berdasarkan konteks tambahan yang hanya diketahui Guru BK (kondisi keluarga, psikologis siswa, dll.).
- Memindahkan siswa ke paket lain jika ada pertimbangan khusus melalui fitur **Pindah Paket**.

---

## 5. Peran Guru BK dalam Sistem Ini

Guru BK bukan sekadar operator sistem. Dalam APPEM RIASEC, Guru BK adalah **pengambil keputusan utama** yang didukung oleh data yang kaya dari sistem.

### Yang Dilakukan Sistem (Otomatis)
- ✅ Mengolah hasil tes RIASEC secara objektif
- ✅ Mencocokkan data dengan basis pengetahuan yang terstandarisasi
- ✅ Menghasilkan rekomendasi berbasis multi-dimensi
- ✅ Mencatat pilihan siswa sebagai data perbandingan
- ✅ Menandai ketidaksesuaian antara pilihan siswa dan rekomendasi

### Yang Dilakukan Guru BK (Keputusan Manusia)
- 🎯 Membaca dan menginterpretasikan rekomendasi sistem
- 🎯 Melakukan konsultasi jika ada ketidaksesuaian
- 🎯 Mempertimbangkan faktor non-akademik yang tidak tertangkap sistem
- 🎯 Mengesahkan finalisasi paket mapel siswa
- 🎯 Memberikan bimbingan lanjutan setelah penetapan paket

---

## 6. Fitur Analisa Kesesuaian Paket

Fitur ini secara khusus dirancang untuk **membantu Guru BK mendeteksi potensi masalah** sebelum siswa menyesal di kemudian hari.

### Cara Membaca Analisa

| Indikator | Artinya |
|---|---|
| ✅ **Sesuai** | Paket final yang ditetapkan sistem **ada dalam daftar pilihan siswa**. Ini bukan berarti sistem memvalidasi pilihan siswa — ini berarti secara kebetulan pilihan siswa *searah* dengan rekomendasi berbasis data. |
| ⚠️ **Tidak Sesuai** | Paket final yang direkomendasikan sistem **berbeda dari semua pilihan siswa**. Ini adalah **sinyal peringatan** bahwa siswa mungkin memilih berdasarkan alasan subjektif yang tidak mencerminkan potensinya. |

### Apa yang Harus Dilakukan Guru BK saat Status "Tidak Sesuai"?

Status **Tidak Sesuai** bukan berarti siswa salah atau sistem salah. Status ini adalah **undangan untuk berdialog**. Guru BK perlu:

1. **Mendengarkan** alasan siswa memilih paket tersebut.
2. **Menjelaskan** mengapa sistem merekomendasikan paket yang berbeda — gunakan data RIASEC dan nilai raport yang tersedia di modal analisa.
3. **Mengeksplorasi** apakah ada faktor luar (tekanan teman, orang tua, informasi yang salah) yang mempengaruhi pilihan siswa.
4. **Mendampingi** siswa untuk memahami potensi dirinya secara lebih objektif.
5. **Memutuskan** secara bijaksana apakah finalisasi dipertahankan atau disesuaikan.

---

## 7. Pertanyaan yang Sering Ditanyakan (FAQ)

### ❓ "Apakah sistem ini menentukan paket berdasarkan pilihan siswa?"

**Tidak.** Pilihan siswa hanya dicatat sebagai referensi. Rekomendasi dihitung dari RIASEC + Cita-cita + Nilai Raport. Pilihan siswa digunakan di tahap akhir sebagai **pembanding**, bukan sebagai input rekomendasi.

---

### ❓ "Jika siswa memilih Paket A dan sistem merekomendasikan Paket B, siapa yang benar?"

Keduanya belum tentu salah. Sistem berbicara dari sudut pandang **data objektif**. Siswa berbicara dari sudut pandang **perasaan dan persepsinya**. Guru BK bertugas menjembatani keduanya melalui proses konsultasi.

---

### ❓ "Apakah Guru BK wajib mengikuti rekomendasi sistem?"

**Tidak wajib.** Rekomendasi sistem adalah **saran berbasis data**, bukan keputusan final. Guru BK tetap pemegang otoritas penuh atas keputusan peminatan.

---

### ❓ "Mengapa siswa yang memilih paket yang 'populer' sering tidak sesuai dengan rekomendasinya?"

Karena paket populer cenderung dipilih karena faktor sosial, bukan karena kecocokan dengan kepribadian. APPEM RIASEC tidak mengenal konsep "populer" — ia hanya mengenal data RIASEC dan nilai akademik.

---

### ❓ "Apa yang terjadi jika siswa belum mengerjakan tes RIASEC?"

Tanpa data RIASEC, sistem tidak dapat menghasilkan rekomendasi yang akurat. Guru BK disarankan untuk memastikan **seluruh siswa menyelesaikan tes RIASEC** sebelum proses peminatan dimulai.

---

### ❓ "Apakah nilai raport yang lebih tinggi selalu menghasilkan rekomendasi yang lebih baik?"

Tidak selalu. Nilai raport digunakan sebagai **faktor penguat**, bukan faktor tunggal. Seorang siswa dengan nilai Fisika tinggi namun profil RIASEC yang sangat Artistic mungkin justru lebih tepat diarahkan ke paket yang berbeda — dan ini adalah peran Guru BK untuk mendiskusikannya.

---

## 📎 Catatan Penting untuk Implementasi

> [!IMPORTANT]
> Sistem ini adalah **alat bantu keputusan (Decision Support System)**, bukan sistem yang menggantikan peran dan penilaian profesional Guru BK. Data yang dihasilkan sistem harus selalu diinterpretasikan dalam konteks pengetahuan Guru BK tentang kondisi nyata setiap siswa.

> [!NOTE]
> Untuk hasil rekomendasi yang optimal, pastikan tiga kondisi ini terpenuhi sebelum proses peminatan:
> 1. Siswa telah **menyelesaikan tes RIASEC** secara mandiri dan jujur.
> 2. Data **nilai raport** siswa telah diimport ke dalam sistem.
> 3. **Paket mapel** yang tersedia di sekolah sudah didaftarkan dan dipetakan dengan benar oleh Administrator.

---

*Dokumentasi ini dibuat untuk membantu seluruh pengguna sistem — khususnya Guru BK — dalam memahami filosofi, alur kerja, dan cara penggunaan APPEM RIASEC secara tepat dan efektif.*
