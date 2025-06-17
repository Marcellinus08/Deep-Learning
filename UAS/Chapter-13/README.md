Chapter 13: Loading and Preprocessing Data with TensorFlow

1. tf.data.Dataset
API untuk membuat pipeline input data yang efisien:
- .from_tensor_slices(): dari NumPy array
- .map(): transformasi tiap elemen
- .shuffle(): acak data
- .batch(): kelompokkan
- .prefetch(): optimasi async loading
2. Keunggulan tf.data
- Bisa digunakan pada GPU/TPU
- Streaming data ukuran besar
- Kustomisasi penuh preprocessing
3. CSV Pipeline
- Gunakan TextLineDataset untuk membaca baris teks, lalu decode_csv() untuk parsing.
4. Image Pipeline
- read_file() → decode_jpeg() → resize() → normalisasi
- Sangat berguna untuk data gambar berukuran besar
5. TFRecord Format
- Format binary efisien untuk data besar dan multi-platform (standar TensorFlow)
- Format:
  + Data disimpan dalam Example → serialized → ditulis ke file .tfrecord
- Keunggulan:
  + Cepat dibaca
  + Ringan dan terkompresi
  + Platform-independent
6. Preprocessing Terintegrasi
- Pipeline dapat dikombinasikan dengan training untuk membuat proses end-to-end yang efisien dan scalable.
