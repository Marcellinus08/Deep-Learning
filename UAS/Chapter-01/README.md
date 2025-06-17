Chapter 1: The Machine Learning

1. Persiapan dan Visualisasi Data
- Menggunakan data dari OECD dan GDP World Bank tahun 2015.
- Data difilter dan digabung berdasarkan negara.
- Visualisasi scatterplot menggambarkan korelasi positif antara GDP per kapita dan Life Satisfaction.
2. Linear Regression (Model Dasar)
- Model linier sederhana dilatih pada sebagian data (sample).
- Model digunakan untuk memprediksi Life Satisfaction negara Cyprus.
3. Perbandingan Model
a. Linear Regression (seluruh data)
- Model linier dilatih menggunakan seluruh dataset (bukan subset).
b. Ridge Regression
- Regularisasi L2 diterapkan untuk menghindari overfitting pada data kecil.
c. Polynomial Regression (Overfitting)
- Model polinomial derajat tinggi (30) diterapkan.
- Pipeline preprocessing mencakup standarisasi fitur.
Evaluasi Visual
Visualisasi kurva prediksi membantu memahami kinerja dan kompleksitas model.
Ridge menunjukkan trade-off antara bias dan varians.
