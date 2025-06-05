# Analisis Data Penjualan Retail dengan Python

Proyek ini berisi serangkaian analisis data penjualan retail menggunakan Python. Analisis dilakukan mulai dari pembersihan data, segmentasi pelanggan, hingga analisis produk favorit dan pola pembelian menggunakan metode Market Basket Analysis. Visualisasi data juga disediakan untuk membantu pemahaman hasil analisis.

---

## Daftar Isi

- [Deskripsi Proyek](#deskripsi-proyek)  
- [Langkah-Langkah Analisis](#langkah-langkah-analisis)  
- [Tools dan Library](#tools-dan-library)  
- [Cara Menjalankan](#cara-menjalankan)  
- [Catatan Penting](#catatan-penting)  

---

## Deskripsi Proyek

Data yang digunakan merupakan transaksi penjualan produk retail yang mencakup informasi seperti nomor faktur, deskripsi produk, kuantitas, harga satuan, dan negara pembeli. Proyek ini bertujuan untuk mengungkap insight terkait produk terlaris, segmentasi pelanggan, dan pola pembelian yang dapat mendukung strategi pemasaran dan peningkatan penjualan.

---

## Langkah-Langkah Analisis

1. **Import dan Persiapan Data**  
   Data diimpor dan dibersihkan dengan menghapus entri yang tidak valid (seperti transaksi dengan kuantitas atau harga ≤ 0). Kolom `TotalPrice` ditambahkan untuk analisis pendapatan produk.

2. **Analisis Produk Terlaris**  
   Mengelompokkan data berdasarkan produk untuk menentukan 10 produk dengan jumlah penjualan tertinggi, kemudian divisualisasikan menggunakan bar chart.

3. **Analisis Produk Berdasarkan Pendapatan**  
   Menghitung total pendapatan tiap produk dan menampilkan 10 produk dengan pendapatan tertinggi lengkap dengan visualisasi.

4. **Segmentasi Pelanggan menggunakan Metode RFM (Recency, Frequency, Monetary)**  
   Melakukan segmentasi pelanggan berdasarkan:
   - **Recency**: waktu sejak transaksi terakhir  
   - **Frequency**: jumlah transaksi  
   - **Monetary**: total pengeluaran  
   Visualisasi jumlah pelanggan tiap segmen juga disediakan.

5. **Market Basket Analysis (Apriori Algorithm)**  
   Menganalisis produk apa saja yang sering dibeli bersamaan menggunakan algoritma apriori dan menghasilkan aturan asosiasi berdasarkan metrik lift.

---

## Tools dan Library

- Python 3.x  
- Pandas  
- Matplotlib  
- Seaborn  
- mlxtend (untuk Apriori dan Association Rules)  

---

## Cara Menjalankan

1. Pastikan semua dependensi sudah terinstal, misalnya menggunakan pip:

   ```bash
   pip install pandas matplotlib seaborn mlxtend
