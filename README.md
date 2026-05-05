# 🛍️ Indonesia E-Commerce Sales Analysis 2023–2025

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-2.0-150458?logo=pandas)
![Tableau](https://img.shields.io/badge/Tableau-Public-E97627?logo=tableau)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)

> **Platform:** Shopee Indonesia &nbsp;|&nbsp; **Period:** December 2023 – November 2025 &nbsp;|&nbsp; **Transactions:** 22,766

---

## 📌 Project Overview

A comprehensive analysis of 2 years of sales and shipping data from Shopee Indonesia, covering the full data analyst workflow — from data cleaning and exploratory data analysis (EDA) to an interactive Tableau dashboard.

**Business Objectives:**
- Identify revenue trends and seasonal patterns
- Analyze product category performance and geographic distribution
- Understand order cancellation patterns and their root causes
- Deliver data-driven business recommendations

---

## 🔗 Interactive Dashboard

👉 **[View on Tableau Public](https://public.tableau.com/app/profile/taufik.ibrahim/viz/IndonesiaE-CommerceSalesAnalysis2023-2025/IndonesiaE-CommerceDashboard)**

The dashboard includes:
- KPI Overview (Revenue, Orders, Cancel Rate, AOV)
- Monthly Revenue Trend 2023–2025
- Year-over-Year Comparison: 2024 vs 2025
- Top Product Categories by Revenue
- Geographic Distribution by Province
- Payment Method Analysis
- Cancel Rate Analysis

---

## 📊 Dataset

| Parameter | Detail |
|---|---|
| Source | [Kaggle — Indonesia E-Commerce Sales & Shipping 2023–2025](https://www.kaggle.com/datasets/bakitacos/indonesia-e-commerce-sales-and-shipping-20232025) |
| Total Transactions | 22,766 orders |
| Period | December 2023 – November 2025 |
| Features | 19 variables |
| Platform | Shopee Indonesia |

---

## 🔧 Tools & Libraries

| Tool | Purpose |
|---|---|
| **Python 3.11** | Data processing & EDA |
| **Pandas** | Data manipulation & cleaning |
| **Matplotlib / Seaborn** | Statistical visualization |
| **Tableau Public** | Interactive dashboard |

---

## 🗂️ Project Structure

```
📁 indonesia-ecommerce-analysis/
├── 📓 ecommerce_sales_shipping_indonesia.ipynb  ← Main analysis notebook
├── 📊 all_months_clean.csv                      ← Primary dataset
├── 📊 DecemberSales2024_clean.xlsx              ← Additional data (Dec 2024)
├── 📊 JulySales2025_clean.xlsx                  ← Additional data (Jul 2025)
├── 📊 ecommerce_clean.csv                       ← Output: cleaned data
├── 📊 ecommerce_time.csv                        ← Output: time-series data
└── 📄 README.md
```

---

## 🔍 Data Cleaning Summary

| Issue | Action Taken |
|---|---|
| Incorrect datetime types (`object`) | Converted to `datetime64` |
| Inefficient categorical columns | Cast to `category` dtype |
| Completed orders with Rp 0 value (0.35%) | Dropped as anomalies |
| 2 files missing timestamps (Dec 2024 & Jul 2025) | Fixed with representative dates |
| Data spread across multiple files | Merged using `pd.concat()` |

---

## 💡 Key Insights & Business Recommendations

### 1. 📍 Geographic Concentration
> 65% of revenue is concentrated in 3 Java provinces (West Java, DKI Jakarta, Banten). Expanding into Sumatra & Kalimantan could unlock the remaining 35% of potential revenue.

**Recommendation:** Prioritize logistics partnerships in Sumatra & Kalimantan to reduce shipping times and support geographic expansion.

---

### 2. 💳 COD Payment Dominance
> Cash-on-Delivery (COD) accounts for 55% of transactions, increasing failed-delivery risk.

**Recommendation:** Restrict COD to customers with a positive order history and introduce incentives (e.g., vouchers, cashback) to encourage online payment adoption — reducing COD-related cancellations by an estimated 10–15%.

---

### 3. 📈 Seasonal Sales Peaks
> Highest revenue occurred in September 2024 (Rp 71,193,097), coinciding with Shopee's 9.9 Sale event.

**Recommendation:** Allocate 30–40% of ad budget to peak sale periods (9.9, 10.10, 12.12) and pre-stock high-demand SKUs at least 2 weeks in advance.

---

### 4. ❌ Above-Average Cancel Rate
> Cancellation rate of 13.6% exceeds the industry benchmark of 8–10%. The highest cancel month was June 2025 — correlating with the implementation of a 0.5% e-commerce revenue tax.

**Recommendation:** Implement real-time order monitoring with automated alerts when cancel rates exceed 10%. Improve pre-purchase clarity (pricing, delivery estimates) to reduce buyer regret cancellations.

---

### 5. 🏆 Product Mix Strategy
> Seal/Bolt/Roof products = revenue driver (Rp 245M) with high unit value. Piggy banks = traffic driver with the highest order volume (6,366 orders).

**Recommendation:** Bundle high-volume (traffic) products with high-margin (revenue) products to increase average order value. Use piggy banks as entry-point products with upsell opportunities.

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/taufikibraahim/indonesia-ecommerce-analysis.git
cd indonesia-ecommerce-analysis

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn openpyxl

# 3. Launch the notebook
jupyter notebook ecommerce_sales_shipping_indonesia.ipynb
```

---

## 👤 About the Author

**Mohammad Taufik Ibrahim** — Data Analyst

- 🔗 LinkedIn: [linkedin.com/in/taufikibraahim](https://www.linkedin.com/in/taufikibraahim/)
- 📊 Tableau: [public.tableau.com/app/profile/taufik.ibrahim](https://public.tableau.com/app/profile/taufik.ibrahim)
- 💻 GitHub: [github.com/taufikibraahim](https://github.com/taufikibraahim)

---

*⭐ If you found this project useful, consider leaving a star!*
