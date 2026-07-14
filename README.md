# Ringkasan Proyek
Proyek analitik ini bertujuan untuk mendiagnosis akar masalah tingginya tingkat pembatalan layanan (*churn*) pada pelanggan perusahaan telekomunikasi. Analisis dilakukan secara *end-to-end* menggunakan SQL untuk ekstraksi data historis dan Python untuk uji korelasi statistik.

## 🛠️ Tools yang Digunakan
* **SQL (SQLite):** Data Aggregation, Conditional Logic (CASE WHEN), Data Filtering.
* **Python (Pandas, Seaborn):** Data Cleaning, Pemodelan Matriks Korelasi (Heatmap), Exploratory Data Analysis (EDA).

## 💡 Key Insights (Temuan Bisnis)
1. **Contract Vulnerability (Temuan SQL):** 
   Pelanggan dengan tipe kontrak bulanan (*Month-to-month*) memiliki tingkat *churn* tertinggi yang sangat mengkhawatirkan, yaitu sebesar **42.71%**. Hal ini berbanding terbalik dengan pelanggan kontrak 2 tahun yang tingkat *churn*-nya hanya di angka 2.83%.
2. **Retention Sweet Spot (Temuan Python):** 
   Analisis *Heatmap* menunjukkan korelasi negatif moderat (-0.35) antara *tenure* (lama berlangganan) dan tingkat *churn*. Ini mengonfirmasi bahwa risiko kehilangan pelanggan berada pada titik tertinggi di bulan-bulan awal berlangganan, dan loyalitas akan terbentuk seiring berjalannya waktu.

## 🚀 Rekomendasi Strategi
Tim *Marketing* disarankan untuk mengalihkan alokasi anggaran retensi agar difokuskan 100% pada pengalaman pengguna (UX) pelanggan baru di 6 bulan pertama, khususnya bagi mereka yang memilih paket *Month-to-month*.
