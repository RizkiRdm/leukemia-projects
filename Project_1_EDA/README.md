# Project 1: Analisis Deskriptif & Visualisasi Data Awal Leukemia - Detail Teknis

**Tujuan Project:**

*   Melakukan analisis statistik deskriptif dan visualisasi data awal untuk memahami karakteristik dataset leukemia.
*   Mengidentifikasi anomali data dan pola-pola menarik awal.
*   Menjadi dasar untuk analisis faktor risiko di Project 2.

**Plan Project 1:**

1.  **Data Loading & Cleaning:**
    *   Load dataset leukemia dari file `data/leukemia_dataset.csv`.
    *   Handling *missing values* (jika ada).
    *   Handling anomali data (misalnya nilai negatif di `WBC_Count`, BMI rendah ekstrem).

2.  **Analisis Statistik Deskriptif:**
    *   Hitung statistik deskriptif (rata-rata, median, standar deviasi, dll.) untuk kolom numerik menggunakan Pandas `describe()`.
    *   Hitung frekuensi dan proporsi kategori untuk kolom kategori menggunakan Pandas `value_counts()`.

3.  **Visualisasi Data Univariat:**
    *   Buat histogram untuk kolom numerik menggunakan Seaborn `histplot()`.
    *   Buat boxplot untuk kolom BMI menggunakan Seaborn `boxplot()`.
    *   Buat bar chart dan pie chart untuk kolom kategori menggunakan Seaborn `countplot()` dan Matplotlib `pie()`.

4.  **Visualisasi Data Bivariat Awal (vs Leukemia_Status):**
    *   Buat boxplot berdampingan untuk kolom numerik vs `Leukemia_Status` menggunakan Seaborn `boxplot()`.
    *   Buat *stacked bar chart* untuk kolom kategori vs `Leukemia_Status` menggunakan Pandas `crosstab()` dan Matplotlib `bar()`.

5.  **Rangkum Insight Project 1:**
    *   Dokumentasikan semua *insight* dan temuan dari analisis statistik deskriptif dan visualisasi data awal dalam laporan Project 1.

**Tools & Library Python yang Digunakan di Project 1:**

*   **Bahasa Pemrograman:** Python
*   **Library Data Science:** Pandas, NumPy
*   **Library Statistik:** SciPy (opsional, jika ada perhitungan statistik lebih *advance*)
*   **Library Visualisasi:** Matplotlib, Seaborn

**Struktur Folder Project 1:**

```ASSCII
📦Project_1_EDA
 ┣ 📂Visualizations
 ┃ ┣ 📂Barchart
 ┃ ┃ ┣ 📜barcharts_bivariate_status_leukemia_vs_categorical_col.png
 ┃ ┃ ┗ 📜barcharts_univariate_categorical_column.png
 ┃ ┣ 📂Boxplots
 ┃ ┃ ┣ 📜boxplot_BMI.png
 ┃ ┃ ┗ 📜boxplots_bivariate_status_vs_categorical_column.png
 ┃ ┗ 📂histogram
 ┃ ┃ ┣ 📜histogram_patient_age_young_olds.png
 ┃ ┃ ┗ 📜histogram_univariate_numerical_column.png
 ┣ 📂notebook
 ┃ ┗ 📜statistic_leukimia_analysis.ipynb
 ┗ 📜README.md
```