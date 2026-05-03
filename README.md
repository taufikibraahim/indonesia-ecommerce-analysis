# 🛍️ Indonesia E-Commerce Sales Analysis 2023–2025

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas)
![Tableau](https://img.shields.io/badge/Tableau-Public-E97627?logo=tableau)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> **Platform:** Shopee Indonesia &nbsp;|&nbsp; **Period:** Desember 2023 – November 2025 &nbsp;|&nbsp; **Transactions:** 22,766

---

## 📌 Project Overview

Analisis komprehensif terhadap data penjualan dan pengiriman e-commerce Indonesia di platform Shopee selama 2 tahun. Project ini mencakup seluruh alur kerja data analyst — dari data cleaning, exploratory data analysis (EDA), hingga visualisasi dashboard interaktif di Tableau.

**Tujuan Analisis:**
- Mengidentifikasi tren revenue dan pola musiman
- Menganalisis performa kategori produk dan distribusi geografis
- Memahami pola pembatalan pesanan dan faktor penyebabnya
- Memberikan rekomendasi bisnis berbasis data

---

## 🗂️ Project Structure

```
📁 indonesia-ecommerce-analysis/
├── 📓 ecommerce_sales_shipping_indonesia.ipynb  ← Main notebook
├── 📊 all_months_clean.csv                      ← Dataset utama
├── 📊 DecemberSales2024_clean.xlsx              ← Data tambahan Des 2024
├── 📊 JulySales2025_clean.xlsx                  ← Data tambahan Jul 2025
├── 📊 ecommerce_clean.csv                       ← Output: data bersih
├── 📊 ecommerce_time.csv                        ← Output: data tren waktu
└── 📄 README.md
```

---

## 🔧 Tools & Libraries

| Tool | Kegunaan |
|---|---|
| **Python 3.11** | Data processing & EDA |
| **Pandas** | Data manipulation & cleaning |
| **Matplotlib** | Visualisasi dasar |
| **Seaborn** | Visualisasi statistik |
| **Tableau Public** | Dashboard interaktif |

---

## 📊 Dataset

| Parameter | Detail |
|---|---|
| Sumber | [Kaggle — Indonesia E-Commerce Sales & Shipping 2023–2025](https://www.kaggle.com/datasets/bakitacos/indonesia-e-commerce-sales-and-shipping-20232025) |
| Total Transaksi | 22,766 pesanan |
| Periode | Desember 2023 – November 2025 |
| Jumlah Kolom | 19 variabel |
| Platform | Shopee Indonesia |

---

## 🔍 Data Cleaning Summary

| Masalah | Tindakan |
|---|---|
| Tipe data datetime salah (`object`) | Diubah ke `datetime64` |
| Kolom kategorikal tidak efisien | Diubah ke tipe `category` |
| Order Selesai dengan nilai Rp 0 (0.35%) | Di-drop sebagai anomali |
| 2 file tanpa timestamp (Des 2024 & Jul 2025) | Diperbaiki dengan tanggal representatif |
| Data tersebar di multiple file | Digabung dengan `pd.concat()` |

---

## 💡 Key Insights

**1. 📍 Konsentrasi Geografis**
> 65% revenue terkonsentrasi di 3 provinsi Jawa (Jawa Barat, DKI Jakarta, Banten). Ekspansi ke Sumatera & Kalimantan berpotensi membuka 35% revenue baru.

**2. 💳 Dominasi COD**
> COD mendominasi 55% transaksi — meningkatkan risiko gagal bayar. Rekomendasi: filter COD hanya untuk pelanggan dengan histori baik dan berikan insentif untuk pembayaran online.

**3. 📈 Momen Sale**
> Revenue tertinggi terjadi September 2024 (Rp 71.193.097) bertepatan dengan 9.9 Shopee Sale. Maksimalkan budget iklan & stok di periode 9.9, 10.10, dan 12.12.

**4. ❌ Cancel Rate**
> Cancel rate 13.6% berada di atas rata-rata industri (8–10%). Tertinggi Juni 2025 — berkorelasi dengan implementasi pajak e-commerce 0.5% dari omzet.

**5. 🏆 Product Mix**
> Seal/Baut/Roof = revenue driver (Rp 245 juta) dengan nilai per unit tinggi. Celengan = traffic driver dengan volume order tertinggi (6,366 orders).

---

## 📈 Dashboard Tableau

🔗 **[Lihat Dashboard Interaktif →](https://public.tableau.com/app/profile/taufik.ibrahim/viz/IndonesiaE-CommerceSalesAnalysis2023-2025/IndonesiaE-CommerceDashboard)**

Dashboard mencakup:
- KPI Overview (Revenue, Orders, Cancel Rate, AOV)
- Tren Revenue Bulanan 2023–2025
- Perbandingan 2024 vs 2025
- Top Kategori Produk by Revenue
- Distribusi Geografis per Provinsi
- Analisis Metode Pembayaran
- Cancel Rate Analysis

---

## 🚀 How to Run

1. Clone repository ini
```bash
git clone https://github.com/taufikibraahim/indonesia-ecommerce-analysis.git
cd indonesia-ecommerce-analysis
```

2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

3. Jalankan notebook
```bash
jupyter notebook ecommerce_sales_shipping_indonesia.ipynb
```

---

## 👤 Author

**Mohammad Taufik Ibrahim**
- 🔗 LinkedIn: [linkedin.com/in/taufikibraahim](https://www.linkedin.com/in/taufikibraahim/)
- 📊 Tableau: [public.tableau.com/app/profile/taufik.ibrahim](https://public.tableau.com/app/profile/taufik.ibrahim)

---

*⭐ Jika project ini bermanfaat, jangan lupa kasih star di GitHub!*
