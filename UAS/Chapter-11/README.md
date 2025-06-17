Chapter 11: Training Deep Neural Networks

1. Tantangan dalam Deep Learning
- Vanishing gradients: gradien mengecil saat backprop melewati banyak layer → solusi: ReLU, He initialization
- Exploding gradients: gradien membesar → solusi: gradient clipping
2. Weight Initialization
- He initialization cocok untuk ReLU → distribusi bobot stabil
3. Activation Function
- ReLU: default modern DL
- Leaky ReLU, ELU: alternatif untuk mengatasi dead neuron
4. Batch Normalization (BN)
- Normalisasi aktivasi antar layer → mempercepat training dan stabilisasi
- Dapat ditempatkan sebelum atau setelah aktivasi
5. Dropout
- Teknik regularisasi: node secara acak dinonaktifkan saat training
- Mengurangi overfitting dengan mencegah co-adaptation antar neuron
6. Callbacks
- EarlyStopping: hentikan training jika validasi tidak membaik
- ModelCheckpoint: simpan model terbaik selama training
7. Learning Rate Schedules (dibahas di bab selanjutnya)
- Exponential decay, 1cycle, dll.
8. Evaluasi Akhir
- Gunakan test set untuk evaluasi akhir setelah tuning selesai
