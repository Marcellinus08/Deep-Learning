Chapter 6: Decision Trees

1. Apa itu Decision Tree?
Model prediktif yang memecah data ke dalam cabang-cabang berdasarkan fitur.
Setiap node berisi pertanyaan dan cabangnya menjawab ya/tidak.
2. Klasifikasi & Regresi
- Klasifikasi: memprediksi kelas
- Regresi: memprediksi nilai numerik
3. Algoritma CART
CART (Classification and Regression Tree) adalah algoritma greedy:
- Pada setiap node, cari split terbaik yang meminimalkan impurity (misalnya Gini)
Gini Impurity
[ G_i = 1 - \sum p_i^2 ]
Entropy
[ H = -\sum p_i \log_2 p_i ]
4. Overfitting & Regularisasi
- Tanpa batas kedalaman, Decision Tree cenderung overfit
- Solusi:
  + Batasi max_depth, min_samples_split, min_samples_leaf
  + Pruning (post-training, tidak tersedia default di Scikit-Learn)
5. Visualisasi
Gunakan plot_tree() atau export ke Graphviz dengan export_graphviz
6. Keuntungan
- Interpretable & cepat
- Dukung data numerik & kategorikal
7. Kelemahan
- Rentan terhadap overfitting
- Tidak stabil (sedikit perubahan → pohon berbeda)
8. Decision Tree untuk Regresi
Sama prinsipnya, tetapi menggunakan prediksi nilai rata-rata dan split berdasarkan minimisasi MSE.
