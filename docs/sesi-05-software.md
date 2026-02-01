# PTSI Sesi 5: Perangkat Lunak (Software)

> **Mata Kuliah:** 200201204 - Pengantar Teknologi Sistem Informasi
> **Dosen:** Ega Dioni Putri, S.T., M.M.G.

---

## Big Picture

- Software = **pikiran, jiwa, dan akal** komputer
- Software adalah instruksi yang memberi tahu hardware apa yang harus dilakukan
- Tanpa software, komputer tidak dapat beroperasi (minimal harus ada OS)

---

## Konsep Kunci

---

### 1. Definisi Software

**Software adalah:**
- Sekumpulan item/objek yang membentuk "konfigurasi" meliputi:
  - **Programs** (program)
  - **Documents** (dokumen)
  - **Data**

**Menurut IEEE (1990):**
> "Computer programs, procedures, and possibly associated documentation and data pertaining to the operation of a computer system"

**Karakteristik Software:**
- Software is **engineered**, not manufactured (direkayasa, bukan diproduksi)
- Software does **not wear out**, but it does **deteriorate** (tidak aus, tapi bisa usang)
- Software is both a **product** and a **vehicle** for delivering information
- Most software is still **custom-built**

---

### 2. Peran Software

**Tanpa software, komputer tidak bisa beroperasi!**

**Peran software secara umum:**
- Melakukan aktivitas **bersama-sama dengan hardware**
- Menyediakan segala **sumber daya** yang bisa digunakan pada komputer
- Memungkinkan **user berkomunikasi** dengan hardware melalui perintah

---

### 3. Empat Jenis Software pada Komputer (Wajib Hafal!)

| Jenis | Fungsi | Contoh |
|-------|--------|--------|
| **Sistem Operasi** | Mengatur sistem kerja komputer, penerjemah HW-SW | Windows, macOS, Linux, Android |
| **Bahasa Pemrograman** | Memfasilitasi penulisan, pengujian, eksekusi program | Python, Java, C++, JavaScript |
| **Program Utilitas** | Mengelola, mengoptimalkan, memelihara komputer | Antivirus, Disk Cleanup, Backup |
| **Program Aplikasi** | Membantu pekerjaan spesifik pengguna | MS Office, Photoshop, Chrome |

---

### 4. Sistem Operasi (Operating System - OS)

**Definisi:**
Program yang berfungsi untuk **mengatur sistem kerja seluruh komputer** seperti **penerjemah antara HW dan SW**

**Fungsi OS:**
- Mengelola operasi-operasi komputer
- Mengeksekusi program-program aplikasi
- Menyediakan antarmuka (interface) untuk pengguna
- Mengkoordinasikan instalasi dan pembuangan program
- Menentukan program mana yang harus jalan, I/O device atau memori yang dipakai

**Contoh OS:**
- **Desktop:** Windows, macOS, Linux, Ubuntu, ChromeOS
- **Mobile:** Android, iOS, Symbian
- **Server:** Unix, FreeBSD

---

### 5. Bahasa Pemrograman

**Definisi:**
Sekumpulan instruksi dan tools yang dibuat untuk memfasilitasi **penulisan, pengujian, dan eksekusi program**

**Mengapa termasuk software?**
- Termasuk **compiler, interpreter, dan runtime environment** (ketiganya SW)
- Memfasilitasi pengembangan SW bagi developer
- Membutuhkan update untuk naik versi atau bug improvement
- Berinteraksi dengan SW lainnya

**Contoh:** Python, Java, C++, JavaScript, PHP, Go

---

### 6. Program Utilitas (Utility Program)

**Definisi:**
Disebut juga **program layanan**, yaitu software yang dirancang untuk **mengelola dan menyesuaikan** hardware, OS, atau aplikasi

**Fungsi:**
- Menganalisis sistem
- Mengkonfigurasi pengaturan
- Mengoptimalkan kinerja
- Memelihara komputer

**Contoh:**
- Backup
- Disk Cleanup
- Disk Defragmenter
- Antivirus
- System Restore
- File Manager

---

### 7. Program Aplikasi

**Definisi:**
Software **siap pakai** yang digunakan untuk membantu pekerjaan pengguna

**Karakteristik:**
- Dikembangkan sendiri atau dibeli dari pemasok luar
- Untuk kebutuhan tertentu/spesifik
- Bersifat tambahan

**Lokasi di Windows:**
- `C:\Program Files` → Aplikasi 64-bit
- `C:\Program Files (x86)` → Aplikasi 32-bit

**Contoh:** MS Office, Adobe Photoshop, Chrome, Zoom, Game

---

### 8. Hubungan Hardware dan Software

```
┌─────────────────────────────────────┐
│              USER                   │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│      SYSTEM AND APPLICATION         │
│           PROGRAMS                  │
│  (Compiler, Text Editor, Database)  │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│        OPERATING SYSTEM             │
└─────────────────────────────────────┘
                 ↓↑
┌─────────────────────────────────────┐
│       COMPUTER HARDWARE             │
└─────────────────────────────────────┘
```

**Poin Penting:**
- User berinteraksi dengan Applications
- Applications meminta resources dari OS
- OS berinteraksi dengan Hardware
- OS = **jembatan** antara aplikasi dan hardware

---

### 9. Lisensi Software (Wajib Hafal!)

| Jenis | Biaya | Hak Cipta | Modifikasi | Contoh |
|-------|-------|-----------|------------|--------|
| **Freeware** | Gratis | Ada batasan | Tidak boleh | WhatsApp, Instagram, Facebook |
| **Shareware** | Gratis (trial) | Ada batasan | Tidak boleh | VPN trial, VivaVideo |
| **Proprietary** | Bayar | Dilindungi | Tidak boleh | MS Office, Photoshop, CorelDraw |
| **Open Source** | Gratis | Bebas | Boleh | Linux, LibreOffice, GIMP |

**Penjelasan Detail:**

**Freeware:**
- Dapat digunakan **tanpa biaya**
- Masih ada **batasan hak cipta**
- Tidak boleh dimodifikasi

**Shareware:**
- Gratis dalam **jangka waktu tertentu** (trial)
- Setelah masa trial, harus bayar atau berhenti
- Contoh: Aplikasi dengan "Free 3-day trial"

**Proprietary Software:**
- **Harus membeli** untuk menggunakan
- Tidak boleh mendistribusikan ulang
- Kode **tidak open for public**

**Open Source Software:**
- **Bebas** digunakan, diubah, dan didistribusikan
- Kode tersedia untuk publik
- Biasanya untuk tujuan sosial

---

## Perbedaan yang Sering Membingungkan

### Hardware vs Software

| Aspek | Hardware | Software |
|-------|----------|----------|
| Sifat | Fisik, bisa disentuh | Non-fisik, instruksi |
| Analogi | Tubuh/raga | Jiwa/pikiran |
| Contoh | CPU, RAM, Monitor | Windows, Chrome, Word |
| Kerusakan | Aus, rusak fisik | Usang, bug |

### Sistem Operasi vs Program Aplikasi

| Aspek | Sistem Operasi | Program Aplikasi |
|-------|----------------|------------------|
| Fungsi | Mengelola seluruh sistem | Pekerjaan spesifik |
| Keharusan | **Wajib ada** | Opsional/tambahan |
| Contoh | Windows, Android | Word, Chrome |
| Posisi | Penerjemah HW-SW | Di atas OS |

### Program Utilitas vs Program Aplikasi

| Aspek | Program Utilitas | Program Aplikasi |
|-------|------------------|------------------|
| Fungsi | Memelihara/optimasi sistem | Membantu pekerjaan user |
| Target | Hardware, OS, sistem | Kebutuhan user |
| Contoh | Antivirus, Disk Cleanup | Word, Photoshop |

### Freeware vs Open Source

| Aspek | Freeware | Open Source |
|-------|----------|-------------|
| Biaya | Gratis | Gratis |
| Modifikasi | **Tidak boleh** | **Boleh** |
| Kode | Tertutup | Terbuka |
| Distribusi | Terbatas | Bebas |

---

## Tips Menjawab Soal

### Cara Ingat 4 Jenis Software: "SO-BA-UTI-APP"
- **S**istem **O**perasi
- **BA**hasa Pemrograman
- Program **UTI**litas
- Program **APP**likasi

### Cara Ingat 4 Jenis Lisensi: "FREE-SHARE-PRO-OPEN"
- **FREE**ware - Gratis, ada batasan
- **SHARE**ware - Trial/gratis sementara
- **PRO**prietary - Bayar, tidak boleh modifikasi
- **OPEN** Source - Gratis, bebas modifikasi

### Keyword Identifikasi

**Sistem Operasi:**
- Penerjemah HW-SW
- Mengatur sistem kerja
- Windows, macOS, Linux, Android

**Program Utilitas:**
- Memelihara, optimasi
- Antivirus, backup, cleanup

**Program Aplikasi:**
- Siap pakai
- Pekerjaan spesifik user

---

## Contoh Soal Latihan

### Soal 1: Pilihan Ganda
**Software yang berfungsi sebagai penerjemah antara hardware dan software adalah?**

a) Program Aplikasi
b) Program Utilitas
c) Sistem Operasi
d) Bahasa Pemrograman

> **Jawaban: C** - Sistem Operasi berfungsi sebagai penerjemah antara HW dan SW

---

### Soal 2: Pilihan Ganda
**Manakah yang termasuk Program Utilitas?**

a) Microsoft Word
b) Antivirus
c) Windows
d) Python

> **Jawaban: B** - Antivirus adalah program utilitas untuk memelihara keamanan komputer

---

### Soal 3: Pilihan Ganda
**Software yang bisa digunakan gratis dalam jangka waktu tertentu (trial) disebut?**

a) Freeware
b) Shareware
c) Proprietary
d) Open Source

> **Jawaban: B** - Shareware = gratis dalam jangka waktu tertentu

---

### Soal 4: Pilihan Ganda
**Perbedaan utama antara Freeware dan Open Source adalah?**

a) Freeware berbayar, Open Source gratis
b) Freeware tidak boleh dimodifikasi, Open Source boleh
c) Freeware untuk bisnis, Open Source untuk sosial
d) Tidak ada perbedaan

> **Jawaban: B** - Freeware tidak boleh dimodifikasi, Open Source boleh dimodifikasi

---

### Soal 5: Essay
**Sebutkan dan jelaskan 4 jenis software pada komputer!**

> **Jawaban:**
> 1. **Sistem Operasi** - Program yang mengatur sistem kerja komputer dan menjadi penerjemah antara HW dan SW. Contoh: Windows, macOS, Linux
> 2. **Bahasa Pemrograman** - Instruksi dan tools untuk memfasilitasi penulisan, pengujian, dan eksekusi program. Contoh: Python, Java
> 3. **Program Utilitas** - Software untuk mengelola, mengoptimalkan, dan memelihara komputer. Contoh: Antivirus, Disk Cleanup
> 4. **Program Aplikasi** - Software siap pakai untuk membantu pekerjaan spesifik user. Contoh: MS Office, Photoshop

---

### Soal 6: Essay
**Jelaskan perbedaan 4 jenis lisensi software!**

> **Jawaban:**
>
> | Jenis | Penjelasan |
> |-------|------------|
> | **Freeware** | Gratis digunakan tapi ada batasan hak cipta, tidak boleh dimodifikasi |
> | **Shareware** | Gratis dalam jangka waktu tertentu (trial), setelah itu harus bayar |
> | **Proprietary** | Harus membeli, tidak boleh mendistribusikan ulang atau memodifikasi |
> | **Open Source** | Bebas digunakan, diubah, dan didistribusikan kembali |

---

## Quick Recall (Hafalan Cepat)

- **Software** = pikiran/jiwa komputer, instruksi untuk hardware
- **4 Jenis SW** = Sistem Operasi, Bahasa Pemrograman, Program Utilitas, Program Aplikasi
- **Sistem Operasi** = penerjemah HW-SW (Windows, macOS, Linux)
- **Program Utilitas** = memelihara sistem (Antivirus, Backup)
- **Program Aplikasi** = siap pakai untuk user (Word, Chrome)
- **4 Jenis Lisensi** = Freeware, Shareware, Proprietary, Open Source
- **Open Source** = satu-satunya yang boleh dimodifikasi
- **Shareware** = gratis tapi ada masa trial

---

## Koneksi dengan CBIS

Software adalah salah satu dari **5 elemen CBIS**:
1. People
2. Data
3. Hardware
4. **Software** ← Sesi ini!
5. Telecommunications

---

*Sumber: Slide PTSI Sesi 5 - Perangkat Lunak (Software), Universitas Siber Asia*
