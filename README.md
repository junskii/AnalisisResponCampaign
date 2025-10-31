# Analisis Respon Campaign Pelanggan Supermarket
![Tableau](#https://public.tableau.com/app/profile/muhammad.jundullah/viz/Book1_17512056895580/Dashboard1?publish=yes)

Notebook ini menganalisis perilaku respons pelanggan supermarket berdasarkan berbagai atribut, seperti pendapatan, kunjungan web, status perkawinan, pendidikan, dan lainnya. Tujuan dari analisis ini adalah untuk mengidentifikasi pola perilaku pelanggan dan memberikan rekomendasi yang dapat diterapkan untuk meningkatkan efektivitas kampanye pemasaran di masa depan.

## Daftar Isi

1. [Tujuan](#tujuan)
2. [Overview Data](#overview-data)
3. [Pembersihan Data](#pembersihan-data)
4. [Statistik Deskriptif](#statistik-deskriptif)
5. [Statistik Inferensial](#statistik-inferensial)
   - 5.1 [Pendapatan vs Respons](#pendapatan-vs-respons)
   - 5.2 [Pengeluaran Wine vs Respons](#pengeluaran-wine-vs-respons)
   - 5.3 [Pendidikan vs Respons](#pendidikan-vs-respons)
   - 5.4 [Status Pernikahan vs Respons](#status-pernikahan-vs-respons)
6. [Insight dan Rekomendasi](#insight-dan-rekomendasi)

---

## Tujuan

Tujuan dari analisis ini adalah untuk:
- Menyelidiki faktor-faktor yang mempengaruhi respons pelanggan terhadap kampanye.
- Melakukan uji statistik untuk mengidentifikasi perbedaan signifikan antar kelompok (responden dan non-responden).
- Memberikan wawasan dan rekomendasi berdasarkan temuan data untuk mengoptimalkan strategi pemasaran.

---

## Overview Data

Dataset ini berisi informasi pelanggan dan respons mereka terhadap kampanye pemasaran. Beberapa fitur yang ada dalam dataset ini antara lain:
- **Demografi Pelanggan**: Pendapatan, Pendidikan, Status Pernikahan, dll.
- **Respons Kampanye**: Apakah pelanggan merespons kampanye.
- **Interaksi Web**: Jumlah kunjungan ke website per bulan.

Dataset telah dibersihkan dan diproses untuk memastikan akurasi analisis.

---

## Pembersihan Data

Pada bagian ini, data dibersihkan dengan menangani nilai yang hilang, memperbaiki tipe data, dan menangani outlier. Beberapa langkah yang diambil adalah:
- Nilai yang hilang ditangani dengan cara menghapus atau mengimputasi data yang hilang.
- Kolom `Response` diubah menjadi tipe data boolean (True/False).
- Outlier pada kolom numerik seperti `Income` dan `MntWines` diatasi.

---

## Statistik Deskriptif

Statistik deskriptif memberikan gambaran umum tentang data, meliputi:
- **Pendapatan**: Rata-rata dan distribusi pendapatan pelanggan.
- **Pengeluaran Wine**: Pengeluaran rata-rata untuk wine.
- **Recency**: Waktu sejak pembelian terakhir.
- **NumWebVisitsMonth**: Jumlah kunjungan web per bulan.

---

## Statistik Inferensial

Bagian ini berisi uji statistik untuk menentukan apakah ada perbedaan signifikan antar kelompok. Uji yang dilakukan adalah:
- **Pendapatan vs Respons**: Uji t independen untuk membandingkan rata-rata pendapatan antara pelanggan yang merespons kampanye dan yang tidak.
- **Pengeluaran Wine vs Respons**: Uji t independen untuk membandingkan rata-rata pengeluaran wine antara responden dan non-responden.
- **Pendidikan vs Respons**: Uji Chi-Square untuk menentukan apakah ada asosiasi antara tingkat pendidikan dan respons terhadap kampanye.
- **Status Pernikahan vs Respons**: Uji Chi-Square untuk menganalisis hubungan antara status pernikahan dan respons.

---

## Insight dan Rekomendasi

**Insight Utama**:
1. **Pendapatan dan Respons**: Pelanggan dengan pendapatan lebih tinggi cenderung lebih sering merespons kampanye, yang menunjukkan bahwa **pendapatan berperan penting** dalam respons terhadap promosi.
2. **Pengeluaran Wine**: Pelanggan dengan pengeluaran lebih tinggi untuk wine lebih cenderung merespons kampanye, menunjukkan bahwa **loyalitas produk** dapat mempengaruhi respons.
3. **Pendidikan dan Respons**: Ada asosiasi signifikan antara tingkat pendidikan dan respons, yang menunjukkan bahwa **pendidikan mempengaruhi tingkat keterlibatan pelanggan**.
4. **Status Pernikahan dan Respons**: Status pernikahan berhubungan dengan respons, dengan pelanggan yang sudah menikah lebih cenderung merespons kampanye.

**Rekomendasi**:
1. **Targetkan Pelanggan dengan Pendapatan Lebih Tinggi**: Fokuskan kampanye pemasaran pada pelanggan dengan pendapatan lebih tinggi karena mereka lebih cenderung merespons.
2. **Segmentasi Berdasarkan Tingkat Pendidikan**: Sesuaikan kampanye dengan tingkat pendidikan pelanggan untuk meningkatkan tingkat respons.
3. **Fokus pada Pelanggan dengan Pengeluaran Lebih Tinggi untuk Wine**: Pelanggan yang memiliki pengeluaran lebih tinggi untuk wine lebih mungkin merespons, sehingga memberikan **penawaran yang lebih relevan** dapat meningkatkan konversi.


---

## Kebutuhan Sistem

- Python 3.x
- Libraries: pandas, numpy, scipy, matplotlib, seaborn, tableau

Pastikan untuk menginstal package yang dibutuhkan dengan:
```bash
pip install pandas numpy scipy matplotlib seaborn

