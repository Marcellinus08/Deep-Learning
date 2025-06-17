Chapter 2: End-to-End Machine Learning Project
1. Big Picture
Sebuah proyek Machine Learning biasanya mencakup:

Pemahaman masalah
Pengumpulan dan eksplorasi data
Persiapan data
Pemilihan dan pelatihan model
Evaluasi dan penyempurnaan
Deployment dan pemantauan
2. Dataset: California Housing
Digunakan untuk memprediksi harga median rumah berdasarkan fitur seperti jumlah kamar, lokasi, kepadatan penduduk, dan lain-lain.

3. Split Data
Stratified sampling berdasarkan income_cat agar distribusi pendapatan tetap proporsional di train/test.
4. Eksplorasi Data
Visualisasi distribusi, korelasi antar fitur, dan kombinasi fitur seperti rooms_per_household.

5. Preprocessing
Numerik: median imputation + scaling
Kategorikal: one-hot encoding
Dihubungkan dalam ColumnTransformer
6. Model
Linear Regression: baseline yang cepat namun underfitting
Random Forest: model yang lebih kompleks dan akurat
7. Evaluasi
Digunakan metrik RMSE (Root Mean Squared Error)
Lebih akurat menggunakan cross-validation daripada hanya pada training set
8. Fine-Tuning
Teknik seperti Grid Search dan Randomized Search digunakan untuk hyperparameter tuning (belum dimasukkan di kode awal, akan muncul di bab selanjutnya)
9. Deployment
Model akhir dievaluasi di test set dan bisa disimpan untuk di-deploy (misalnya dengan joblib atau pickle)
