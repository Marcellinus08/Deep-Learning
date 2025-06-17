Chapter 15: Processing Sequences Using RNNs and CNNs

1. Data Sekuensial
- Contoh: time series, teks, audio
- Karakteristik: urutan data penting (berurutan)
2. Recurrent Neural Networks (RNN)
- Cocok untuk data urutan
- Setiap waktu langkah (t) menerima input + state dari t-1
- Output tergantung pada input saat ini dan konteks masa lalu
3. Jenis RNN
- SimpleRNN: dasar, rentan vanishing gradient
- LSTM: menangani long-term dependencies
- GRU: lebih ringan dari LSTM, performa mirip
4. CNN untuk Time Series
- Bisa digunakan untuk mengekstrak pola lokal
- Biasanya lebih cepat dilatih
- Cocok untuk forecasting pendek
5. Tips
- Gunakan return_sequences=True jika ingin menghubungkan beberapa RNN
- TimeSeriesGenerator dari Keras dapat membantu membuat window data
- Untuk forecasting, bisa gunakan pendekatan sliding window
6. Problem Umum
- Vanishing gradient pada long sequences
- Latency inference yang tinggi untuk RNN
-Untuk sequence panjang: pakai LSTM/GRU + attention (bab 16)
