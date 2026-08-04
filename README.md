# 📘 Dokumentasi Sistem APPEM
## Panduan Penggunaan untuk Guru BK

> **APPEM** — *Aplikasi Pemetaan Minat dan Karier Siswa*
> Sistem berbasis web yang dirancang untuk membantu Guru Bimbingan dan Konseling (BK) dalam mengelola proses tes RIASEC siswa, menganalisis hasilnya, dan memfasilitasi penempatan siswa ke paket mata pelajaran yang sesuai.

---

## 📋 Daftar Isi

1. [Pendahuluan](#1-pendahuluan)
2. [Login & Keamanan Akun](#2-login--keamanan-akun)
3. [Dashboard Guru BK](#3-dashboard-guru-bk)
4. [Profil Sekolah](#4-profil-sekolah)
5. [Manajemen Data Siswa](#5-manajemen-data-siswa)
6. [Manajemen Mata Pelajaran (Mapel)](#6-manajemen-mata-pelajaran-mapel)
7. [Manajemen Paket Mapel](#7-manajemen-paket-mapel)
8. [Manajemen Bidang Cita-cita](#8-manajemen-bidang-cita-cita)
9. [Manajemen Nilai Siswa](#9-manajemen-nilai-siswa)
10. [Progres Siswa](#10-progres-siswa)
11. [Rekapitulasi & Finalisasi Hasil](#11-rekapitulasi--finalisasi-hasil)
12. [Alur Kerja Lengkap (End-to-End)](#12-alur-kerja-lengkap-end-to-end)
13. [Tips & Troubleshooting](#13-tips--troubleshooting)

---

## 1. Pendahuluan

### Apa itu APPEM?

APPEM adalah sistem digital yang membantu Guru BK untuk:

- **Mengelola data siswa** secara terpusat
- **Memantau progres** pengerjaan tes RIASEC setiap siswa
- **Menganalisis hasil** tes minat RIASEC secara otomatis
- **Mencocokkan** hasil RIASEC siswa dengan pilihan paket mata pelajaran
- **Mempublikasikan hasil akhir** penempatan paket kepada siswa

### Alur Proses Siswa di APPEM

```
[Siswa Login] → [Tes RIASEC 42 Soal] → [Pilih Bidang Cita-cita] → [Pilih 3 Prioritas Paket Mapel]
                                                                              ↓
[Siswa Lihat Hasil Akhir] ← [Guru BK Publikasikan] ← [Guru BK Finalisasi Paket]
```

### Hak Akses Guru BK

Sebagai Guru BK, Anda memiliki akses penuh untuk:
- Mengelola data sekolah, siswa, dan nilai
- Memantau dan menganalisis progres siswa
- Menentukan dan memfinalisasi penempatan paket mapel
- Mempublikasikan hasil akhir kepada siswa

> [!NOTE]
> Akun Guru BK dibuat oleh **Administrator** sistem. Anda tidak dapat mendaftar sendiri. Hubungi admin jika belum memiliki akun.

---

## 2. Login & Keamanan Akun

### Cara Login

1. Buka aplikasi APPEM di browser
2. Masukkan **Username** (NIP atau nama pengguna yang diberikan admin)
3. Masukkan **Password**
4. Klik tombol **Login**

> [!IMPORTANT]
> Jangan bagikan username dan password Anda kepada siapapun, termasuk siswa. Setiap tindakan di sistem tercatat atas nama akun Anda.

### Lupa Password?

Sistem APPEM sudah menyediakan fitur **Reset Password** secara mandiri.

1. Klik tautan **Lupa Password?** pada halaman login
2. Masukkan **alamat email** yang terdaftar pada akun Anda
3. Cek kotak masuk email Anda dan ikuti tautan reset yang dikirimkan
4. Buat password baru dan login kembali

> [!IMPORTANT]
> Pastikan alamat email yang terdaftar di akun Anda **masih aktif dan dapat diakses**. Jika email tidak aktif atau tidak terdaftar, hubungi Administrator sistem untuk bantuan lebih lanjut.

---

## 3. Dashboard Guru BK

Setelah login, Anda akan langsung diarahkan ke **Dashboard Guru BK**.

### Informasi yang Ditampilkan

| Kartu Informasi | Keterangan |
|---|---|
| 👥 **Jumlah Siswa** | Total siswa yang terdaftar di sekolah Anda pada tahun yang dipilih |
| 📌 **Progress Siswa** | Ringkasan tahapan pengerjaan siswa (0/3, 1/3, 2/3, 3/3) |
| 📢 **Sudah Diumumkan** | Berapa siswa yang hasil akhirnya sudah dipublikasikan |
| 📨 **Receive Results** | Jumlah siswa yang masuk ke paket tampung sementara |
| 🗂 **Final Results** | Jumlah siswa yang sudah mendapat paket final |
| 📚 **Data Umum** | Jumlah Paket Mapel, Bidang Cita-cita, dan Mapel yang ada |

### Grafik Progress Siswa

Di bagian bawah dashboard terdapat **grafik batang** yang memvisualisasikan distribusi progress siswa:

- 🔴 **Belum Mulai (0/3)** — Siswa belum mengerjakan apapun
- 🟠 **Sedang Proses (1/3)** — Siswa sudah selesai tes RIASEC
- 🟡 **Hampir Selesai (2/3)** — Siswa sudah memilih cita-cita
- 🟢 **Selesai (3/3)** — Siswa sudah memilih 3 prioritas paket mapel

### Filter Tahun

Gunakan dropdown **Tahun** di pojok kanan atas dashboard untuk melihat data per tahun akademik.

---

## 4. Profil Sekolah

> [!IMPORTANT]
> **Wajib dilengkapi sebelum menggunakan fitur lainnya.** Jika profil sekolah belum diisi, sebagian besar fitur tidak dapat diakses.

### Cara Mengisi Profil Sekolah

1. Klik menu **Profil Sekolah** pada sidebar
2. Isi formulir berikut:
   - **NPSN** — Nomor Pokok Sekolah Nasional
   - **Nama Sekolah** — Nama lengkap sekolah
   - **Alamat** — Alamat lengkap sekolah
3. Klik **Simpan Perubahan**
4. Muncul notifikasi hijau ✅ jika berhasil disimpan

---

## 5. Manajemen Data Siswa

Menu ini digunakan untuk mengelola data identitas siswa yang terdaftar di sistem.

### Melihat Daftar Siswa

1. Klik menu **Data Siswa** pada sidebar
2. Daftar siswa akan tampil dalam bentuk tabel
3. Gunakan **kolom pencarian** untuk mencari siswa berdasarkan nama atau NISN
4. Gunakan **filter tahun** untuk menyaring data per tahun

### Menambah Siswa Secara Manual

1. Klik tombol **➕ Tambah Siswa**
2. Isi data:
   - Nama Siswa
   - NISN (Nomor Induk Siswa Nasional)
   - Jenis Kelamin
   - Tanggal Lahir
3. Klik **Simpan**

> [!TIP]
> Cara yang **lebih efisien** adalah mengimpor data siswa melalui menu **Nilai Siswa** menggunakan file Excel. Akun siswa akan otomatis dibuat bersamaan dengan data nilai.

### Mengedit Data Siswa

1. Temukan siswa yang ingin diedit
2. Klik tombol **✏️ Edit** di kolom Aksi
3. Ubah data yang diperlukan
4. Klik **Simpan**

### Menghapus Data Siswa

1. Klik tombol **🗑️ Hapus** di kolom Aksi
2. Konfirmasi penghapusan pada dialog yang muncul

> [!WARNING]
> Menghapus data siswa akan menghapus seluruh riwayat tes, nilai, dan hasil yang terkait dengan siswa tersebut. Tindakan ini **tidak dapat dibatalkan**.

---

## 6. Manajemen Mata Pelajaran (Mapel)

Menu ini digunakan untuk mengelola daftar mata pelajaran yang digunakan dalam sistem.

### Melihat Daftar Mapel

1. Klik menu **Mata Pelajaran** pada sidebar
2. Daftar mapel tampil dalam tabel

### Menambah Mapel Baru

1. Klik tombol **➕ Tambah Mapel**
2. Isi nama mata pelajaran
3. Klik **Simpan**

> [!NOTE]
> Data mata pelajaran digunakan bersama antar sekolah. Sebelum menambahkan, pastikan mapel yang Anda maksud belum ada dalam daftar untuk menghindari duplikasi.

### Mengedit & Menghapus Mapel

Gunakan tombol **✏️ Edit** atau **🗑️ Hapus** pada baris data yang ingin diubah.

> [!CAUTION]
> Anda hanya dapat menghapus mapel yang **Anda sendiri yang menginput**. Mapel yang sudah ada sebelumnya (diinput oleh sekolah lain atau admin) hanya bisa dihapus oleh Administrator.

---

## 7. Manajemen Paket Mapel

Paket Mapel adalah kumpulan mata pelajaran yang dikelompokkan menjadi satu paket kelas/penjurusan. Siswa akan ditempatkan ke salah satu paket ini berdasarkan hasil analisis APPEM.

### Melihat Daftar Paket Mapel

1. Klik menu **Paket Mapel** pada sidebar
2. Daftar paket tampil lengkap dengan informasi:
   - Nama Paket
   - Daftar mapel dalam paket
   - Kapasitas (daya tampung maksimal)
   - Sisa kapasitas tersedia

### Menambah Paket Mapel Baru

1. Klik tombol **➕ Tambah Paket**
2. Isi formulir:
   - **Nama Paket** (contoh: IPA, IPS, Bahasa, Rekayasa Perangkat Lunak)
   - **Kapasitas** — jumlah maksimal siswa yang bisa masuk paket ini
   - **Mapel** — pilih mata pelajaran yang termasuk dalam paket ini
3. Klik **Simpan**

### Mengatur Pemetaan Mapel ke Paket

Gunakan fitur **Set Mapel** untuk mengonfigurasi mata pelajaran mana saja yang masuk ke dalam suatu paket.

> [!TIP]
> Isi **kapasitas** paket dengan cermat. Sistem akan menggunakan informasi ini untuk menentukan apakah paket masih memiliki sisa tempat saat finalisasi berlangsung.

---

## 8. Manajemen Bidang Cita-cita

Bidang cita-cita adalah kategori karier/profesi yang tersedia untuk dipilih siswa setelah menyelesaikan tes RIASEC. Setiap cita-cita terhubung dengan mapel-mapel pendukungnya.

### Melihat Daftar Cita-cita

1. Klik menu **Bidang Cita-cita** pada sidebar
2. Daftar bidang cita-cita tampil beserta kategorinya

### Menambah Bidang Cita-cita

1. Klik tombol **➕ Tambah Cita-cita**
2. Isi nama bidang cita-cita dan kategorinya
3. Klik **Simpan**

> [!NOTE]
> Data bidang cita-cita juga digunakan bersama antar sekolah. Periksa daftar yang ada sebelum menambahkan baru.

### Mengatur Pemetaan Cita-cita ke Mapel

Gunakan fitur **Set Mapel** pada setiap bidang cita-cita untuk menentukan mata pelajaran pendukung dari bidang tersebut.

---

## 9. Manajemen Nilai Siswa

Menu ini untuk mengelola data nilai rapor siswa, yang digunakan sebagai salah satu bahan analisis APPEM.

### Melihat Daftar Nilai

1. Klik menu **Nilai Siswa** pada sidebar
2. Tabel nilai tampil dengan kolom: Nama Mapel, Total Nilai (Semester 1 & 2), Nama Siswa
3. Gunakan **filter tahun** atau **rentang tanggal** untuk menyaring data
4. Gunakan **kolom pencarian** untuk mencari berdasarkan nama siswa atau mapel

### Import Data Nilai via Excel (Direkomendasikan)

Cara tercepat memasukkan data nilai banyak siswa sekaligus:

#### Langkah 1: Download Template Excel

1. Klik tombol **Template** (ikon biru)
2. Pada modal yang muncul:
   - Isi **Jumlah Siswa** yang akan dimasukkan
   - Centang **Mata Pelajaran** yang ingin diisikan nilainya
3. Klik **Download** — file Excel siap diisi akan terunduh

#### Langkah 2: Isi Template Excel

Isi file Excel yang terunduh dengan data:
- NISN siswa
- Nama siswa
- Jenis kelamin
- Tanggal lahir
- Nilai setiap mapel yang dipilih

> [!IMPORTANT]
> Pastikan format NISN diisi dengan benar. Jika siswa belum terdaftar, sistem akan **otomatis membuat akun baru** untuk siswa tersebut berdasarkan data NISN, Nama, Jenis Kelamin, dan Tanggal Lahir.

#### Langkah 3: Upload File Excel

1. Klik **Pilih File Excel** dan pilih file yang sudah diisi
2. Klik tombol **🚀 Import**
3. Progress bar akan menunjukkan proses upload
4. Tunggu hingga status berubah menjadi ✅ **Import selesai!**
5. Halaman akan otomatis refresh menampilkan data terbaru

### Menambah Nilai Secara Manual

1. Klik tombol **➕ Tambah Nilai**
2. Pilih siswa dari daftar
3. Isi nilai untuk setiap mata pelajaran
4. Klik **Simpan**

### Mengedit & Menghapus Nilai

Gunakan tombol **✏️ Edit** atau **🗑️ Hapus** pada baris nilai yang ingin diubah.

---

## 10. Progres Siswa

Menu ini memungkinkan Guru BK memantau sejauh mana setiap siswa telah menyelesaikan tahapan di APPEM.

### Indikator Progress

| Progress | Artinya |
|---|---|
| **0/3** 🔴 | Siswa belum mengerjakan apapun |
| **1/3** 🟠 | Siswa sudah selesai tes RIASEC |
| **2/3** 🟡 | Siswa sudah memilih bidang cita-cita |
| **3/3** 🟢 | Siswa sudah memilih 3 prioritas paket mapel |

### Melihat Progres Siswa

1. Klik menu **Progres Siswa** pada sidebar
2. Tabel siswa tampil beserta progress bar visual
3. Filter menggunakan:
   - **Kolom pencarian** — cari nama atau NISN
   - **Dropdown progress** — filter berdasarkan tahap (0/3 s/d 3/3)
   - **Dropdown tahun** — filter per tahun akademik
   - **Rentang tanggal** — filter berdasarkan tanggal pendaftaran

### Melihat Detail Progress Siswa

Siswa yang sudah mencapai progress **3/3 (Selesai)** dapat dilihat detailnya:

1. Klik tombol **🔍 Lihat Detail** pada baris siswa
2. Halaman detail menampilkan:
   - Hasil tes RIASEC (Top 3 tipe kepribadian)
   - Bidang cita-cita yang dipilih
   - 3 prioritas paket mapel yang dipilih siswa
   - Nilai rapor siswa per mapel

> [!NOTE]
> Tombol **Lihat Detail** hanya aktif untuk siswa yang sudah menyelesaikan semua tahapan (3/3). Siswa yang belum selesai akan menampilkan tombol 🚫 Belum Lengkap.

### Finalisasi Progres

Setelah semua atau sebagian besar siswa menyelesaikan tahapan mereka, Guru BK dapat melakukan **Finalisasi Progres**:

1. Klik tombol **Finalisasi Progres** (tombol hijau di bagian atas)
2. Baca konfirmasi yang muncul dengan cermat
3. Klik **Ya, finalisasi!** untuk melanjutkan

> [!WARNING]
> Finalisasi progres akan memproses data seluruh siswa untuk menentukan penempatan paket. Pastikan **semua data nilai dan paket mapel sudah benar** sebelum melakukan finalisasi.

---

## 11. Rekapitulasi & Finalisasi Hasil

Menu ini menampilkan hasil akhir penempatan siswa ke paket mapel setelah finalisasi dilakukan.

### 11.1 Hasil Final (Final Results)

Menampilkan siswa yang telah berhasil mendapatkan paket mapel final.

#### Mengakses Halaman Final Results

1. Klik menu **Rekapitulasi** → **Hasil Final** pada sidebar

#### Filter & Pencarian

Gunakan opsi filter berikut untuk menyaring data:

| Filter | Fungsi |
|---|---|
| 🔍 **Pencarian** | Cari berdasarkan nama atau NISN siswa |
| 📦 **Paket** | Filter berdasarkan paket mapel tertentu |
| 📅 **Tahun** | Filter berdasarkan tahun akademik |
| 📆 **Rentang Tanggal** | Filter berdasarkan tanggal finalisasi |

#### Kolom Analisis

Untuk setiap siswa, sistem menampilkan:

- **Nama & NISN** siswa
- **Paket Final** yang ditetapkan sistem
- **Status Pencocokan**:
  - ✅ **Sesuai** — Paket final ada dalam daftar pilihan siswa
  - ❌ **Tidak Sesuai** — Paket final berbeda dari pilihan siswa (perlu konsultasi lanjutan)
- **Status Pengumuman** — apakah hasil sudah dipublikasikan ke siswa

#### Memindahkan Siswa ke Paket Lain

Jika ada siswa yang perlu dipindahkan ke paket yang berbeda:

1. Klik baris siswa yang ingin dipindah
2. Pilih paket tujuan dari daftar yang tersedia
3. Konfirmasi pemindahan

> [!TIP]
> Gunakan fitur pindah paket untuk menyeimbangkan jumlah siswa di setiap paket, terutama jika ada paket yang kelebihan atau kekurangan peserta.

#### Mengumumkan Hasil ke Siswa

Untuk mempublikasikan hasil akhir agar bisa dilihat oleh siswa:

1. Pilih siswa yang ingin diumumkan hasilnya (atau pilih semua)
2. Aktifkan tombol **Umumkan** / **Show**
3. Siswa yang bersangkutan akan dapat melihat hasilnya di dashboard mereka

> [!IMPORTANT]
> Hasil hanya akan terlihat oleh siswa setelah Guru BK **mengaktifkan pengumuman**. Sebelum itu, siswa tidak dapat melihat penempatan paket mereka.

#### Export Data ke CSV

1. Pastikan filter sudah sesuai dengan data yang ingin diekspor
2. Klik tombol **Export CSV**
3. File `.csv` akan otomatis terunduh dengan nama format `final_results_YYYYMMDD_HHMMSS.csv`

File CSV berisi kolom:
- No, NISN, Nama Siswa, Nama Paket Final, Status Pencocokan, Show, Created At

---

### 11.2 Paket Tampung (Receive Results)

Siswa yang tidak mendapatkan paket yang cocok dari analisis otomatis akan masuk ke **Paket Tampung** sebagai penampungan sementara.

#### Mengakses Halaman Paket Tampung

1. Klik menu **Rekapitulasi** → **Paket Tampung** pada sidebar

#### Mengelola Siswa di Paket Tampung

Siswa di paket tampung perlu ditangani secara manual:

1. Lihat daftar pilihan paket yang dipilih siswa
2. Konsultasikan dengan siswa secara langsung
3. Pindahkan siswa ke paket yang paling sesuai menggunakan tombol **Pindah Paket**

> [!TIP]
> Siswa yang berstatus **"Tidak Sesuai"** di Final Results (pilihan paketnya berbeda dari hasil analisis) juga perlu mendapat perhatian dan konsultasi lanjutan.

---

## 12. Alur Kerja Lengkap (End-to-End)

Berikut adalah langkah-langkah lengkap yang disarankan untuk satu siklus akademik:

### 🔧 Persiapan Awal (Satu kali setup)

```
1. ✅ Lengkapi Profil Sekolah (NPSN, Nama, Alamat)
2. ✅ Tambahkan Mata Pelajaran yang digunakan di sekolah
3. ✅ Buat Paket Mapel beserta daftar mapel di dalamnya
4. ✅ Isi kapasitas setiap Paket Mapel
5. ✅ Tambahkan Bidang Cita-cita yang relevan
6. ✅ Atur pemetaan mapel pendukung untuk setiap Bidang Cita-cita
```

### 📥 Input Data Siswa & Nilai

```
7. ✅ Download template Excel dari menu Nilai Siswa
8. ✅ Isi template dengan data NISN, Nama, Gender, Tanggal Lahir, dan Nilai per Mapel
9. ✅ Upload file Excel → akun siswa otomatis terbuat
10. ✅ Verifikasi data siswa yang muncul di menu Data Siswa
```

### 🧪 Proses Tes Siswa

```
11. ⏳ Siswa login menggunakan NISN & tanggal lahir
12. ⏳ Siswa mengerjakan Tes RIASEC (42 soal)
13. ⏳ Siswa memilih 1 Bidang Cita-cita
14. ⏳ Siswa memilih 3 Prioritas Paket Mapel
```

### 📊 Pemantauan & Finalisasi

```
15. ✅ Pantau progres di menu Progres Siswa
16. ✅ Pastikan semua siswa mencapai progress 3/3 (atau sebagian besar sudah selesai)
17. ✅ Lakukan Finalisasi Progres → sistem menentukan paket untuk setiap siswa
18. ✅ Review hasil di menu Hasil Final
19. ✅ Tangani siswa di Paket Tampung — konsultasi & pindahkan ke paket yang sesuai
20. ✅ Pindahkan siswa antar paket jika ada ketidakseimbangan kapasitas
```

### 📢 Pengumuman Hasil

```
21. ✅ Aktifkan pengumuman untuk siswa yang sudah final
22. ✅ Siswa dapat melihat hasil akhir di dashboard mereka
23. ✅ Export data ke CSV untuk dokumentasi atau laporan
```

---

## 13. Tips & Troubleshooting

### ❓ Masalah Umum & Solusinya

---

#### 🔴 "Silahkan lengkapi data profil sekolah terlebih dahulu"

**Penyebab:** Profil sekolah belum diisi.

**Solusi:**
1. Pergi ke menu **Profil Sekolah**
2. Isi NPSN, Nama Sekolah, dan Alamat
3. Klik Simpan, lalu kembali ke menu sebelumnya

---

#### 🔴 Import Excel gagal atau data tidak muncul

**Penyebab:** Format file tidak sesuai atau kolom tidak cocok.

**Solusi:**
1. Selalu gunakan template yang diunduh dari sistem (jangan buat template sendiri)
2. Pastikan ekstensi file adalah `.xlsx` atau `.xls`
3. Jangan mengubah nama kolom pada template
4. Pastikan NISN diisi tanpa spasi atau karakter khusus

---

#### 🔴 Tombol "Lihat Detail" tidak bisa diklik

**Penyebab:** Progress siswa belum 3/3 (belum selesai semua tahapan).

**Solusi:** Dorong siswa untuk menyelesaikan semua tahapan (Tes RIASEC → Pilih Cita-cita → Pilih Paket).

---

#### 🔴 Siswa tidak bisa login

**Penyebab:** Akun siswa belum terdaftar atau data tidak sesuai.

**Solusi:**
1. Cek apakah NISN siswa sudah ada di menu **Data Siswa**
2. Jika belum ada, tambahkan manual atau import melalui Excel
3. Password default siswa biasanya menggunakan tanggal lahir (format: DDMMYYYY). Konfirmasi ke Administrator untuk reset jika diperlukan.

---

#### 🔴 Paket sudah penuh, tidak bisa menambah siswa

**Penyebab:** Kapasitas paket sudah tercapai.

**Solusi:**
1. Pindahkan beberapa siswa ke paket lain yang masih memiliki sisa kapasitas
2. Atau tambah kapasitas paket di menu **Edit Paket Mapel**

---

#### 🔴 Hasil analisis banyak yang "Tidak Sesuai"

**Penjelasan:** Ini berarti sistem menempatkan siswa ke paket yang tidak ada dalam pilihan prioritas siswa. Situasi ini normal terjadi ketika paket yang dipilih siswa sudah penuh kapasitasnya.

**Solusi:**
1. Lakukan sesi konsultasi dengan siswa yang berstatus "Tidak Sesuai"
2. Diskusikan apakah penempatan yang ada sudah tepat atau perlu pindah
3. Gunakan fitur **Pindah Paket** untuk menyesuaikan

---

### 💡 Tips Penggunaan Terbaik

1. **Lengkapi setup di awal** — Pastikan semua Mapel, Paket, dan Bidang Cita-cita sudah dikonfigurasi sebelum siswa mulai mengerjakan tes.

2. **Gunakan Import Excel** untuk efisiensi — Lebih cepat dari input manual, terutama jika jumlah siswa banyak.

3. **Pantau progres secara berkala** — Gunakan dashboard dan menu Progres Siswa untuk memastikan tidak ada siswa yang tertinggal.

4. **Lakukan finalisasi di akhir periode** — Tunggu sampai semua atau mayoritas siswa selesai (progress 3/3) sebelum finalisasi untuk hasil yang optimal.

5. **Review paket tampung segera** — Siswa di paket tampung perlu penanganan cepat agar proses penempatan tidak terhambat.

6. **Export data sebagai backup** — Unduh data CSV setelah finalisasi sebagai arsip dan bahan laporan.

---

## 📞 Kontak & Dukungan

Jika mengalami kendala teknis yang tidak tercantum dalam panduan ini, silakan hubungi **Administrator Sistem** yang bertanggung jawab mengelola APPEM di sekolah/instansi Anda.

---

*Dokumentasi ini dibuat berdasarkan versi APPEM yang sedang berjalan. Fitur dapat berkembang sesuai pembaruan sistem.*

**Versi Dokumen:** 1.0  
**Tanggal:** Agustus 2026
