# 📊 Beauty & Cosmetics E-Commerce Insights (Looker Studio)

## Latar Belakang
Analisis pasar dan performa produk kosmetik menggunakan dataset e-commerce (11.373 produk). Project ini berfokus pada pembersihan data yang kompleks (encoding errors) dan visualisasi data interaktif untuk menemukan tren pasar serta rekomendasi strategi bisnis.

## Pertanyaan Bisnis
1. Kategori dan bentuk produk (liquid, cream, stick) apa yang paling mendominasi pasar?
2. Brand mana yang memiliki interaksi konsumen (total ulasan) tertinggi?
3. Bagaimana korelasi antara harga produk dengan rating yang diberikan konsumen?
4. Apakah terdapat anomali (outlier) pada harga produk yang mempengaruhi rata-rata pasar?

## Dataset
- **Sumber:** Kaggle — E-Commerce Cosmetics Dataset
- **Ukuran awal:** 11.373 baris × 30 kolom
- **Missing values:** Ditangani dengan imputasi (untuk data rating) dan filtering.

## Tools
- **Python (Pandas, Numpy) di Google Colab:** Data Cleaning & Feature Engineering.
- **Looker Studio:** Interactive Dashboard & Data Visualization.

## Data Cleaning
- **Encoding Fix:** Membersihkan karakter aneh (mojibake) pada nama brand (contoh: `L'Orï¿½ï¿½ï¿½ï¿½ï¿½ï¿½al` menjadi `L'Oreal`).
- **Data Type Conversion:** Memastikan kolom metrik (harga, rating) menjadi tipe data Numerik yang valid.
- **Feature Engineering:** Membuat kategori baru (Price Category, Popularity Level) dan konversi mata uang (Rupee ke Rupiah).
- **Handling Outliers:** Mengidentifikasi harga ekstrem (misal: parfum 94.000 Rupee) yang membuat nilai rata-rata (mean) menjadi *skewed*.

## Hasil Analisis (Key Insights)
- **Market Dominance:** Bentuk *Liquid* mendominasi hampir semua subkategori, terutama Perfume dan Serum.
- **Engagement:** Kategori *Lips* dan *Skincare* menyumbang lebih dari 65% total ulasan (Reviews).
- **Brand Leader:** Maybelline memimpin dengan hampir 476K ulasan, disusul NYX dan Lakme.
- **Price Anomaly:** Terdapat *outlier* harga ekstrem (di atas 20 juta Rupiah) yang mendistorsi rata-rata harga pasar. Jika dikecualikan, harga rata-rata pasar sebenarnya ada di kisaran Rp 268.000.

## 💡 Actionable Recommendations
1. **Fokus R&D:** Prioritaskan inovasi pada formulasi produk cair (liquid) dan kategori *skincare* untuk mengambil pangsa pasar terbesar.
2. **Audit Premium:** Lakukan audit kualitas pada produk di atas 20K Rupee agar *value for money*-nya sebanding dengan harga.
3. **Strategi Bundling:** Terapkan strategi *bundling* khusus untuk produk kategori *Lips* guna memaksimalkan tingginya interaksi konsumen.


## 🔗 Interactive Dashboard Link
[Cek Dashboard Looker Studio di sini](https://datastudio.google.com/reporting/b682b04f-a985-4f78-a81e-f9f52e9f6b1b)

---
*Created by Shofi Syahria Mahram | [GitHub Profile](https://github.com/shofiesyrrr)*
