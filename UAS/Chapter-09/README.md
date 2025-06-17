Chapter 9: Unsupervised Learning Techniques

1. Clustering
- Unsupervised learning untuk mengelompokkan data berdasarkan kemiripan. Tidak ada label yang digunakan.

A. K-Means
- Algoritma iteratif untuk meminimalkan jarak rata-rata ke pusat cluster.
- Kelebihan:
  + Cepat dan sederhana
- Kekurangan:
  + Perlu menentukan jumlah cluster (k)
  + Tidak cocok untuk cluster non-sferikal
- Evaluasi:
  + Inertia: total jarak kuadrat ke pusat cluster
  + Elbow Method: cari titik di mana penurunan inertia melambat
  + Silhouette Score: metrik seberapa baik data cocok dengan cluster

B. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)
- Mendeteksi cluster berdasarkan kerapatan data
- Kelebihan:
  + Tidak perlu k
  + Mendeteksi outlier (label = -1)
  + Cocok untuk cluster bentuk arbitrer
- Parameter:
  + eps: radius maksimum tetangga
  + min_samples: jumlah minimum poin untuk dianggap core point

C. Gaussian Mixture Model (GMM)
- Pendekatan probabilistik untuk clustering
- Cocok untuk data dengan distribusi Gaussian bertumpuk
- Dapat menghitung probabilitas keanggotaan tiap titik ke tiap cluster
2. Anomaly Detection
- Titik data yang tidak cocok dengan pola mayoritas
- DBSCAN otomatis memberi label -1 untuk outlier
- GMM dapat digunakan untuk threshold probabilitas
3. Clustering dan Dimensionality Reduction
- Clustering bisa dilakukan setelah PCA/TSNE/LLE
- Visualisasi dan kecepatan lebih baik setelah reduksi dimensi
