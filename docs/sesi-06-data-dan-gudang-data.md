# PTSI Sesi 6: Data dan Gudang Data (Data Warehouse)

> **Mata Kuliah:** 200201204 - Pengantar Teknologi Sistem Informasi
> **Dosen:** Ega Dioni Putri, S.T., M.M.G.

---

## Big Picture

- **Data** = masukan mentah dari sistem informasi, fakta-fakta yang perlu dikelola
- **Data Warehouse (DWH)** = "perpustakaan" untuk menyimpan dan menganalisis data dari berbagai sumber
- Analogi: Jika **Database adalah buku**, maka **Data Warehouse adalah perpustakaan**
- DWH mendukung **pengambilan keputusan** dan **intelijen bisnis**

---

## Konsep Kunci

---

### 1. Pengertian Data

**Data adalah:**
- Satu atau lebih **simbol** yang digunakan untuk merepresentasikan sesuatu
- **Aliran fakta-fakta** dalam bentuk yang belum terformat
- **Fakta mentah** terkait orang, tempat, kegiatan yang punya makna penting
- Seluruh fakta tentang dunia kita

> **Catatan:** DATA adalah bentuk jamak dari *datum*, tetapi lazimnya dianggap single sebagai sebuah unit

**Karakteristik Data:**
- Tidak semua data di dunia dianggap signifikan atau menarik
- Sebagian data disetujui semua orang, sebagian diperdebatkan
- Beberapa bersifat pribadi bagi individu/kelompok tertentu
- Data = **masukan mentah** dari sistem informasi

---

### 2. Pentingnya Menyimpan Data

**Mengapa data penting perlu disimpan?**
- Data bisnis bisa sangat **besar dan heterogen**
- Teknik penyimpanan yang tepat memastikan:
  - Manajemen yang baik
  - Lokasi dan distribusi yang tepat
  - Aliran objek yang teratur

**Isu yang perlu dipertimbangkan:**
- **Penempatan data** - di mana data disimpan?
- **Teknologi (media)** - apa yang digunakan untuk penyimpanan?
- **Distribusi** - lokal atau jarak jauh?
- **Kecepatan pengiriman** - seberapa cepat data bisa diakses?

---

### 3. Pengertian Data Warehouse (DWH) - Wajib Hafal!

**Data Warehouse adalah:**
> Sistem atau repositori **terpusat** yang dirancang untuk **menyimpan, mengelola, dan menganalisis** sejumlah besar data dari **berbagai sumber**; terutama digunakan untuk **intelijen bisnis** dan **pengambilan keputusan**

**Analogi Penting:**
- **Database = Buku** (satu sumber informasi)
- **Data Warehouse = Perpustakaan** (kumpulan banyak buku/database)

---

### 4. Perbedaan Database vs Data Warehouse (Sering Keluar di Ujian!)

| Aspek | Database (Basis Data) | Data Warehouse (Gudang Data) |
|-------|----------------------|------------------------------|
| **Tujuan** | Operasi harian (transaksi) | Analitik, pelaporan, pengambilan keputusan |
| **Struktur Data** | Data terkini, terperinci, real-time | Data historis dan agregasi |
| **Sumber Data** | Umumnya dari **satu sistem** | Dari **berbagai sumber** (multi-departemen) |
| **Bentuk Query** | Kecil & sederhana (CRUD) | Besar & kompleks (analisis tren) |
| **Kinerja** | Kecepatan transaksional | Banyak membaca data, query kompleks |
| **Pembaruan** | **Sering** dilakukan | **Jarang** (lebih stabil untuk analisis) |

> **CRUD** = Copy, Read, Update, Delete

---

### 5. Pentingnya DWH dalam Sistem Informasi

**Hubungan IS dan DWH:**
- **IS (Information System)**: mengumpulkan, memproses, menyimpan, dan menyebarluaskan informasi untuk mendukung pengambilan keputusan
- **DWH**: bertindak sebagai **komponen utama** SI tingkat lanjut, memungkinkan wawasan lebih mendalam

**4 Penggunaan DWH dalam SI:**

| No | Penggunaan | Penjelasan |
|----|------------|------------|
| 1 | **Integrasi Data** | Mengintegrasikan dan mengonsolidasikan informasi dari berbagai sistem (penjualan, pelanggan, SDM) |
| 2 | **Dukungan Pengambilan Keputusan** | Memproses data historis untuk analisis tren, peramalan, perencanaan strategis |
| 3 | **Pelaporan Lebih Baik** | Memungkinkan pelaporan tingkat lanjut dengan data agregasi dari waktu ke waktu |
| 4 | **Efisiensi Analisis** | Mendukung alat analitik bisnis untuk eksplorasi data mendalam |

---

### 6. Kegunaan Data Warehouse (Hafal!)

| Kegunaan | Contoh Aktivitas |
|----------|------------------|
| **Intelijen Bisnis** | Analisis tren penjualan, pantau perilaku pelanggan, ramalkan permintaan pasar |
| **Reporting (Pelaporan)** | Membuat dashboard, laporan bulanan/tahunan |
| **Analisis Data** | Menemukan pola, menyortir, memodelkan data |
| **Pengambilan Keputusan** | Perencanaan strategis, evaluasi keberhasilan marketing |

**Dashboard:** Antarmuka yang menampilkan data-data penting dalam bentuk bagan, gambar, atau tabel

---

### 7. Jenis dan Contoh DWH

| Jenis | Fungsi | Contoh |
|-------|--------|--------|
| **Database System** | Sistem penyimpanan data | Oracle Database, MS SQL Server, Amazon RDS |
| **BI (Business Intelligence) Tools** | Alat visualisasi dan analisis bisnis | Looker, Tableau, Power BI |
| **ETL Tools** | Extract, Transform, Load data | Informatica, Talend, Apache Nifi |

> **Catatan:** Ketiga jenis ini bisa saling beririsan atau digabungkan dalam satu DWH

**ETL = Extract, Transform, Load:**
- **Extract** = Mengambil data dari berbagai sumber
- **Transform** = Mengubah/membersihkan data
- **Load** = Memasukkan data ke DWH

---

## Perbedaan yang Sering Membingungkan

### Data vs Informasi (Review)

| Aspek | Data | Informasi |
|-------|------|-----------|
| Sifat | Fakta mentah | Sudah diproses |
| Makna | Belum punya makna | Punya konteks dan makna |
| Contoh | "100", "Jakarta" | "Penjualan Jakarta: 100 unit" |

### Database vs Data Warehouse

| Aspek | Database | Data Warehouse |
|-------|----------|----------------|
| Analogi | **Buku** | **Perpustakaan** |
| Skala | Satu sistem | Multi-sistem |
| Fokus | Operasional harian | Analisis & keputusan |
| Data | Real-time, terkini | Historis, agregasi |
| Query | Sederhana (CRUD) | Kompleks (analisis) |

### IS vs DWH

| Aspek | Information System (IS) | Data Warehouse (DWH) |
|-------|------------------------|----------------------|
| Fungsi | Mengumpulkan, memproses, menyimpan, menyebarkan informasi | Menyimpan dan menganalisis data dari berbagai sumber |
| Posisi | Sistem keseluruhan | Komponen utama SI tingkat lanjut |
| Tujuan | Mendukung operasi dan keputusan | Intelijen bisnis dan pengambilan keputusan |

---

## Tips Menjawab Soal

### Keyword Data Warehouse
- Repositori terpusat
- Berbagai sumber
- Analitik / analisis
- Intelijen bisnis
- Pengambilan keputusan
- Data historis

### Keyword Database
- Operasi harian
- Transaksi
- Real-time
- CRUD (Copy, Read, Update, Delete)
- Satu sistem

### Cara Ingat Perbedaan DB vs DWH
**"DB = Harian, DWH = Historis"**
- **D**ata**B**ase = operasi **harian**, satu sumber
- **D**ata **W**are**H**ouse = data **historis**, banyak sumber

### Cara Ingat Kegunaan DWH: "BI-RAD"
- **B**usiness **I**ntelligence
- **R**eporting
- **A**nalisis Data
- **D**ecision Making (Pengambilan Keputusan)

### Cara Ingat ETL
- **E**xtract = **Ambil** data
- **T**ransform = **Ubah** data
- **L**oad = **Masukkan** ke DWH

---

## Contoh Soal Latihan

### Soal 1: Pilihan Ganda
**Apa yang dimaksud dengan Data Warehouse?**

a) Database untuk menyimpan data harian
b) Sistem untuk memproses transaksi real-time
c) Repositori terpusat untuk menyimpan, mengelola, dan menganalisis data dari berbagai sumber
d) Software untuk membuat laporan sederhana

> **Jawaban: C** - DWH adalah repositori terpusat untuk menyimpan, mengelola, dan menganalisis data dari berbagai sumber untuk intelijen bisnis dan pengambilan keputusan

---

### Soal 2: Pilihan Ganda
**Apa perbedaan utama antara Database dan Data Warehouse?**

a) Database lebih mahal dari Data Warehouse
b) Database untuk operasi harian, Data Warehouse untuk analitik dan pengambilan keputusan
c) Data Warehouse hanya menyimpan data terkini
d) Database menggunakan data dari berbagai sumber

> **Jawaban: B** - Database untuk operasi harian (transaksi), DWH untuk analitik dan pengambilan keputusan

---

### Soal 3: Pilihan Ganda
**Manakah yang BUKAN kegunaan Data Warehouse?**

a) Intelijen Bisnis
b) Pelaporan (Reporting)
c) Transaksi harian
d) Analisis Data

> **Jawaban: C** - Transaksi harian adalah fungsi Database, bukan Data Warehouse

---

### Soal 4: Pilihan Ganda
**Apa kepanjangan dari ETL?**

a) Extract, Transfer, Load
b) Extract, Transform, Load
c) External, Transform, Local
d) Extract, Transmit, Link

> **Jawaban: B** - ETL = Extract, Transform, Load

---

### Soal 5: Pilihan Ganda
**Jika Database diibaratkan sebagai buku, maka Data Warehouse diibaratkan sebagai?**

a) Majalah
b) Koran
c) Perpustakaan
d) Jurnal

> **Jawaban: C** - Database = Buku, Data Warehouse = Perpustakaan (kumpulan banyak database)

---

### Soal 6: Essay
**Jelaskan perbedaan Database dan Data Warehouse! (minimal 4 aspek)**

> **Jawaban:**
>
> | Aspek | Database | Data Warehouse |
> |-------|----------|----------------|
> | **Tujuan** | Operasi harian seperti transaksi | Analitik, pelaporan, pengambilan keputusan |
> | **Sumber Data** | Umumnya dari satu sistem | Dari berbagai sumber (multi-departemen) |
> | **Struktur Data** | Data terkini dan real-time | Data historis dan agregasi |
> | **Pembaruan** | Sering dilakukan | Jarang dilakukan, lebih stabil |

---

### Soal 7: Essay
**Sebutkan dan jelaskan 4 kegunaan Data Warehouse!**

> **Jawaban:**
> 1. **Intelijen Bisnis** - Menganalisis tren penjualan, memantau perilaku pelanggan, meramalkan permintaan pasar
> 2. **Reporting (Pelaporan)** - Membuat dashboard dan laporan bulanan/tahunan untuk pemangku kepentingan
> 3. **Analisis Data** - Melakukan analisis terperinci untuk menemukan pola dan mengambil kesimpulan
> 4. **Pengambilan Keputusan** - Mendukung perencanaan strategis dan mengevaluasi keberhasilan marketing

---

### Soal 8: Analisis
**Mengapa Data Warehouse penting dalam Sistem Informasi?**

> **Jawaban:**
> Data Warehouse penting dalam Sistem Informasi karena:
> 1. **Integrasi Data** - Mengintegrasikan data dari berbagai departemen (penjualan, SDM, pelanggan) ke satu tempat
> 2. **Dukungan Keputusan** - Menyediakan data historis untuk analisis tren dan perencanaan strategis
> 3. **Pelaporan Tingkat Lanjut** - Memungkinkan pelaporan dengan data agregasi dari waktu ke waktu
> 4. **Efisiensi Analisis** - Mendukung alat analitik bisnis seperti Power BI dan Tableau untuk eksplorasi data mendalam

---

## Quick Recall (Hafalan Cepat)

- **Data** = fakta mentah, masukan mentah SI
- **Data Warehouse** = repositori terpusat untuk menyimpan dan menganalisis data dari berbagai sumber
- **Analogi** = Database adalah buku, DWH adalah perpustakaan
- **DB vs DWH** = Harian vs Historis, Satu sumber vs Berbagai sumber
- **Kegunaan DWH** = BI, Reporting, Analisis Data, Pengambilan Keputusan (BI-RAD)
- **ETL** = Extract, Transform, Load
- **Contoh DB System** = Oracle, SQL Server, Amazon RDS
- **Contoh BI Tools** = Looker, Tableau, Power BI
- **Contoh ETL Tools** = Informatica, Talend, Apache Nifi

---

## Koneksi dengan CBIS

Data adalah salah satu dari **5 elemen CBIS**:
1. People
2. **Data** <- Sesi ini!
3. Hardware
4. Software
5. Telecommunications

---

*Sumber: Slide PTSI Sesi 6 - Data dan Gudang Data, Universitas Siber Asia*
