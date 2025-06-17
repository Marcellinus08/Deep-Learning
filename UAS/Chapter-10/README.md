Chapter 10: Introduction to Artificial Neural Networks with Keras

1. Neural Network (NN) vs. Traditional ML
- NN mampu menyelesaikan masalah kompleks yang sulit bagi model linier atau pohon keputusan.
- Memerlukan banyak data dan waktu pelatihan lebih lama.
2. Multi-Layer Perceptron (MLP)
- Terdiri dari lapisan neuron (nodes)
- Setiap neuron melakukan: output = activation(weighted_sum(inputs))
- Arsitektur:
  + Input layer: menerima data mentah
  + Hidden layers: satu atau lebih lapisan tersembunyi (biasanya ReLU)
  + Output layer: satu neuron per kelas (klasifikasi), biasanya softmax
3. Aktivasi
- ReLU (Rectified Linear Unit): max(0, x)
- Softmax: mengubah output menjadi distribusi probabilitas antar kelas
4. Kompilasi
- Loss function: sparse_categorical_crossentropy untuk label integer
- Optimizer: sgd, adam, dll
- Metrics: biasanya accuracy untuk klasifikasi
5. Training & Validation
- Gunakan validation_data untuk memantau overfitting
- Epoch = 1 siklus penuh seluruh data training
6. Evaluasi
- Evaluasi performa di data yang belum pernah dilihat (test set)
7. Summary Keras API
- Sequential API: model linear bertingkat
- Functional API (bab berikutnya): lebih fleksibel, cocok untuk model kompleks
