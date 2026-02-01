# Prompt Template untuk Generate Dokumentasi PTSI

Salin prompt di bawah ini ke Claude Code untuk menghasilkan output yang serupa.

---

## PROMPT (Copy dari sini)

```
Saya mahasiswa Universitas Siber Asia yang sedang mempersiapkan ujian mata kuliah "Pengantar Teknologi Sistem Informasi" (PTSI).

Tolong bantu saya membuat dokumentasi markdown dari slide PDF kuliah dengan format berikut:

## FORMAT OUTPUT:
1. **Big Picture** - Gambaran besar materi dalam 3-5 poin
2. **Konsep Kunci** - Penjelasan detail setiap konsep dengan:
   - Definisi yang jelas
   - Tabel perbandingan jika ada
   - Contoh konkret
3. **Perbedaan yang Sering Membingungkan** - Tabel perbandingan konsep mirip
4. **Tips Menjawab Soal** - Akronim/mnemonik untuk menghafal, keyword identifikasi
5. **Contoh Soal Latihan** - Pilihan ganda dan essay dengan jawaban
6. **Quick Recall** - Poin-poin hafalan cepat dalam bullet points

## GAYA PENULISAN:
- Bahasa Indonesia
- Fokus pada konsep yang sering keluar di ujian
- Gunakan tabel untuk perbandingan
- Tambahkan akronim/mnemonik untuk memudahkan hafalan
- Tandai bagian "Wajib Hafal!" untuk konsep penting
- Concise, to the point, tidak bertele-tele

## INFORMASI TAMBAHAN:
Jangan hanya copy dari slide! Tambahkan juga:
- **Penjelasan lebih dalam** jika konsep di slide kurang jelas
- **Contoh real-world** yang relevan (misalnya contoh perusahaan, aplikasi nyata)
- **Analogi sederhana** untuk konsep yang abstrak
- **Informasi terkini** tentang teknologi yang dibahas
- **Common mistakes** yang sering dilakukan mahasiswa
- **Hubungan antar konsep** dengan materi sesi lain
- **Fun facts** atau trivia yang membantu mengingat

## INSTRUKSI:
1. Baca file PDF slide yang saya berikan
2. Buat dokumentasi markdown sesuai format di atas
3. Simpan ke folder: /Users/itkopnus/Documents/unsia/semester1/Pengantar Teknologi Sistem Informasi/docs/
4. Nama file: sesi-XX-[nama-topik].md

Sekarang tolong proses slide ini: [LAMPIRKAN PDF SLIDE]
```

---

## CONTOH PENGGUNAAN:

```
[Copy prompt di atas]

Sekarang tolong proses slide ini: @"Slide PTSI Sesi 9 - Jenis-jenis SI.pdf"
```

---

## STRUKTUR FILE YANG SUDAH DIBUAT:

| Sesi | File | Status |
|------|------|--------|
| 1 | sesi-01-pendahuluan.md | Done |
| 2 | sesi-02-cbis.md | Done |
| 3 | sesi-03-teknologi-komunikasi.md | Done |
| 4 | sesi-04-hardware.md | Done |
| 5 | sesi-05-software.md | Done |
| 6 | sesi-06-data-dan-gudang-data.md | Done |
| 7 | sesi-07-basis-data.md | Done |
| 9 | sesi-09-jenis-jenis-si.md | Pending |
| 10 | sesi-10-e-commerce.md | Pending |
| 11 | sesi-11-supply-chain-management.md | Pending |

---

## QUICK START (Prompt Singkat)

Jika Claude Code sudah pernah membaca file dokumentasi sebelumnya, bisa pakai prompt singkat:

```
Tolong buatkan dokumentasi markdown untuk slide PTSI dengan format yang sama seperti file-file di folder docs/. Fokus untuk persiapan ujian. Tambahkan juga informasi eksternal yang relevan (contoh real-world, penjelasan lebih dalam, analogi).

Slide: @"[NAMA FILE PDF]"
Simpan ke: docs/sesi-XX-[nama].md
```

---

## CONTOH INFORMASI EKSTERNAL YANG BISA DITAMBAHKAN:

| Topik di Slide | Informasi Tambahan |
|----------------|-------------------|
| DBMS | "MySQL digunakan oleh Facebook, Twitter. PostgreSQL digunakan Spotify, Instagram" |
| E-commerce | "Tokopedia, Shopee, Bukalapak adalah contoh C2C dan B2C di Indonesia" |
| Data Warehouse | "Google BigQuery dan Amazon Redshift adalah contoh cloud DWH modern" |
| Sistem Operasi | "Android berbasis Linux, iOS berbasis Unix (Darwin)" |
| Supply Chain | "Indomie menggunakan SCM untuk distribusi ke 90+ negara" |

Informasi seperti ini membantu mengingat konsep karena terhubung dengan hal yang familiar.
