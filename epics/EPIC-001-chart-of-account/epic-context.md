# Epic Context: Chart of Account

## Status
Draft eksplorasi awal level epic.

## Ringkasan Epic
Epic ini berfokus pada pembentukan Chart of Account sebagai master akun awal di aplikasi accounting. Pada tahap sekarang, fokusnya masih pada setup dan pengelolaan master akun, dengan arah ke depan agar struktur akun ini dapat dipakai oleh modul lain seperti transaksi.

## Aktor Terdampak
- Admin Keuangan
- Owner

## Business Process Diagram
Kondisi saat ini masih as-is dan dikelola di Excel.

```mermaid
flowchart TD
  subgraph Owner["Owner"]
    O1["Memberi arahan kebutuhan struktur akun bila diperlukan"]
    O2["Melihat atau mengecek daftar akun"]
  end

  subgraph Finance["Admin Keuangan"]
    F1["Menyusun dan memelihara Chart of Account di Excel"]
    F2["Menentukan kode akun, nama akun, kategori, dan kelompok akun"]
    F3["Menambah, mengubah, atau merapikan akun di file Excel"]
    F4["Mengecek konsistensi struktur akun secara manual"]
    F5["Membagikan file Excel sebagai referensi master akun"]
  end

  subgraph Ops["Penggunaan Operasional"]
    U1["Tim menggunakan file Excel sebagai acuan saat dibutuhkan"]
    U2["Versi file bisa berbeda antar pengguna atau kebutuhan"]
  end

  O1 --> F1
  O2 --> F5
  F1 --> F2 --> F3 --> F4 --> F5
  F5 --> U1 --> U2
```

## Asumsi yang Sudah Disepakati
- Pengelolaan COA saat ini masih dilakukan di Excel.
- Tidak ada approval formal saat akun ditambah atau diubah.
- Struktur akun saat ini belum baku.
- Kadang ada beberapa versi file COA yang beredar.
- Fokus epic saat ini adalah setup master akun terlebih dahulu.
- COA disiapkan agar nantinya dapat dipakai oleh modul lain.

## Catatan Lanjutan
Section berikutnya yang perlu disusun adalah Problem Statement, lalu Tujuan Epic, KPI, Scope, dan artefak lanjutan lain sesuai alur eksplorasi epic.
