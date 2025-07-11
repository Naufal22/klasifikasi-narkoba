🧠 **Klasifikasi Konsumsi Narkoba Berdasarkan Kepribadian**

Proyek ini menggunakan *machine learning* (Random Forest, XGBoost) untuk mengklasifikasikan status penggunaan ganja berdasarkan data demografi dan skor kepribadian. Tujuannya adalah membangun model untuk skrining risiko, yang relevan dalam konteks informatika medis.

-----

### 📊 Dataset

  * **Sumber**: [Drug Consumption (Quantified) UCI - ID: 373](https://archive.ics.uci.edu/dataset/373/drug+consumption+quantified)
  * **Fitur**: 12 fitur (Demografi, Skor Kepribadian NEO-FFI-R, Impulsivitas).
  * **Label**: `cannabis` (disederhanakan menjadi `User` & `Non-user`).
  * **Ukuran**: 1885 sampel.

-----

### 🎯 Tujuan

  * Membangun model klasifikasi `User` vs `Non-user` yang andal.
  * Mengatasi masalah *class imbalance* menggunakan teknik SMOTE.
  * Membandingkan performa SVM, Random Forest, dan XGBoost.
  * Mengidentifikasi faktor demografi dan kepribadian yang paling berpengaruh.

-----

### ⚙️ Metode

  * **Model**: Random Forest & XGBoost (model dengan performa terbaik).
  * **Preprocessing**: `StandardScaler` untuk normalisasi fitur, `SMOTE` untuk menyeimbangkan data latih.
  * **Evaluasi**: *Accuracy*, *F1-score*, *Classification Report*.

-----

### 🧪 Hasil

Model **Random Forest** dan **XGBoost** memberikan hasil paling stabil, menunjukkan batas performa dataset.

  * **Akurasi**: **\~79%**
  * **F1-score Rata-rata**: **\~0.76**
  * **Fitur Prediktor Utama**: `country`, `age`, `oscore` (keterbukaan), dan `ss` (pencarian sensasi).

-----

### 🔎 Kesimpulan

Model mencapai performa maksimal karena keterbatasan informasi dalam dataset, bukan karena kelemahan algoritma. Faktor demografis (`country`, `age`) dan sifat kepribadian (`oscore`, `ss`) terbukti menjadi prediktor yang paling signifikan.

-----

### 💡 Relevansi Medis

  * **Skrining Risiko**: Dapat berfungsi sebagai alat bantu awal bagi praktisi medis untuk mengidentifikasi individu berisiko.
  * **Pemahaman Faktor**: Memberikan wawasan tentang profil psikologis yang terkait dengan kecenderungan penggunaan narkoba.

-----

### ▶️ Cara Menjalankan

1.  *Clone* repositori ini.
2.  Install semua dependensi yang dibutuhkan dari `Prasyarat`.
3.  Jalankan *notebook* `narkoba.ipynb` di lingkungan Jupyter.

-----

### 📦 Prasyarat

```bash
pip install pandas numpy matplotlib seaborn scikit-learn ucimlrepo imbalanced-learn xgboost
```

-----

### 🙋 Kontak

MUHAMMAD NAUFAL AQIL

📧 muhammadnaufalaqil20@gmail.com

🔗 [GitHub](https://github.com/Naufal22) | [LinkedIn](https://www.linkedin.com/in/muhammad-naufal-aqil-b6114424a/)

-----

### 🙏 Acknowledgements

  * **Dataset oleh**: Fehrman, E., et al. (2015). *Drug Consumption (Quantified) Dataset*, UCI Machine Learning Repository.
