# PTSI Sesi 7: Basis Data (Database)

> **Mata Kuliah:** 200201204 - Pengantar Teknologi Sistem Informasi
> **Dosen:** Ega Dioni Putri, S.T., M.M.G.

---

## Big Picture

- **Basis Data (Database)** = kumpulan data yang saling berhubungan dan diorganisasi untuk akses cepat dan mudah
- **DBMS** = software untuk membuat, mendefinisikan, dan mengelola basis data
- Basis data berperan **sentral** dalam SI untuk menyimpan, mengambil, dan mengelola data secara efisien
- Contoh penggunaan: perbankan, e-commerce, perawatan kesehatan

---

## Konsep Kunci

---

### 1. Definisi Basis Data (Wajib Hafal!)

**Basis Data adalah:**
1. Himpunan kelompok data yang **saling berhubungan** dan diorganisasi agar dapat **diakses/dikelola secara cepat dan mudah**
2. Kumpulan data yang disimpan bersama **tanpa pengulangan (redundansi)** yang tidak perlu
3. Kumpulan file/tabel/arsip yang saling berhubungan dan disimpan dalam **media penyimpanan ekonomis**

**Pentingnya Basis Data dalam SI:**
- Peran sentral dalam menyimpan, mengambil, dan mengelola data secara efisien
- Contoh penggunaan: perbankan, e-commerce, perawatan kesehatan

---

### 2. Operasi Dasar Basis Data (Hafal!)

| No | Operasi | Nama Perintah | Fungsi |
|----|---------|---------------|--------|
| 1 | Pembuatan basis data baru | `CREATE DATABASE` | Membuat database baru |
| 2 | Penghapusan basis data | `DROP DATABASE` | Menghapus database |
| 3 | Pembuatan tabel baru | `CREATE TABLE` | Membuat tabel ke dalam database |
| 4 | Penghapusan tabel | `DROP TABLE` | Menghapus tabel dari database |
| 5 | Penambahan data | `INSERT` | Menambah data baru ke file |
| 6 | Pengambilan data | `RETRIEVE/SEARCH` | Mengambil data dari file |
| 7 | Pengubahan data | `UPDATE` | Mengubah data yang ada |
| 8 | Penghapusan data | `DELETE` | Menghapus data dari file |

---

### 3. Sistem Basis Data

**Komponen Sistem Basis Data:**
- **Hardware** (tidak terlihat di bagan)
- **Operating System** (sistem operasi)
- **Databases** (beberapa basis data)
- **DBMS** (Database Management System)
- **Users** (pengguna)
- **Applications** (dukungan perangkat lunak lain)

```
┌─────────────────────────────────────┐
│     User 1    User 2    User 3     │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│    Application    │    Developer    │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│   Database Management System (DBMS) │
│         Database Administrator      │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│         Operating System            │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│            Database                 │
└─────────────────────────────────────┘
```

> **Poin Penting:** Sistem basis data mengacu pada **DBMS dan data yang dikelolanya**

---

### 4. Database Management System (DBMS) - Wajib Hafal!

**Definisi DBMS:**
> Sistem perangkat lunak yang berperan sebagai **antarmuka** sehingga memungkinkan pengguna untuk **membuat, mendefinisikan, dan mengelola** basis data

**Kemampuan DBMS:**
- Menyimpan, mengatur, dan mengambil data dalam jumlah besar dengan **cepat dan efisien**
- Menegakkan **integritas data**
- Menjaga **keamanan**
- Mempermudah **pengelolaan dan analisis** data

**Contoh DBMS:**
- Microsoft SQL Server
- Oracle Database
- PostgreSQL
- MySQL

---

### 5. Komponen Fungsional DBMS (Hafal!)

| No | Komponen | Fungsi |
|----|----------|--------|
| 1 | **Database Manager/Engine** | Menyediakan interface antara data low-level dengan aplikasi dan query; menafsirkan & mengeksekusi permintaan; memastikan integritas dan keamanan data |
| 2 | **File/Storage Manager** | Mengelola alokasi ruang disk; menangani backup & recovery; merepresentasikan informasi dalam disk |
| 3 | **Query Processor** | Menerjemahkan perintah query ke perintah low-level; mentransformasi permintaan ke bentuk lebih efisien |
| 4 | **DML Precompiler** | Mengkonversi perintah DML (Data Manipulation Language) ke pemanggilan prosedur |
| 5 | **DDL Compiler** | Mengkonversi perintah DDL (Data Definition Language) ke tabel metadata; disimpan di data dictionary |

**DML vs DDL:**
- **DML** = Data Manipulation Language (manipulasi data: SELECT, INSERT, UPDATE, DELETE)
- **DDL** = Data Definition Language (definisi struktur: CREATE, ALTER, DROP)

---

### 6. Model-Model Basis Data (Hafal!)

| Model | Penjelasan | Kategori |
|-------|------------|----------|
| **Relational Model** | Paling umum digunakan; data dalam bentuk tabel 2 dimensi | Berbasis record |
| **Hierarchical Model** | Record dihubungkan dengan struktur pohon (tree) | Berbasis record |
| **Network Model** | Mirip hierarchical, tapi satu anak bisa punya lebih dari satu parent | Berbasis record |
| **Object-oriented Model** | Object dihubungkan melalui metode | Berbasis object |
| **Entity-Relationship (ERM)** | Diagram yang menunjukkan hubungan antar entitas | Berbasis object |
| **Semantic Model** | Menggunakan semantik untuk menyusun dan mendeskripsikan basis data | Berbasis object |

> **Poin Penting:** **Relational Model** adalah yang **paling umum digunakan**

---

### 7. Relational Database (Sering Keluar di Ujian!)

**Definisi:**
Kumpulan file spreadsheet yang membantu bisnis mengatur, mengelola, dan menghubungkan data

**Struktur Tabel (2 Dimensi):**

| Istilah | Nama Lain | Penjelasan |
|---------|-----------|------------|
| **Kolom (Column)** | Field, Attribute | Lajur vertikal; menyatakan tipe data |
| **Baris (Row)** | Record, Tuple | Lajur mendatar; mengandung nilai spesifik |

**Atribut Kunci (Wajib Hafal!):**

| Jenis Key | Penjelasan |
|-----------|------------|
| **Primary Key** | Atribut kunci dalam baris yang nilainya **UNIK** (tidak dimiliki baris lain) |
| **Foreign Key** | **Referensi** ke primary key di tabel lain (menghubungkan antar tabel) |

**Contoh Tabel:**

| NIM (PK) | Nama Mahasiswa | Alamat | Tanggal Lahir |
|----------|----------------|--------|---------------|
| 980001 | Ali Akbar | Jl. Dago 101 Cirebon | 2 Januari 1979 |
| 980002 | Budi Haryanto | Jl. Gajah Mada 10 Bandung | 6 Oktober 1978 |

---

### 8. Struktur Dasar Basis Data

**Hierarki:**
```
Database
    └── Schema (struktur logis)
            └── Table
                    └── Column (Field)
```

**Schema** = Struktur logis sebuah basis data

**Struktur Setiap Tabel:**
- Nama kolom (field)
- Tipe data (Character, Integer, Date, dll)
- Lebar (karakter maksimum yang dapat ditampung)

---

### 9. Operasi CRUD (Wajib Hafal!)

| Huruf | Operasi | Fungsi |
|-------|---------|--------|
| **C** | Create | Adding new data (menambah data baru) |
| **R** | Read | Retrieving data (mengambil data) |
| **U** | Update | Modifying data (mengubah data) |
| **D** | Delete | Removing data (menghapus data) |

---

### 10. Query dan SQL

**Query:**
> Sebuah **permintaan akan informasi**, bisa berasal dari pengguna atau sistem

**SQL (Structured Query Language):**
> Bahasa pemrograman untuk **menyimpan dan mengolah data** pada basis data relasional

**Perintah Umum SQL:**
- `SELECT` - Mengambil data
- `INSERT` - Menambah data
- `UPDATE` - Mengubah data
- `DELETE` - Menghapus data

**Contoh SQL:**
```sql
-- MENCARI MATA KULIAH YANG BOBOTNYA 3 SKS
SELECT mata_kuliah
FROM tabel_kuliah
WHERE SKS = 3;
```

---

### 11. Plus Minus Penggunaan Database

**Manfaat (+):**
- Sentralisasi dan integrasi data
- Peningkatan efisiensi dan keamanan data
- Dukungan untuk banyak pengguna (kemudahan berbagi data)
- Redundansi data bisa dikurangi
- Mekanisme pemulihan data jika hilang sudah tersedia di DBMS

**Tantangan (-):**
- Kompleksitas desain basis data, perlu SDM terampil
- Masalah pemeliharaan dan kinerja
- Biaya HW dan SW meningkat (butuh high speed processor & kapasitas besar)
- Untuk organisasi kecil, DBMS justru tidak efektif

---

## Perbedaan yang Sering Membingungkan

### Database vs Data Warehouse (Review Sesi 6)

| Aspek | Database | Data Warehouse |
|-------|----------|----------------|
| Tujuan | Operasi harian (transaksi) | Analitik & pengambilan keputusan |
| Data | Real-time, terkini | Historis, agregasi |
| Query | Sederhana (CRUD) | Kompleks (analisis) |

### Primary Key vs Foreign Key

| Aspek | Primary Key | Foreign Key |
|-------|-------------|-------------|
| Fungsi | Identifikasi **unik** setiap baris | **Referensi** ke tabel lain |
| Nilai | Harus unik, tidak boleh NULL | Boleh duplikat, boleh NULL |
| Jumlah | Satu per tabel | Bisa banyak per tabel |

### DML vs DDL

| Aspek | DML | DDL |
|-------|-----|-----|
| Kepanjangan | Data Manipulation Language | Data Definition Language |
| Fungsi | Manipulasi **data** | Definisi **struktur** |
| Perintah | SELECT, INSERT, UPDATE, DELETE | CREATE, ALTER, DROP |

### Column vs Row

| Aspek | Column (Kolom) | Row (Baris) |
|-------|----------------|-------------|
| Nama lain | Field, Attribute | Record, Tuple |
| Arah | Vertikal | Horizontal |
| Isi | Tipe data | Nilai data |

---

## Tips Menjawab Soal

### Cara Ingat CRUD
**C-R-U-D** = **C**reate, **R**ead, **U**pdate, **D**elete
- Urutan operasi dasar pada data

### Cara Ingat Komponen DBMS: "DaFi-QuDiDi"
- **Da**tabase Manager
- **Fi**le Manager
- **Qu**ery Processor
- **D**ML Precompiler
- **D**DL Compiler

### Cara Ingat Model Database
**Model berbasis Record:** "Re-Hi-Ne"
- **Re**lational
- **Hi**erarchical
- **Ne**twork

**Model berbasis Object:** "Ob-En-Se"
- **Ob**ject-oriented
- **En**tity-Relationship
- **Se**mantic

### Keyword Identifikasi

**Primary Key:**
- Unik
- Tidak boleh NULL
- Identifikasi baris

**Foreign Key:**
- Referensi
- Menghubungkan tabel
- Relasi antar tabel

**DBMS:**
- Antarmuka
- Membuat, mendefinisikan, mengelola
- Integritas, keamanan

---

## Contoh Soal Latihan

### Soal 1: Pilihan Ganda
**Apa kepanjangan dari DBMS?**

a) Data Base Management Software
b) Database Management System
c) Data Basic Management System
d) Database Maintenance System

> **Jawaban: B** - DBMS = Database Management System

---

### Soal 2: Pilihan Ganda
**Manakah yang merupakan operasi CRUD?**

a) Create, Run, Update, Delete
b) Copy, Read, Update, Delete
c) Create, Read, Update, Delete
d) Create, Read, Upload, Download

> **Jawaban: C** - CRUD = Create, Read, Update, Delete

---

### Soal 3: Pilihan Ganda
**Apa yang dimaksud dengan Primary Key?**

a) Kunci untuk membuka database
b) Atribut yang nilainya unik dan mengidentifikasi setiap baris
c) Referensi ke tabel lain
d) Password untuk akses database

> **Jawaban: B** - Primary Key adalah atribut kunci yang nilainya unik, tidak dimiliki baris lain

---

### Soal 4: Pilihan Ganda
**Model basis data yang paling umum digunakan adalah?**

a) Hierarchical Model
b) Network Model
c) Relational Model
d) Object-oriented Model

> **Jawaban: C** - Relational Model adalah yang paling umum digunakan

---

### Soal 5: Pilihan Ganda
**Manakah yang BUKAN komponen fungsional DBMS?**

a) Database Manager
b) Query Processor
c) File Manager
d) Operating System

> **Jawaban: D** - Operating System bukan komponen DBMS, melainkan komponen sistem basis data secara keseluruhan

---

### Soal 6: Essay
**Jelaskan apa itu DBMS dan sebutkan 3 kemampuannya!**

> **Jawaban:**
> DBMS (Database Management System) adalah sistem perangkat lunak yang berperan sebagai antarmuka sehingga memungkinkan pengguna untuk membuat, mendefinisikan, dan mengelola basis data.
>
> 3 Kemampuan DBMS:
> 1. Menyimpan, mengatur, dan mengambil data dalam jumlah besar dengan cepat dan efisien
> 2. Menegakkan integritas data dan menjaga keamanan
> 3. Mempermudah pengelolaan dan analisis data

---

### Soal 7: Essay
**Jelaskan perbedaan Primary Key dan Foreign Key!**

> **Jawaban:**
>
> | Aspek | Primary Key | Foreign Key |
> |-------|-------------|-------------|
> | Definisi | Atribut kunci yang nilainya unik untuk mengidentifikasi setiap baris | Referensi ke primary key di tabel lain |
> | Nilai | Harus unik, tidak boleh NULL | Boleh duplikat, boleh NULL |
> | Fungsi | Identifikasi unik setiap record | Menghubungkan antar tabel (relasi) |

---

### Soal 8: Essay
**Sebutkan dan jelaskan 5 komponen fungsional DBMS!**

> **Jawaban:**
> 1. **Database Manager/Engine** - Menyediakan interface antara data dengan aplikasi; menafsirkan dan mengeksekusi permintaan pengguna
> 2. **File/Storage Manager** - Mengelola alokasi ruang disk dan menangani backup & recovery
> 3. **Query Processor** - Menerjemahkan perintah query ke perintah low-level yang dapat dimengerti database manager
> 4. **DML Precompiler** - Mengkonversi perintah DML ke pemanggilan prosedur normal
> 5. **DDL Compiler** - Mengkonversi perintah DDL ke tabel metadata yang disimpan di data dictionary

---

### Soal 9: Analisis
**Mengapa relational model adalah model basis data yang paling umum digunakan?**

> **Jawaban:**
> Relational model paling umum digunakan karena:
> 1. **Struktur sederhana** - Data disimpan dalam bentuk tabel 2 dimensi yang mudah dipahami
> 2. **Fleksibel** - Mudah menambah, mengubah, dan menghapus data
> 3. **Relasi antar tabel** - Menggunakan primary key dan foreign key untuk menghubungkan tabel
> 4. **SQL** - Didukung oleh bahasa query standar (SQL) yang mudah dipelajari
> 5. **Mengurangi redundansi** - Data tidak perlu diulang di banyak tempat

---

## Quick Recall (Hafalan Cepat)

- **Basis Data** = kumpulan data saling berhubungan, tanpa redundansi, akses cepat & mudah
- **DBMS** = software antarmuka untuk membuat, mendefinisikan, mengelola database
- **CRUD** = Create, Read, Update, Delete
- **Primary Key** = atribut unik, identifikasi baris
- **Foreign Key** = referensi ke primary key tabel lain
- **Relational Model** = model paling umum, data dalam tabel 2D
- **Column** = Field/Attribute (vertikal)
- **Row** = Record/Tuple (horizontal)
- **SQL** = bahasa untuk menyimpan dan mengolah data
- **DDL** = Data Definition Language (CREATE, ALTER, DROP)
- **DML** = Data Manipulation Language (SELECT, INSERT, UPDATE, DELETE)
- **Contoh DBMS** = MySQL, PostgreSQL, Oracle, SQL Server

---

## Koneksi dengan CBIS

Basis Data adalah bagian dari elemen **Data** dalam 5 elemen CBIS:
1. People
2. **Data** <- Sesi 6 & 7!
3. Hardware
4. Software
5. Telecommunications

---

*Sumber: Slide PTSI Sesi 7 - Basis Data, Universitas Siber Asia*
