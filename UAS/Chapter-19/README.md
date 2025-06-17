Chapter 19: Training and Deploying at Scale

1. Persiapan Data MNIST
- MNIST adalah dataset gambar tangan angka 0–9 berukuran 28x28 piksel grayscale. Data di-normalisasi menjadi [0,1] dan dibagi menjadi data training, validasi, dan testing.
2. Training Model Dasar
- Model sederhana Sequential dengan dua Dense layers dilatih menggunakan sparse_categorical_crossentropy. Model ini digunakan sebagai baseline sebelum disimpan dan diekspor.
3. Export SavedModel Format
- Model disimpan ke direktori dalam format SavedModel, format standar TensorFlow untuk deployment. Direktori berisi arsitektur, bobot, dan metadata signature.
4. Menjalankan TensorFlow Serving
- Menginstal tensorflow-model-server dari repository Google.
- Menjalankan server REST API di port 8501 secara background dengan model yang telah diekspor.
- Melakukan request HTTP POST ke endpoint /v1/models/{model_name}:predict dengan data input JSON.
- Mendapatkan prediksi dari model dan memvisualisasikan hasilnya.
5. Distribusi Pelatihan dengan MirroredStrategy
- tf.distribute.MirroredStrategy() memungkinkan pelatihan model menggunakan beberapa GPU secara paralel.
- Kelebihan:
  + Meningkatkan kecepatan training.
  + Dapat memanfaatkan semua GPU pada satu mesin.
6. Evaluasi dan Visualisasi
- Menghitung loss dan accuracy pada test set.
- Menampilkan plot learning curve dari training dan validasi menggunakan pandas.DataFrame.plot().
