# EPIC-000 Pengelolaan Transaksi Pembelian - Ajay ganteng hari ini

## Tujuan Epic

### Tujuan Utama

Membangun modul baru untuk menstandarkan pencatatan transaksi pembelian barang dan jasa dalam satu sumber data utama agar proses pencatatan lebih konsisten dan pelaporan pembelian serta hutang vendor menjadi lebih cepat dan andal.

### Hasil yang Ingin Dicapai

**Standardisasi Pencatatan**

- Tersedia alur input transaksi pembelian yang seragam di dalam aplikasi.
- Pencatatan transaksi barang dan jasa mengikuti aturan input yang sesuai dengan kebutuhan masing-masing.

**Konsolidasi Data**

- Data transaksi pembelian tidak lagi tersebar di banyak file dan memiliki satu sumber data utama.
- Data transaksi lebih konsisten dan lebih mudah ditelusuri.

**Percepatan Pelaporan**

- Data transaksi pembelian lebih siap digunakan untuk laporan pembelian.
- Data transaksi pembelian lebih siap digunakan untuk monitoring hutang dan vendor payable.
- Waktu penyusunan laporan berkurang dibanding proses manual sebelumnya.

## Indikator Keberhasilan / KPI

| Kategori | Target | Deskripsi | Cara Pengukuran | Waktu Pengukuran | Penanggung Jawab |
| ---------- | ---------- | ---------- | ---------- | ---------- | ---------- |
| Standardisasi pencatatan | 100% transaksi pembelian baru dicatat melalui modul baru | Tidak ada lagi pencatatan transaksi pembelian baru di file Excel terpisah | Audit sumber pencatatan transaksi pembelian | 1 bulan setelah go-live | Finance / Accounting |
| Konsistensi data | Minimal 90% transaksi pembelian memenuhi format data wajib yang ditetapkan | Data transaksi pembelian tercatat dengan field utama yang lengkap dan seragam | Audit kelengkapan data pada transaksi yang diinput | 1 bulan setelah go-live | Finance / Accounting |
| Kecepatan pelaporan | Waktu penyusunan laporan pembelian dan hutang vendor berkurang minimal 50% dibanding proses manual sebelumnya | Proses penyusunan laporan menjadi lebih cepat karena data sudah terpusat dan lebih rapi | Perbandingan waktu penyusunan laporan sebelum dan sesudah implementasi | 1 sampai 2 siklus pelaporan setelah go-live | Finance / Accounting |

## Scope

### In Scope

- Membangun modul baru untuk pencatatan transaksi pembelian barang dan jasa.
- Menyediakan standar input transaksi pembelian yang seragam di dalam aplikasi sebagai pengganti pencatatan manual di Excel.
- Menyimpan data transaksi pembelian dalam satu sumber data utama agar tidak tersebar di banyak file.
- Mendukung input transaksi dari invoice vendor beserta detail penting seperti vendor, nominal, pajak, jatuh tempo, dan informasi yang relevan untuk pembelian.
- Membedakan aturan input transaksi pembelian barang dan jasa sesuai kebutuhan datanya masing-masing.
- Mendukung pelaporan pembelian operasional berdasarkan data transaksi yang tercatat.
- Mendukung pelaporan hutang dan vendor payable berdasarkan transaksi pembelian yang sudah diinput.
- Menyediakan validasi dasar saat pencatatan agar data lebih konsisten dan siap dipakai untuk pelaporan.

### Planned Features

| Fitur | Deskripsi | Kapan Akan Dikerjakan |
| ------- | --------------------------------------- | --------------------------- |
| Approval transaksi pembelian | Proses existing belum memiliki approval, jadi belum perlu masuk tahap awal | Setelah alur pencatatan inti stabil |
| Otomasi pembacaan invoice | Ekstraksi otomatis dari dokumen invoice belum wajib untuk tahap awal | Fase lanjutan |
| Dashboard analitik pembelian lanjutan | Fokus awal adalah pencatatan dan pelaporan operasional inti lebih dulu | Fase lanjutan |

### Out of Scope

| Out of Scope | Catatan |
| --------------------------- | ----------------------------------------------------- |
| Proses procurement dari permintaan sampai purchase order | Epic dimulai dari invoice vendor, bukan dari proses pengadaan awal |
| Proses pembayaran ke vendor | Bisa diarahkan ke epic account payable payment process bila nanti dibutuhkan |
| Standardisasi format invoice dari vendor | Standardisasi dilakukan di aplikasi internal, bukan dengan mengubah format dari vendor |
| Laporan keuangan menyeluruh di luar area pembelian dan hutang | Epic ini fokus pada transaksi pembelian, hutang, dan vendor payable |
