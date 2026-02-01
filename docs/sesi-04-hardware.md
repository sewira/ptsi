# PTSI Sesi 4: Perangkat Keras (Hardware)

> **Mata Kuliah:** 200201204 - Pengantar Teknologi Sistem Informasi
> **Dosen:** Ega Dioni Putri, S.T., M.M.G.

---

## Big Picture

- Hardware = bagian **fisik** komputer
- Analogi: Hardware seperti **raga/tubuh**, Software seperti **jiwa/pikiran**
- Hardware dan Software **saling melengkapi** - tidak bisa berfungsi sendiri-sendiri

---

## Konsep Kunci

---

### 1. Definisi Hardware dan Komputer

**Hardware (Perangkat Keras):**
- Bagian fisik komputer dan komponen di dalamnya
- Seperti organ, otot, tulang dalam tubuh manusia
- "Mesin" yang menjalankan proses fisik

**Komputer:**
- Perangkat elektronik yang **mengolah data mentah**
- Memprosesnya sesuai **instruksi yang diberikan**
- Mengeluarkan **hasil sesuai harapan**

> **Ingat:** Hardware tanpa software = benda mati. Software tanpa hardware = tidak ada wadah.

---

### 2. Klasifikasi Hardware Berdasarkan Letak

| Internal | Eksternal |
|----------|-----------|
| Di dalam fisik komputer | Di luar, terhubung via port |
| **Esensial** (wajib ada) | **Periferal** (tambahan) |
| CPU, memori, kartu video | Keyboard, mouse, monitor, printer |

---

### 3. Empat Jenis Perangkat Keras (Wajib Hafal!)

#### A. Input Device (Perangkat Masukan)

**Fungsi:** Memasukkan data dari luar ke dalam memori/prosesor

**Contoh:**
- Keyboard
- Mouse
- Joystick
- Scanner
- Web Camera
- Microphone

**Dua Tipe Masukan:**
| Tipe | Fungsi | Hasil |
|------|--------|-------|
| **Signal Input** | Energi untuk mendapatkan output | Data |
| **Maintenance Input** | Energi agar komputer beroperasi | Program |

---

#### B. Processing Device (Perangkat Pemroses)

**Fungsi:** Menangani pemrosesan, penyimpanan, dan pengambilan informasi

**Contoh:**
- **CPU** (Central Processing Unit) - "Otak" komputer
- **GPU** (Graphic Processing Unit) - Proses grafis
- **Motherboard** - Papan utama penghubung semua komponen
- **Network Card** - Koneksi jaringan
- **Sound Card** - Proses suara
- **Video Card** - Proses tampilan video

---

#### C. Output Device (Perangkat Keluaran)

**Fungsi:** Mengeluarkan data/informasi dari komputer

**Contoh:**
- **Monitor** - Menampilkan informasi visual
- **Printer** - Mencetak ke kertas
- **Speaker** - Mengeluarkan suara
- **Headphone** - Suara personal
- **Projector** - Proyeksi ke layar besar

---

#### D. Storage Device (Perangkat Penyimpanan)

**Fungsi:** Menyimpan dan mengambil data/informasi digital

**Tiga Tipe Penyimpanan:**

| Tipe | Karakteristik | Contoh |
|------|---------------|--------|
| **Primer** | Internal, data hilang saat mati, ukuran kecil | RAM, Cache |
| **Sekunder** | Data permanen, ukuran besar | USB, HDD, SSD |
| **Tersier** | Data masif, biaya murah | DVD, Tape |

---

## Ringkasan 4 Jenis Hardware (Tabel Lengkap)

| Jenis | Fungsi | Contoh |
|-------|--------|--------|
| **Input** | Memasukkan data | Keyboard, Mouse, Scanner, Webcam, Mic |
| **Process** | Memproses data | CPU, GPU, Motherboard, Sound/Video Card |
| **Output** | Mengeluarkan data | Monitor, Printer, Speaker, Headphone |
| **Storage** | Menyimpan data | RAM, HDD, SSD, USB, DVD |

---

## Alur Kerja Hardware

```
INPUT → PROCESS → OUTPUT
  ↓         ↓         ↓
Keyboard   CPU      Monitor
Mouse      GPU      Printer
Scanner    RAM      Speaker
           ↓
        STORAGE
        (HDD/SSD)
```

---

## Perbedaan yang Sering Membingungkan

### CPU vs GPU

| Aspek | CPU | GPU |
|-------|-----|-----|
| Kepanjangan | Central Processing Unit | Graphic Processing Unit |
| Fungsi | Proses umum, "otak" komputer | Proses grafis/visual |
| Penggunaan | Semua operasi komputer | Gaming, video editing, AI |

### RAM vs HDD/SSD

| Aspek | RAM | HDD/SSD |
|-------|-----|---------|
| Tipe | Penyimpanan **primer** | Penyimpanan **sekunder** |
| Data | **Hilang** saat mati | **Permanen** |
| Kecepatan | Sangat cepat | Lebih lambat (HDD) / Cepat (SSD) |
| Kapasitas | Kecil (4-64 GB) | Besar (256 GB - TB) |

### HDD vs SSD

| Aspek | HDD | SSD |
|-------|-----|-----|
| Kepanjangan | Hard Disk Drive | Solid State Drive |
| Komponen | Ada piringan berputar | Chip memori (no moving parts) |
| Kecepatan | Lebih lambat | Lebih cepat |
| Harga | Lebih murah | Lebih mahal |
| Ketahanan | Rentan guncangan | Lebih tahan |

---

## Tips Menjawab Soal

### Cara Ingat 4 Jenis Hardware: "I-P-O-S"
- **I**nput - Masuk
- **P**rocess - Proses
- **O**utput - Keluar
- **S**torage - Simpan

### Keyword untuk Identifikasi

**Input Device:**
- Memasukkan, masukan, dari luar
- Keyboard, mouse, scanner, webcam, mic

**Processing Device:**
- Memproses, mengolah, menghitung
- CPU, GPU, motherboard

**Output Device:**
- Mengeluarkan, keluaran, menampilkan
- Monitor, printer, speaker

**Storage Device:**
- Menyimpan, penyimpanan, backup
- RAM, HDD, SSD, USB, DVD

---

## Contoh Soal Latihan

### Soal 1: Pilihan Ganda
**Manakah yang termasuk Input Device?**

a) Monitor
b) Printer
c) Keyboard
d) Speaker

> **Jawaban: C** - Keyboard adalah perangkat untuk memasukkan data

---

### Soal 2: Pilihan Ganda
**CPU adalah singkatan dari?**

a) Computer Processing Unit
b) Central Processing Unit
c) Central Program Unit
d) Computer Program Unit

> **Jawaban: B** - Central Processing Unit

---

### Soal 3: Pilihan Ganda
**Manakah yang merupakan penyimpanan primer?**

a) HDD
b) USB
c) RAM
d) DVD

> **Jawaban: C** - RAM adalah penyimpanan primer (data hilang saat komputer mati)

---

### Soal 4: Pilihan Ganda
**Perbedaan hardware internal dan eksternal adalah?**

a) Internal lebih mahal
b) Internal ada di dalam komputer dan esensial, eksternal di luar dan bersifat periferal
c) Eksternal lebih penting
d) Tidak ada perbedaan

> **Jawaban: B**

---

### Soal 5: Essay
**Sebutkan dan jelaskan 4 jenis perangkat keras berdasarkan fungsinya!**

> **Jawaban:**
> 1. **Input Device** - Perangkat untuk memasukkan data dari luar ke komputer. Contoh: keyboard, mouse, scanner
> 2. **Processing Device** - Perangkat untuk memproses data. Contoh: CPU, GPU, motherboard
> 3. **Output Device** - Perangkat untuk mengeluarkan data/informasi. Contoh: monitor, printer, speaker
> 4. **Storage Device** - Perangkat untuk menyimpan data. Contoh: HDD, SSD, RAM

---

### Soal 6: Essay
**Jelaskan perbedaan penyimpanan primer, sekunder, dan tersier!**

> **Jawaban:**
>
> | Tipe | Karakteristik | Contoh |
> |------|---------------|--------|
> | **Primer** | Data di internal komputer, hilang saat komputer mati, ukuran kecil | RAM, Cache |
> | **Sekunder** | Data permanen, ukuran besar | USB, HDD, SSD |
> | **Tersier** | Untuk data masif dengan biaya murah | DVD, Tape |

---

### Soal 7: Analisis
**Mengapa hardware dan software dikatakan saling melengkapi?**

> **Jawaban:**
> Hardware dan software saling melengkapi karena:
> 1. **Hardware tanpa software** = benda mati yang tidak berguna, tidak bisa melakukan apa-apa
> 2. **Software tanpa hardware** = tidak punya wadah untuk dijalankan
> 3. Ibarat tubuh (hardware) membutuhkan jiwa (software) untuk berfungsi
> 4. Keduanya harus ada agar komputer dapat bekerja sesuai harapan

---

## Quick Recall (Hafalan Cepat)

- **Hardware** = bagian fisik komputer
- **Komputer** = perangkat elektronik yang mengolah data → proses → hasil
- **4 Jenis Hardware** = Input, Process, Output, Storage (I-P-O-S)
- **Input** = Keyboard, Mouse, Scanner, Webcam
- **Process** = CPU, GPU, Motherboard
- **Output** = Monitor, Printer, Speaker
- **Storage** = RAM (primer), HDD/SSD (sekunder), DVD (tersier)
- **Internal** = esensial, di dalam (CPU, RAM)
- **Eksternal** = periferal, di luar (keyboard, mouse, monitor)

---

## Koneksi dengan CBIS

Hardware adalah salah satu dari **5 elemen CBIS**:
1. People
2. Data
3. **Hardware** ← Sesi ini!
4. Software
5. Telecommunications

---

*Sumber: Slide PTSI Sesi 4 - Perangkat Keras (Hardware), Universitas Siber Asia*
