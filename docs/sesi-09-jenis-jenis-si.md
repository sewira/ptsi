# Sesi 9: Jenis-Jenis Sistem Informasi

## 📋 Big Picture

Sistem informasi dalam organisasi bukan "one size fits all" - setiap level manajemen dan departemen punya kebutuhan berbeda:

1. **Struktur Piramida Organisasi** - Sistem informasi dirancang mengikuti hierarki organisasi: dari operasional (bawah) hingga strategis (puncak)
2. **Area Fungsional** - Setiap departemen (Sales, Finance, HR, Manufacturing, Accounting) punya SI spesialisasi sendiri
3. **Level Keputusan Berbeda** - Semakin tinggi level, semakin tidak terstruktur keputusannya (TPS = rutin, ESS = strategis)
4. **Integrasi Data** - Sistem di level bawah jadi "bahan baku" untuk sistem di level atas (TPS → MIS → DSS → ESS)
5. **Knowledge Workers** - Ada lapisan khusus untuk pekerja pengetahuan (engineer, designer) dengan sistem KMS dan OAS

**Analogi Sederhana**: Bayangkan organisasi seperti restoran:
- **TPS** = Kasir yang catat pesanan (transaksi harian)
- **MIS** = Manajer shift yang lihat laporan penjualan harian
- **DSS** = Chef yang analisis menu mana yang laris, harus ganti resep atau tidak
- **ESS** = Owner yang putuskan buka cabang baru atau tidak

---

## 🎯 Konsep Kunci

### 1. Transaction Processing System (TPS)

**Definisi**: Sistem untuk mencatat dan memproses transaksi rutin harian di level operasional.

**Karakteristik Wajib Hafal!**:
- Level: **Operasional** (bawah piramida)
- Fungsi: Otomatisasi tugas rutin dan berulang
- Output: Data transaksi detail untuk arsip
- Sifat: **Real-time** atau **batch processing**

**Contoh Konkret**:
| Sistem | Fungsi |
|--------|--------|
| **POS (Point of Sale)** | Catat penjualan di kasir (Alfamart, Indomaret) |
| **Payroll System** | Hitung gaji karyawan otomatis |
| **A/R, A/P, GL** | Account Receivable (piutang), Account Payable (hutang), General Ledger (buku besar) |
| **Order Processing** | Proses pesanan pelanggan (Tokopedia, Shopee) |
| **Inventory System** | Catat keluar-masuk barang gudang |

**Real-World Example**:
- **Gojek/Grab**: Setiap kali driver terima orderan, itu dicatat di TPS mereka
- **BCA Mobile**: Transfer uang = transaksi yang diproses TPS
- **BPJS Kesehatan**: Setiap klaim pasien dicatat di TPS

**IPO (Input-Process-Output)**:
```
INPUT                    PROCESS                     OUTPUT
Time cards          →    Calculating pay        →    Paychecks
Employee lists      →    Calculate benefits     →    Receipts
Wages & salary data →    Calculate taxes        →    Account balances
                         Update databases            Reports
```

---

### 2. Knowledge Management System (KMS)

**Definisi**: Sistem untuk menemukan, mengembangkan, dan mengintegrasikan pengetahuan (internal + external) bagi knowledge workers.

**Karakteristik**:
- Level: **Knowledge Level** (Data Workers + Office Workers)
- Fungsi: Advisor untuk manajemen puncak & menengah
- Tools: Search engine, expert system, web-based aid, data management

**Perbedaan Knowledge Workers vs Office Workers**:
| Knowledge Workers | Office Workers |
|-------------------|----------------|
| Engineer, Designer, Scientist | Secretary, Admin |
| Buat pengetahuan baru | Kelola dokumen & komunikasi |
| Contoh: CAD software, simulation | Contoh: Word processing, email |

**Contoh Aplikasi**:
- **Confluence (Atlassian)**: Wiki untuk dokumentasi tim engineering
- **Notion**: Knowledge base untuk perusahaan startup
- **Microsoft SharePoint**: Document management untuk korporat
- **Jupyter Notebook**: Data scientist analisis data

**Real-World**:
- Perusahaan seperti **Google** dan **Meta** pakai internal wiki untuk share pengetahuan antar engineer
- **Stack Overflow** untuk programmer = eksternal KMS

---

### 3. Management Information System (MIS)

**Definisi**: Sistem yang menghasilkan **laporan berkala** untuk mendukung keputusan rutin terstruktur di level manajemen menengah.

**Karakteristik**:
- Level: **Manajemen Menengah** (Middle Managers)
- Fungsi: Akses, atur, ringkas, tampilkan info untuk keputusan rutin
- Output: **Scheduled reports**, **Ad hoc reports**, **Exception reports**
- Sifat keputusan: **Semi-terstruktur**

**Contoh Laporan MIS**:
| Laporan | Deskripsi | Frekuensi |
|---------|-----------|-----------|
| Sales Management Report | Penjualan per region | Mingguan/Bulanan |
| Inventory Control | Stok barang & reorder point | Harian/Mingguan |
| Annual Budget vs Actual | Perbandingan anggaran vs realisasi | Bulanan |
| Production Scheduling | Jadwal produksi pabrik | Mingguan |

**Real-World**:
- **SAP**: ERP yang punya modul MIS untuk berbagai departemen
- **Odoo**: Open-source ERP dengan laporan MIS
- **Tableau/Power BI**: Visualisasi laporan MIS dalam dashboard

**Perbedaan dengan TPS**:
```
TPS                           MIS
Data detail transaksi    →    Data ringkasan/agregat
Real-time/Harian         →    Berkala (mingguan/bulanan)
Untuk operator           →    Untuk manajer
```

---

### 4. Decision Support System (DSS)

**Definisi**: Sistem untuk mendukung keputusan **kompleks yang tidak rutin** dengan analisis skenario dan simulasi.

**Karakteristik**:
- Level: **Manajemen Taktis** (Middle Managers)
- Fungsi: Analisis **what-if**, simulasi, optimasi
- Sifat keputusan: **Tidak terstruktur/semi-terstruktur**
- Metodologi: Mathematical modeling, OLAP, data mining, simulation

**Perbedaan MIS vs DSS**:
| Aspek | MIS | DSS |
|-------|-----|-----|
| **Keputusan** | Rutin, terstruktur | Kompleks, tidak rutin |
| **Output** | Laporan tetap | Analisis interaktif |
| **Contoh** | "Berapa penjualan bulan ini?" | "Bagaimana jika kita turunkan harga 10%?" |
| **Tool** | Reporting | Simulation, what-if analysis |

**Metodologi DSS**:
1. **Mathematical Modeling**: Optimasi dengan rumus matematika (linear programming)
2. **OLAP (Online Analytical Processing)**: Analisis multidimensi (sales by region by product by time)
3. **Data Mining**: Temukan pola tersembunyi dari data besar
4. **Simulation**: Simulasi skenario bisnis

**Contoh Konkret**:
- **Pricing Analysis**: "Kalau harga naik 5%, profit berapa? Demand turun berapa?"
- **Production Scheduling**: "Kalau tambah shift malam, cost vs benefit-nya gimana?"
- **Investment Analysis**: "Invest di mesin baru atau expand ke pasar baru?"

**Real-World**:
- **Google Analytics**: Analisis traffic website dengan berbagai skenario
- **Amazon**: DSS untuk pricing dinamis (harga berubah real-time)
- **Airline**: Yield management system untuk optimasi harga tiket

---

### 5. Executive Support System (ESS)

**Definisi**: Sistem untuk mendukung keputusan **strategis** di level senior management yang dapat mengubah cara bisnis dijalankan.

**Karakteristik**:
- Level: **Manajemen Strategis** (Senior/Top Management)
- Fungsi: Strategic planning jangka panjang (5 tahun)
- Input: Data dari TPS, MIS, DSS + **External Information** (ekonomi, kompetitor)
- Output: 5-year sales trend, profit planning, product development

**Perbedaan dengan Sistem Lain**:
```
ESS: "Apakah kita harus pivot bisnis model?"
DSS: "Strategi mana yang paling optimal?"
MIS: "Bagaimana performa bulan ini?"
TPS: "Berapa transaksi hari ini?"
```

**Contoh Keputusan ESS**:
- Merger & Acquisition (beli perusahaan lain?)
- Ekspansi geografis (buka kantor di negara lain?)
- Pivot produk (ganti model bisnis?)
- Investment besar (bangun pabrik baru?)

**Real-World**:
- **CEO Dashboard**: Gabungan metrik dari semua sistem
- **Bloomberg Terminal**: Data pasar finansial untuk eksekutif
- **Gojek Super App Strategy**: Keputusan diversifikasi dari transport ke fintech

**Flow Data ke ESS**:
```
Transaction Processes → MIS → DSS → ESS
                                 ↗
External Information (market, economy)
Data Warehouse
```

---

### 6. Sistem Informasi Fungsional

**Definisi**: SI dengan **spesialisasi fungsi** yang fokus pada departemen/unit kerja tertentu.

**5 Area Fungsional Utama**:

#### A. **Sales & Marketing**
- Identify potential customers
- Define customer wants & needs
- Identify market opportunities
- Make customers aware & persuade to buy
- Perform sales transaction

**Contoh Sistem**: CRM (Customer Relationship Management) seperti Salesforce, HubSpot

#### B. **Manufacturing/Production**
- Purchasing materials
- Assembling/fabricating product
- Delivering product
- Servicing product & supporting customer

**Contoh**: ERP Manufacturing Module, SAP Production Planning

#### C. **Accounting & Finance**
- Financial transactions
- Financial statements
- Paying taxes
- Investing cash
- Financing operations

**Contoh**: Accounting software (Accurate, Zahir, QuickBooks)

#### D. **Human Resources**
- Determining hiring requirements
- Hiring people
- Training & development
- Paying employees
- Administering benefits
- Disciplinary actions & terminations

**Contoh**: HRIS (Talenta, Mekari, BambooHR)

#### E. **Engineering**
- Research about new methods
- Determine how to produce products
- Determine how to improve production

**Contoh**: CAD software (AutoCAD), PLM (Product Lifecycle Management)

**Karakteristik SI Fungsional**:
- **Data**: Terperinci DAN ringkas
- **Update**: Banyak pembaruan kecil & rutin
- **Kualitas Info**: TARL + Ringkas
  - **T**epat waktu
  - **A**kurat
  - **R**elevan
  - **L**engkap
  - **Ringkas**

**Business Processes Requiring Coordination**:
- Creating new product (butuh Engineering + Marketing + Finance)
- Creating coordinated plan (butuh semua departemen)
- Fulfilling customer orders (butuh Sales + Manufacturing + Finance)

---

## ⚖️ Perbedaan yang Sering Membingungkan

### 1. TPS vs MIS vs DSS vs ESS

| Aspek | TPS | MIS | DSS | ESS |
|-------|-----|-----|-----|-----|
| **Level** | Operasional | Menengah | Menengah-Taktis | Strategis |
| **User** | Operational Managers | Middle Managers | Middle Managers | Senior Managers |
| **Keputusan** | Rutin harian | Rutin berkala | Kompleks, analitik | Strategic, long-term |
| **Output** | Detail transaksi | Laporan ringkasan | Simulasi, what-if | Trend, forecasting |
| **Contoh** | POS, Payroll | Sales report bulanan | Pricing optimization | 5-year business plan |
| **Sifat** | Terstruktur | Semi-terstruktur | Tidak terstruktur | Sangat tidak terstruktur |

### 2. KMS vs OAS (Office Automation System)

| Aspek | KMS | OAS |
|-------|-----|-----|
| **User** | Knowledge Workers | Office Workers |
| **Fungsi** | Ciptakan pengetahuan baru | Kelola dokumen & komunikasi |
| **Contoh** | CAD, Simulation, Expert System | Word, Email, Calendar |
| **Output** | Design, Research, Innovation | Documents, Reports, Schedules |

### 3. SI Fungsional vs SI Level Manajemen

| SI Fungsional | SI Level Manajemen |
|---------------|-------------------|
| Berdasarkan **departemen** (HR, Finance, Marketing) | Berdasarkan **level organisasi** (Operasional, Taktis, Strategis) |
| **Horizontal** (across departments) | **Vertical** (across levels) |
| Fokus pada **area bisnis spesifik** | Fokus pada **tipe keputusan** |

**Fun Fact**: Dalam praktik, sebuah sistem bisa masuk ke KEDUA kategori sekaligus! Contoh: "HR MIS" = SI Fungsional (HR) + SI Level Manajemen (MIS).

---

## 💡 Tips Menjawab Soal

### Akronim: **TKMD-ESS**
- **T**PS = Transaksi
- **K**MS = Knowledge
- **M**IS = Management reports
- **D**SS = Decision analysis
- **ESS** = Executive Strategic

### Keyword Identifikasi

**Kalau soal bilang...**  →  **Jawabannya:**

| Keyword Soal | Sistem |
|--------------|--------|
| "Transaksi harian", "POS", "Payroll", "Order processing" | **TPS** |
| "Laporan bulanan", "Scheduled report", "Inventory control" | **MIS** |
| "What-if analysis", "Simulasi", "Pricing analysis", "OLAP" | **DSS** |
| "5-year plan", "Strategic decision", "Merger", "Expand" | **ESS** |
| "Knowledge workers", "Expert system", "External + Internal content" | **KMS** |
| "Departemen HR/Finance/Marketing" | **SI Fungsional** |

### Tips Hafalan Piramida

```
        ESS (Senior) ← Strategic (5 tahun)
       /   \
     DSS   MIS (Middle) ← Tactical (analisis)
     /       \
   KMS      OAS (Data/Office Workers) ← Knowledge
    \         /
      TPS (Operational) ← Daily transactions
```

**Mnemonik Level**: **O-K-T-S**
- **O**perational (TPS)
- **K**nowledge (KMS/OAS)
- **T**actical (MIS/DSS)
- **S**trategic (ESS)

### Common Mistakes yang Sering Dilakukan

❌ **Salah**: "MIS buat keputusan strategis"
✅ **Benar**: MIS untuk keputusan **rutin terstruktur**, ESS untuk strategis

❌ **Salah**: "TPS menghasilkan laporan untuk manajemen"
✅ **Benar**: TPS **menyimpan data transaksi**, MIS yang **buat laporan** dari data TPS

❌ **Salah**: "DSS sama dengan ESS"
✅ **Benar**: DSS = tactical/middle level, ESS = strategic/top level

❌ **Salah**: "SI Fungsional hanya untuk satu departemen"
✅ **Benar**: Beberapa proses butuh **koordinasi antar departemen** (cross-functional)

---

## 📝 Contoh Soal Latihan

### A. Pilihan Ganda

**Soal 1:**
Sistem yang digunakan kasir Indomaret untuk mencatat penjualan setiap pelanggan termasuk jenis sistem informasi...

A. Management Information System
B. Transaction Processing System
C. Decision Support System
D. Executive Support System

**Jawaban: B. Transaction Processing System**
**Penjelasan**: Keyword "kasir", "mencatat penjualan" = transaksi rutin harian = TPS. Indomaret POS adalah contoh klasik TPS.

---

**Soal 2:**
Manajer produksi ingin menganalisis: "Bagaimana jika kita tambah shift malam, apakah cost-nya worth it dengan peningkatan output?" Sistem yang tepat adalah...

A. TPS
B. MIS
C. DSS
D. KMS

**Jawaban: C. DSS (Decision Support System)**
**Penjelasan**: Keyword "what-if analysis", "simulasi skenario" = DSS. Ini keputusan kompleks yang butuh analisis, bukan laporan rutin.

---

**Soal 3:**
CEO Gojek ingin memutuskan apakah expand bisnis ke Vietnam atau tidak, dengan analisis ekonomi, kompetitor, dan tren 5 tahun. Sistem yang mendukung adalah...

A. MIS
B. DSS
C. ESS
D. TPS

**Jawaban: C. ESS (Executive Support System)**
**Penjelasan**: Keyword "CEO", "strategic decision", "expand", "5 tahun" = ESS. Ini keputusan strategis yang mengubah cara bisnis dijalankan.

---

**Soal 4:**
Sistem yang membantu engineer menggunakan CAD untuk design produk baru termasuk kategori...

A. TPS
B. KMS (Knowledge Management System)
C. MIS
D. ESS

**Jawaban: B. KMS**
**Penjelasan**: Keyword "engineer", "design" = knowledge worker. CAD adalah tool untuk create new knowledge/product.

---

**Soal 5:**
Laporan penjualan bulanan yang membandingkan target vs realisasi untuk manajer penjualan dihasilkan oleh sistem...

A. TPS
B. MIS
C. DSS
D. ESS

**Jawaban: B. MIS**
**Penjelasan**: Keyword "laporan berkala (bulanan)", "manajer", "perbandingan" = MIS. Ini scheduled report untuk keputusan rutin.

---

**Soal 6:**
Berikut ini yang BUKAN termasuk area fungsional utama dalam organisasi adalah...

A. Sales & Marketing
B. Transaction Processing
C. Human Resources
D. Manufacturing

**Jawaban: B. Transaction Processing**
**Penjelasan**: TPS adalah **jenis SI berdasarkan level**, bukan **area fungsional**. Area fungsional: Sales, HR, Finance, Manufacturing, Accounting.

---

**Soal 7:**
Karakteristik informasi yang dihasilkan SI Fungsional harus memenuhi kriteria TARL, yaitu...

A. Transparan, Akurat, Relevan, Lengkap
B. Tepat waktu, Akurat, Relevan, Lengkap
C. Tepat waktu, Aman, Relevan, Lengkap
D. Transparan, Aman, Relevan, Logis

**Jawaban: B. Tepat waktu, Akurat, Relevan, Lengkap**
**Penjelasan**: **Wajib hafal!** TARL = **T**epat waktu, **A**kurat, **R**elevan, **L**engkap (+Ringkas).

---

**Soal 8:**
Data yang digunakan ESS berasal dari...

A. Hanya internal (TPS, MIS, DSS)
B. Hanya external (market data, ekonomi)
C. Internal (TPS, MIS, DSS) + External + Data Warehouse
D. Hanya dari TPS

**Jawaban: C. Internal + External + Data Warehouse**
**Penjelasan**: ESS butuh **comprehensive data** dari berbagai sumber untuk keputusan strategis, termasuk data eksternal (ekonomi, kompetitor).

---

**Soal 9:**
Metodologi yang digunakan DSS mencakup semua KECUALI...

A. Mathematical Modeling
B. OLAP (Online Analytical Processing)
C. Scheduled Reports
D. Data Mining

**Jawaban: C. Scheduled Reports**
**Penjelasan**: Scheduled reports = karakteristik **MIS**, bukan DSS. DSS fokus pada **analisis interaktif** (modeling, OLAP, data mining, simulation).

---

**Soal 10:**
Business process yang membutuhkan koordinasi dari banyak area fungsional adalah...

A. Paying employees
B. Creating a new product
C. Performing sales transaction
D. Analyzing data

**Jawaban: B. Creating a new product**
**Penjelasan**: Buat produk baru butuh **Engineering** (design) + **Marketing** (riset pasar) + **Finance** (budget) + **Manufacturing** (produksi). Ini **cross-functional process**.

---

### B. Essay

**Soal 1:**
Jelaskan perbedaan antara MIS dan DSS, berikan contoh konkret masing-masing!

**Jawaban:**

**Perbedaan MIS dan DSS:**

| Aspek | MIS | DSS |
|-------|-----|-----|
| **Tipe Keputusan** | Rutin, terstruktur | Kompleks, tidak terstruktur |
| **Output** | Laporan tetap berkala | Analisis interaktif, simulasi |
| **Metodologi** | Aggregation, Summarization | Modeling, What-if, Simulation |
| **User** | Middle managers (rutin) | Middle managers (analitik) |

**Contoh MIS**: Laporan penjualan bulanan yang menampilkan total penjualan per region, perbandingan dengan target, dan tren 3 bulan terakhir. Laporan ini **tetap formatnya** dan keluar **setiap bulan** untuk review manajer.

**Contoh DSS**: Aplikasi pricing analysis yang memungkinkan manajer marketing mensimulasikan: "Jika harga produk X diturunkan 10%, berapa penurunan profit margin? Berapa peningkatan volume penjualan yang dibutuhkan untuk break even?" DSS memberikan **analisis skenario berbeda** sesuai kebutuhan.

**Analogi**: MIS seperti **rapor bulanan** (format tetap), DSS seperti **kalkulator scientific** (bisa hitung berbagai skenario).

---

**Soal 2:**
Mengapa ESS membutuhkan data dari external sources? Berikan contoh external data yang digunakan!

**Jawaban:**

ESS membutuhkan **external data** karena keputusan strategis tidak bisa hanya mengandalkan data internal perusahaan. Senior management harus mempertimbangkan **faktor eksternal** yang dapat mengubah landscape bisnis.

**Alasan butuh external data:**
1. **Market Intelligence**: Tren industri, competitor analysis
2. **Economic Indicators**: Inflasi, GDP, interest rate yang mempengaruhi daya beli
3. **Regulatory Changes**: Perubahan regulasi pemerintah
4. **Technology Trends**: Disrupsi teknologi yang dapat mengancam atau menciptakan peluang

**Contoh external data:**
- **Data ekonomi**: Pertumbuhan ekonomi Indonesia, inflasi, nilai tukar rupiah
- **Data kompetitor**: Market share Tokopedia vs Shopee vs Lazada
- **Data demografi**: Pertumbuhan populasi Gen Z yang suka e-commerce
- **Technology trends**: Adopsi AI, cloud computing di industri retail
- **Social media sentiment**: Persepsi publik terhadap brand

**Contoh kasus**: CEO Bluebird (taksi) harus monitor **data eksternal** tentang adopsi ride-hailing apps (Gojek/Grab) untuk putuskan strategi **digital transformation**, bukan hanya lihat data internal revenue yang turun.

---

**Soal 3:**
Apa perbedaan Knowledge Workers dan Office Workers? Berikan contoh masing-masing dan sistem yang mendukung mereka!

**Jawaban:**

**Knowledge Workers:**
- **Definisi**: Pekerja yang **create new knowledge/products** menggunakan expertise mereka
- **Contoh profesi**: Engineer, Designer, Scientist, Architect, Researcher
- **Sistem pendukung**: KWS (Knowledge Work Systems)
  - CAD (Computer-Aided Design) untuk engineer
  - Simulation software untuk scientist
  - 3D modeling untuk designer
- **Output**: Produk baru, design, research, inovasi

**Office Workers:**
- **Definisi**: Pekerja yang **manage documents and communications**
- **Contoh profesi**: Secretary, Admin, Data entry staff
- **Sistem pendukung**: OAS (Office Automation Systems)
  - Word processing (Microsoft Word, Google Docs)
  - Email (Outlook, Gmail)
  - Calendar & scheduling
  - Desktop publishing
- **Output**: Documents, reports, schedules, communications

**Analogi**:
- Knowledge Worker = **Chef** yang ciptakan resep baru
- Office Worker = **Waiter** yang catat pesanan dan atur jadwal

Keduanya bekerja di **Knowledge Level** dalam piramida SI, tapi dengan fungsi berbeda.

---

**Soal 4:**
Jelaskan konsep "cross-functional business process" dan mengapa penting untuk efisiensi organisasi!

**Jawaban:**

**Cross-functional business process** adalah proses bisnis yang membutuhkan **koordinasi dari banyak departemen/area fungsional** untuk menyelesaikan satu tujuan bisnis.

**Contoh cross-functional processes:**

1. **Fulfilling customer orders**:
   - Sales & Marketing: Terima order dari customer
   - Manufacturing: Produksi barang yang dipesan
   - Finance: Proses pembayaran
   - Accounting: Catat transaksi ke buku besar
   - Human Resources: (jika butuh hiring untuk scale up production)

2. **Creating a new product**:
   - Engineering: Research & design produk
   - Marketing: Riset pasar & customer needs
   - Finance: Budgeting & investment analysis
   - Manufacturing: Produksi & quality control

**Mengapa penting?**
- **Efisiensi**: Koordinasi antar departemen menghindari duplikasi kerja
- **Kecepatan**: Proses paralel lebih cepat daripada sequential
- **Kualitas**: Kolaborasi menghasilkan output lebih baik
- **Customer satisfaction**: Response time lebih cepat

**Masalah jika tidak ada koordinasi (silo mentality)**:
- Marketing janjikan fitur ke customer → Engineering tidak tahu → Customer kecewa
- Production bikin banyak → Marketing tidak ready jual → Inventory menumpuk

**Solusi**: **Integrated Information Systems** (seperti ERP - Enterprise Resource Planning) yang menghubungkan semua departemen dalam satu database terpadu.

**Real-world example**: Amazon fulfillment process yang seamlessly koordinasi dari order (website) → warehouse (pick & pack) → shipping (delivery) → payment (finance).

---

**Soal 5:**
Bandingkan karakteristik informasi yang dihasilkan oleh TPS, MIS, dan ESS dari segi detail, frekuensi, dan pengguna!

**Jawaban:**

| Aspek | TPS | MIS | ESS |
|-------|-----|-----|-----|
| **Detail Data** | Sangat rinci (per transaksi) | Ringkasan/agregat | Highly summarized + trend |
| **Contoh** | "Budi beli Indomie Rp 3.000 pukul 10:05" | "Total penjualan Indomie Rp 50 juta/bulan" | "Tren penjualan mie instan naik 15%/tahun selama 5 tahun" |
| **Frekuensi Update** | Real-time / Harian | Berkala (mingguan/bulanan) | Jarang (quarterly/yearly) |
| **Frekuensi Akses** | Sangat sering (setiap transaksi) | Scheduled (sesuai periode laporan) | On-demand (saat butuh keputusan strategis) |
| **Pengguna** | Operational staff (kasir, admin) | Middle managers | Senior executives (CEO, CFO, COO) |
| **Time Horizon** | Current / Past (hari ini, kemarin) | Recent past (bulan ini, quarter ini) | Long-term (3-5 tahun) |
| **Scope** | Narrow (satu fungsi spesifik) | Departmental | Enterprise-wide + External |
| **Sumber Data** | Internal operational | Internal (dari TPS) | Internal + External + Data Warehouse |
| **Format Output** | Structured data | Structured reports | Dashboards, visualizations, trends |

**Analogi**:
- **TPS** = Buku catatan harian (detail semua kejadian)
- **MIS** = Laporan bulanan (ringkasan poin penting)
- **ESS** = Annual report + business forecast (big picture + future)

**Flow informasi**:
```
TPS (detail) → MIS (summary) → ESS (strategic insights)
```

Data "naik" dari level operasional ke strategis, semakin ringkas tapi semakin strategic value-nya.

---

## 🚀 Quick Recall

### Wajib Hafal!

**Piramida SI (dari bawah ke atas)**:
```
ESS → Senior Managers → Strategic decisions (5-year planning)
DSS/MIS → Middle Managers → Tactical decisions (analysis, reports)
KMS/OAS → Knowledge/Office Workers → Knowledge creation & docs
TPS → Operational Managers → Daily transactions
```

**5 Sistem Utama**:
1. **TPS** = Transaksi harian (POS, Payroll, Order)
2. **KMS** = Knowledge workers (CAD, Expert System, Search)
3. **MIS** = Laporan berkala (Sales report, Inventory control)
4. **DSS** = Analisis kompleks (What-if, Simulation, OLAP)
5. **ESS** = Strategic decisions (5-year plan, M&A, Expansion)

**5 Area Fungsional**:
1. Sales & Marketing
2. Manufacturing/Production
3. Accounting & Finance
4. Human Resources
5. Engineering

**Karakteristik Kualitas Informasi (TARL-R)**:
- **T**epat waktu
- **A**kurat
- **R**elevan
- **L**engkap
- **R**ingkas

**Perbedaan Cepat**:
- **TPS vs MIS**: Detail vs Ringkasan
- **MIS vs DSS**: Laporan rutin vs Analisis kompleks
- **DSS vs ESS**: Tactical vs Strategic
- **KMS vs OAS**: Create knowledge vs Manage docs

**Flow Data**:
```
TPS → MIS → DSS → ESS
       ↘      ↗
     Data Warehouse
          ↑
   External Information
```

**Keyword Soal**:
- "Transaksi", "POS", "Payroll" → **TPS**
- "Laporan bulanan", "Inventory report" → **MIS**
- "What-if", "Simulasi", "Analisis skenario" → **DSS**
- "Strategic", "5-year", "CEO", "Expand" → **ESS**
- "Knowledge worker", "Engineer", "CAD" → **KMS**

**Akronim: O-K-T-S**
- **O**perational → TPS
- **K**nowledge → KMS/OAS
- **T**actical → MIS/DSS
- **S**trategic → ESS

---

## 🔗 Hubungan dengan Materi Lain

**Sesi 2 (CBIS)**: Jenis-jenis SI adalah **implementasi konkret** dari komponen CBIS (Hardware, Software, Data, Procedures, People)

**Sesi 6 (Data & Data Warehouse)**:
- TPS menghasilkan **operational data**
- Data Warehouse menyimpan **historical data** untuk MIS, DSS, ESS

**Sesi 7 (Basis Data)**:
- Semua SI (TPS, MIS, DSS, ESS) mengandalkan **database** sebagai fondasi
- DBMS mendukung query untuk reporting (MIS) dan analysis (DSS)

**Sesi 10 (E-Commerce)**: E-commerce adalah **aplikasi SI** yang menggabungkan TPS (order processing) + MIS (sales report) + DSS (pricing optimization)

**Sesi 11 (SCM)**: Supply Chain Management adalah contoh **cross-functional system** yang koordinasi Manufacturing, Sales, Finance

---

## 🎓 Fun Facts

1. **Istilah "MIS" dulu artinya berbeda**: Di tahun 1960-1970an, "MIS" artinya adalah **semua sistem informasi di perusahaan**. Sekarang artinya lebih spesifik (laporan untuk manajemen).

2. **ESS dulunya butuh dedicated terminal**: Tahun 1980-1990an, eksekutif punya **workstation khusus** untuk ESS (mahal!). Sekarang tinggal buka dashboard di smartphone.

3. **TPS adalah sistem paling "mission-critical"**: Kalau TPS down 1 jam, perusahaan bisa rugi miliaran (contoh: BCA ATM down, Tokopedia error). Kalau ESS down, impact tidak langsung terasa.

4. **Google menggunakan OKR (Objectives & Key Results)** yang didukung ESS untuk track strategic goals. Ini contoh modern ESS di perusahaan tech.

5. **Netflix pricing algorithm** adalah contoh sophisticated DSS yang test ribuan kombinasi harga di berbagai negara.

6. **Gojek/Grab driver allocation** menggunakan **real-time TPS + AI** untuk match driver dengan penumpang dalam hitungan detik.

---

## ✅ Checklist Sebelum Ujian

- [ ] Hafal 5 jenis SI berdasarkan level manajemen (TPS, KMS, MIS, DSS, ESS)
- [ ] Bisa bedakan MIS vs DSS vs ESS
- [ ] Hafal 5 area fungsional (Sales, Manufacturing, Finance, Accounting, HR)
- [ ] Paham karakteristik TARL+Ringkas untuk kualitas informasi
- [ ] Bisa kasih contoh konkret untuk setiap jenis SI
- [ ] Paham konsep cross-functional business process
- [ ] Hafal piramida SI (level + user + output)
- [ ] Tahu flow data dari TPS → MIS → DSS → ESS
- [ ] Bisa bedakan Knowledge Workers vs Office Workers

---

**Prepared by**: Claude Code (AI Assistant)
**Format**: Markdown untuk persiapan ujian PTSI - Universitas Siber Asia
**Last Updated**: 2026-02-01

---

**💪 Semangat belajar! Jangan lupa latihan soal dan diskusi dengan teman untuk memperdalam pemahaman!**
