# 🛒 Customer Segmentation with K-Means Clustering
### Segmentasi Pelanggan Grosir Menggunakan Machine Learning

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USERNAME/customer-segmentation-kmeans/blob/main/customer_segmentation.ipynb)
![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.2-orange?logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

---

## 📌 Deskripsi Proyek

Proyek ini menerapkan algoritma **K-Means Clustering** untuk mengelompokkan pelanggan grosir berdasarkan pola pengeluaran tahunan mereka di enam kategori produk. Hasil segmentasi diintegrasikan ke dalam kerangka **Business Intelligence** untuk menghasilkan rekomendasi strategi pemasaran yang lebih terarah dan berbasis data.

> 💡 **Business Problem:** Perusahaan grosir kesulitan memahami karakteristik pelanggan secara individual. Dengan segmentasi berbasis data, strategi pemasaran, promosi, dan layanan dapat disesuaikan per segmen pelanggan.

---

## 📊 Dataset

| Aspek | Detail |
|-------|--------|
| **Nama** | Wholesale Customers Data Set |
| **Sumber** | [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers) |
| **Ukuran** | 440 baris × 8 kolom |
| **Fitur** | Channel, Region, Fresh, Milk, Grocery, Frozen, Detergents_Paper, Delicassen |

---

## 🔧 Teknologi yang Digunakan

- **Python** — bahasa pemrograman utama
- **Pandas & NumPy** — manipulasi dan analisis data
- **Scikit-learn** — preprocessing, K-Means, PCA, Silhouette Score
- **Matplotlib & Seaborn** — visualisasi data
- **Jupyter Notebook** — environment pengembangan
- **Power BI** — dashboard Business Intelligence

---

## 🚀 Alur Analisis

```
Dataset → EDA → Preprocessing → Elbow Method → K-Means → Evaluasi → Visualisasi → Business Insight
```

1. **Exploratory Data Analysis (EDA)** — distribusi data, korelasi antar fitur
2. **Preprocessing** — seleksi fitur + normalisasi dengan StandardScaler
3. **Elbow Method** — menentukan jumlah klaster optimal (K=3)
4. **Training K-Means** — melatih model dengan K=3
5. **Evaluasi** — Silhouette Score = **0.548** (cukup baik ✅)
6. **Visualisasi** — PCA 2D scatter plot, bar chart, radar chart
7. **Business Insight** — rekomendasi strategi per segmen

---

## 📈 Hasil Segmentasi

| Klaster | Profil | Jumlah Pelanggan | Karakteristik Utama |
|---------|--------|:-----------------:|---------------------|
| **Klaster 0** | Pelanggan Grocery & Retail | 45 | Pengeluaran tinggi pada Grocery, Milk, Detergents_Paper |
| **Klaster 1** | Pelanggan Umum (Mayoritas) | 393 | Pengeluaran sedang dan merata di semua kategori |
| **Klaster 2** | Pelanggan VIP | 2 | Pengeluaran ekstrem tinggi di Fresh, Frozen, Delicassen |

### Evaluasi Model
| Metrik | Nilai | Interpretasi |
|--------|-------|--------------|
| Silhouette Score (K=3) | **0.548** | Cukup baik — klaster terbentuk jelas |
| Metode pemilihan K | Elbow Method | Titik siku di K=3 |

---

## 💡 Business Insight & Rekomendasi

### 🔵 Klaster 0 — Pelanggan Grocery & Retail
- Buat program loyalitas B2B dan diskon grosir khusus
- Tawarkan kontrak pembelian jangka panjang
- Fokus efisiensi suplai produk grocery & household

### 🟠 Klaster 1 — Pelanggan Umum (Mayoritas)
- Kampanye promosi reguler dan bundling produk hemat
- Edukasi produk untuk mendorong upselling
- Program loyalitas dengan sistem poin atau cashback

### 🟢 Klaster 2 — Pelanggan VIP
- Layanan personal dengan account manager khusus
- Tawarkan produk eksklusif, impor, atau private label
- Pertahankan relasi dengan pendekatan langsung & kontrak premium

---

## 📁 Struktur Repo

```
customer-segmentation-kmeans/
│
├── 📓 customer_segmentation.ipynb   # Notebook utama (end-to-end)
├── 📊 Wholesale_customers_data.csv  # Dataset original
├── 📋 requirements.txt              # Daftar library Python
└── 📄 README.md                     # Dokumentasi proyek ini
```

---

## ⚙️ Cara Menjalankan

### Option 1: Google Colab (Recommended)
Klik badge **"Open in Colab"** di bagian atas halaman ini.

### Option 2: Local (Jupyter Notebook)
```bash
# 1. Clone repo ini
git clone https://github.com/USERNAME/customer-segmentation-kmeans.git
cd customer-segmentation-kmeans

# 2. Install dependencies
pip install -r requirements.txt

# 3. Jalankan Jupyter Notebook
jupyter notebook customer_segmentation.ipynb
```

---

## 🔮 Saran Pengembangan

- [ ] Tambahkan fitur **RFM Analysis** (Recency, Frequency, Monetary)
- [ ] Bandingkan dengan metode lain: **Hierarchical Clustering** atau **DBSCAN**
- [ ] Buat **dashboard interaktif** dengan Streamlit atau Tableau Public
- [ ] Tangani outlier sebelum clustering untuk hasil yang lebih robust

---

## 📚 Referensi

- Dua, D. & Graff, C. (2021). *Wholesale Customers Data Set*. UCI Machine Learning Repository. https://archive.ics.uci.edu/ml/datasets/Wholesale+customers
- Scikit-learn Documentation — Clustering: https://scikit-learn.org/stable/modules/clustering.html

---

## 👩‍💻 Author

**Zahrotun Nafisah**  
Sistem Informasi 2022  
📧 [email kamu] | 🔗 [LinkedIn kamu]
