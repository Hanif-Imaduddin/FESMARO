# Sentiment Analysis on Amazon Reviews

## Deskripsi Proyek

Proyek ini bertujuan untuk melakukan analisis sentimen pada ulasan pelanggan dari platform Amazon. Dua model machine learning digunakan untuk membandingkan performa dalam klasifikasi sentimen, yaitu **Random Forest** dan **DistilBERT**. Dataset yang digunakan berisi lebih dari 3,6 juta ulasan dengan label sentimen positif dan negatif.

## Struktur Proyek

```
📂 Sentiment-Analysis-Project
│-- 📄 README.md (Dokumen ini)
│-- 📄 Laporan.pdf (Laporan penelitian lengkap)
│-- 📂 dataset/ (Folder berisi dataset ulasan Amazon)
│   │-- reviews.csv
│-- 📂 notebooks/
│   │-- RandomForest_Model.ipynb (Notebook dengan model Random Forest)
│   │-- DistilBERT_Model.ipynb (Notebook dengan model DistilBERT)
```

## Metodologi

1. **Data Preprocessing**

   - Pembersihan teks ulasan
   - Normalisasi huruf
   - Tokenisasi menggunakan DistilBERT

2. **Modeling**

   - **Random Forest**: Model berbasis pohon keputusan yang digunakan sebagai baseline.
   - **DistilBERT**: Model berbasis transformer yang lebih canggih untuk memahami konteks teks secara mendalam.

3. **Evaluasi Model**

   - Akurasi:
     - Random Forest: **61.05%**
     - DistilBERT: **92.44%**
   - Waktu Testing:
     - Random Forest: **5 jam**
     - DistilBERT: **3 jam**

## Kesimpulan

DistilBERT unggul dalam akurasi dan efisiensi dibandingkan Random Forest. Dengan pemrosesan berbasis transformer, DistilBERT mampu menangkap makna konteks yang lebih kompleks dalam teks, menghasilkan klasifikasi sentimen yang lebih akurat.

## Cara Menjalankan Proyek

1. Pastikan Anda telah menginstal dependensi yang diperlukan:
   ```bash
   pip install pandas scikit-learn transformers torch
   ```
2. Jalankan notebook sesuai model yang diinginkan:
   - Untuk Random Forest:
     ```bash
     jupyter notebook notebooks/RandomForest_Model.ipynb
     ```
   - Untuk DistilBERT:
     ```bash
     jupyter notebook notebooks/DistilBERT_Model.ipynb
     ```

## Referensi

- [Sentiment Analysis with DistilBERT](https://jacobj215.github.io/Sentiment-Analysis-with-DistilBERT/)
- [Analisis Sentimen Ulasan Produk E-Commerce (UGM Repository)](https://etd.repository.ugm.ac.id/penelitian/detail/230575)

---

**Penulis:** Koding Muda Nusantara - Telkom University\
**Tanggal: 31 Maret 2025**

