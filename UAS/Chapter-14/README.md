Chapter 14: Deep Computer Vision Using CNNs

1. Apa itu CNN?
- Convolutional Neural Networks adalah jenis arsitektur deep learning yang unggul dalam pemrosesan data grid seperti gambar.
- Ciri utama:
  + Convolution layer: filter belajar mendeteksi fitur lokal
  + Pooling layer: downsampling untuk mengurangi dimensi & memperkuat fitur dominan
  + Fully Connected layer: untuk klasifikasi akhir
2. Layer Convolution
- Filter (kernel) bergerak di atas gambar
- Padding "same" mempertahankan ukuran input
- Aktivasi umum: ReLU
3. Pooling
- MaxPooling: mengambil nilai maksimum dari patch
- Menurunkan dimensi, menambah translasi-invariansi
4. Arsitektur Populer
- LeNet-5
  + CNN klasik untuk MNIST, terdiri dari: Conv → Pool → Conv → Pool → Dense → Output
- Modern CNN
  + Kombinasi bertingkat: Conv → BN → ReLU → Pooling → Dropout → Dense
5. Dropout
- Mengurangi overfitting dengan menonaktifkan neuron selama training
6. Tips Praktis
- Gunakan padding="same" agar output tidak terlalu cepat mengecil
- Layer akhir gunakan softmax untuk klasifikasi multi-kelas
- Pastikan input memiliki channel axis: (28, 28, 1)
7. Visualisasi Filter
- Dapat digunakan untuk interpretasi: apa yang dipelajari oleh layer pertama?
