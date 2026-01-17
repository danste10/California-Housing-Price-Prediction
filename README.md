# California Housing Price Prediction
**Capstone Project Module 3 - Data Science**

## Project Overview
Proyek ini bertujuan untuk mengembangkan model prediksi harga rumah di California menggunakan Machine Learning. Dengan dataset sensus yang mencakup data pendapatan, lokasi geografis, dan karakteristik bangunan, model ini dirancang untuk memberikan estimasi harga yang akurat bagi perusahaan real estate dan investor.

## Business Problem
Penentuan harga properti secara manual seringkali bersifat subjektif, lambat, dan berisiko. Hal ini dapat menyebabkan:
* **Underpricing:** Perusahaan kehilangan potensi margin keuntungan.
* **Overpricing:** Properti sulit terjual dan kalah saing di pasar.
* **Inefisiensi:** Proses riset manual menghambat kecepatan pengambilan keputusan.

**Goal:** Membangun sistem otomatisasi valuasi properti yang objektif, cepat, dan berbasis data.

## Data & Preprocessing
Dataset terdiri dari 20.640 entri. Langkah-langkah pengolahan data meliputi:
1.  **Cleaning:** Imputasi nilai kosong pada `total_bedrooms` menggunakan nilai Median.
2.  **Feature Engineering:** One-Hot Encoding untuk fitur `ocean_proximity`.
3.  **Scaling:** RobustScaler untuk menangani outlier pada data numerik.

## Modeling & Evaluation
Dua algoritma dibandingkan untuk mendapatkan performa terbaik:
* **Linear Regression** (Baseline)
* **Random Forest Regressor** (Final Model)

### Model Performance (Random Forest):
| Metric | Score |
| :--- | :--- |
| **MAPE** | 18.63% |
| **R-Squared** | 0.77 |

Model ini berhasil menangkap **77% variabilitas harga**, menjadikannya fondasi yang kuat untuk digitalisasi valuasi aset perusahaan.

## Key Insights & Recommendations
* **Predictor Utama:** `Median Income` adalah faktor paling dominan dalam menentukan harga, disusul oleh lokasi geografis (`Inland`).
* **Strategi Bisnis:** Fokus pada akuisisi properti di area berpendapatan tinggi dan dekat pesisir untuk memaksimalkan ROI.
* **Operasional:** Gunakan model sebagai alat *screening* awal bagi tim sales untuk mempercepat pemberian kuotasi harga kepada klien.

## File Directory
* `Capstone_Project_Module_3.ipynb`: Notebook kodingan lengkap.
* `linear_regression_model.pkl`: Model baseline (Linear Regression).
* `random_forest_model_final.pkl`: Model final (Random Forest).

---
**Author:** Daniel Stevalen Wijaya
