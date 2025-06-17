Chapter 8: Dimensionality Reduction

1. Mengapa Mengurangi Dimensi?
- Mempercepat pemrosesan
- Mengurangi noise
- Memvisualisasi data
- Menghindari curse of dimensionality
2. Principal Component Analysis (PCA)
- Teknik reduksi dimensi linier
- Mengubah data ke sumbu-sumbu baru (principal components) yang memaksimalkan varian
- Komponen PCA:
  + Komponen pertama = arah varian maksimum
  + Komponen kedua = ortogonal ke yang pertama, varian terbesar kedua, dst.
- Explained Variance
  + Proporsi informasi yang dipertahankan oleh tiap komponen
  + Dapat digunakan untuk menentukan berapa banyak komponen yang dibutuhkan
3. PCA Invers
- Kita bisa rekonstruksi data dari komponen → lihat seberapa banyak info hilang
4. Kernel PCA
- PCA versi non-linear, menggunakan kernel trick
- Cocok untuk data yang tidak bisa dipisahkan secara linier
5. Locally Linear Embedding (LLE)
- Teknik manifold learning
- Mengasumsikan bahwa data hidup di manifold berdimensi lebih rendah
- Menggabungkan lokal linearity untuk menghasilkan representasi global
