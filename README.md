# UMKM Sales Dashboard (Excel)

Dashboard penjualan interaktif untuk UMKM alat tulis kantor (ATK), dibuat dengan Microsoft Excel. Dashboard ini membantu manajemen melihat kinerja penjualan dalam satu halaman.

<img width="802" height="687" alt="image" src="https://github.com/user-attachments/assets/131657b5-45eb-467c-8d37-dc7716965366" />

## Tujuan Analisis

1. Bagaimana kinerja penjualan secara keseluruhan dan dari bulan ke bulan?
2. Produk apa yang paling menyumbang penjualan?
3. Kota mana yang paling banyak bertransaksi?
4. Metode pembayaran apa yang paling sering dipakai?
5. Bisakah manajemen memfilter semua hal di atas dalam satu halaman?

## Tentang Proyek

- **Data:** 10.005 transaksi, Januari 2022 – Juni 2025
- **Alat:** Microsoft Excel (PivotTable, PivotChart, Slicer, Timeline)

## Langkah Pengerjaan

1. **Persiapan data:** muat data transaksi mentah ke sheet `Data`.
2. **Pemeriksaan dan pembersihan:** cek nilai kosong, duplikat, tipe kolom (tanggal, angka), dan penulisan nama produk, kota, serta status.
3. **Pembuatan PivotTable:** satu PivotTable per ukuran di sheet `Pivot` (penjualan bulanan, metode pembayaran, transaksi per kota, penjualan per produk).
4. **Pembuatan PivotChart:** ubah tiap PivotTable menjadi grafik.
5. **Pembuatan KPI:** Total Transaksi, Kuantitas, Total Sales, dan Grand Total.
6. **Filter interaktif:** pasang Slicer (Produk, Metode Pembayaran, Kota) dan Timeline (Tanggal), lalu hubungkan ke semua PivotTable.
7. **Penyusunan tampilan:** susun KPI, grafik, dan filter di sheet `Dashboard`.

> ⚠️ Langkah di atas disusun dari isi README. Sesuaikan dengan proses yang benar-benar Anda lakukan.

## Isi Dashboard

- **KPI:** Total Transaksi (10.005), Kuantitas (30.060), Total Sales (Rp647,4 juta), Grand Total (Rp935,7 juta)
- **Grafik:** tren penjualan bulanan, distribusi metode pembayaran, transaksi per kota, penjualan per produk
- **Filter interaktif:** Produk, Metode Pembayaran, Kota, dan Tanggal (Timeline)

## Insight dan Rekomendasi

### 1. Kontribusi Produk terhadap Penjualan
<img width="363" height="375" alt="image" src="https://github.com/user-attachments/assets/bfec7dfd-10bf-43a8-9f74-5929b557b603" />

| Produk | Kontribusi penjualan |
|---|---|
| Kalkulator Casio | 48,39% |
| Kertas HVS A4 70gsm 500lbr | 17,93% |
| Binder A5 | 7,54% |

- **Insight:** Kalkulator Casio menyumbang 48,39% penjualan (Rp313,3 juta), padahal hanya 6,3% dari jumlah transaksi. Harganya Rp175.000, jauh di atas sebagian besar produk lain (di bawah Rp30.000). Bersama Kertas HVS A4, dua produk ini menyumbang ±66% penjualan.
- **Rekomendasi:** Jaga stok Kalkulator Casio agar tidak kosong, dan negosiasikan harga beli dengan pemasok. Dorong produk murah dengan transaksi banyak lewat bundling (misalnya paket kertas + binder) agar tidak bergantung pada satu produk.

### 2. Transaksi per Kota
- **Insight:** Denpasar dan Surabaya adalah kota dengan transaksi terbanyak.
- **Rekomendasi:** Prioritaskan stok dan promosi di dua kota ini. Cari tahu mengapa kota lain tertinggal, apakah karena pasar yang kecil atau jangkauan yang kurang.

### 3. Metode Pembayaran
- **Insight:** Transfer paling sering dipakai (4.007 transaksi).
- **Rekomendasi:** Pastikan proses transfer lancar dan konfirmasi pembayarannya cepat. Pertimbangkan insentif kecil untuk metode yang paling mudah dicatat.

### 4. Tren Penjualan Bulanan
- **Insight:** Penjualan tertinggi pada Maret, terendah pada Juli dan September.
- **Rekomendasi:** Siapkan stok lebih banyak menjelang Maret. Buat promo atau penawaran khusus di Juli dan September untuk mengisi bulan sepi.

**Catatan:** angka dihitung dari seluruh status pesanan (Completed, Pending, Canceled, Return). Untuk hasil yang lebih akurat, bandingkan juga dengan hanya status Completed.

## Cara Menggunakan

1. Unduh `dashboard_interaktif.xlsx`.
2. Buka di Microsoft Excel 2013 atau lebih baru.
3. Buka sheet `Dashboard`, lalu gunakan slicer dan timeline untuk memfilter data.

## Struktur File

| Sheet | Isi |
|---|---|
| Data | Data transaksi mentah |
| Dashboard | Tampilan utama (KPI, grafik, filter) |
| Pivot | PivotTable sumber grafik |

---

Zulkifli H · 123kifri622@gmail.com
