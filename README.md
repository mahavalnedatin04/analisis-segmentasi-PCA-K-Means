# Optimasi Segmentasi Pengguna Perpustakaan Menggunakan PCA dan K-Means Clustering

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mahavalnedatin04/analisis-segmentasi-PCA-K-Means/blob/main/analisis_segmentasi_pca_kmeans.ipynb)

## Latar Belakang & Tujuan
Evaluasi kualitas layanan perpustakaan menggunakan instrumen **LibQUAL+** menghasilkan banyak dimensi dan indikator penilaian. Proyek ini bertujuan untuk mereduksi dimensi fitur menggunakan **Principal Component Analysis (PCA)** sekaligus mengoptimalkan pengelompokan profil kepuasan pemustaka menggunakan **K-Means Clustering** agar strategi peningkatan layanan dapat difokuskan secara tepat sasaran.

## Alur Metodologi
1. **Data Preprocessing & Uji Kelayakan:** Pembersihan data, seleksi indikator LibQUAL+, standardisasi skala fitur (`StandardScaler`), serta pengujian kelayakan analisis faktor menggunakan **KMO** (*Kaiser-Meyer-Olkin*) dan **Bartlett's Test of Sphericity**.
2. **Reduksi Dimensi (PCA):** Ekstraksi komponen utama berdasarkan *eigenvalue* dan *cumulative explained variance* untuk menyederhanakan variabel tanpa kehilangan informasi penting.
3. **Penentuan Klaster Optimal & Clustering (K-Means):** Evaluasi jumlah klaster terbaik menggunakan **Silhouette Score**, pembentukan klaster dengan K-Means, serta uji beda antar klaster (*ANOVA / Kruskal-Wallis* dan *Post-Hoc Tukey HSD*).
4. **Profiling Segmen Pemustaka:** Interpretasi karakteristik tingkat kepuasan pada masing-masing klaster yang terbentuk.

## Tools & Library
* **Bahasa Pemrograman:** Python 3
* **Lingkungan Kerja:** Google Colaboratory
* **Library Utama:** `pandas`, `numpy`, `scikit-learn`, `factor_analyzer`, `scipy`, `statsmodels`, `matplotlib`, `seaborn`

---
*Dikembangkan sebagai bagian dari penelitian Magister Teknologi Informasi.*
