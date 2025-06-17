Chapter 16: Natural Language Processing with RNNs and Attention

1. Natural Language Processing (NLP)
- Bidang yang mempelajari interaksi antara komputer dan bahasa manusia.
- Task NLP umum:
  + Text classification
  + Named Entity Recognition (NER)
  + Machine translation
  + Text generation
2. Preprocessing Teks
- Tokenization: memecah kalimat menjadi kata/token
- Padding: agar semua input memiliki panjang yang sama
- Vocabulary: memetakan kata ke ID numerik
3. Embedding Layer
- Mengubah ID kata ke vektor dense (representasi semantik)
- Pre-trained embedding: GloVe, Word2Vec
4. Recurrent Networks
- LSTM & GRU: mengatasi vanishing gradient pada long sequences
- Bidirectional: memproses dari dua arah (→ dan ←), lebih kontekstual
5. Attention Mechanism
- Memungkinkan model "memperhatikan" bagian penting dari input saat memprediksi
- Digunakan secara luas dalam transformer dan seq2seq model
- Inti attention:
  + [ Attention(Q, K, V) = softmax\left(\frac{QK^T}{\sqrt{d_k}}\right)V ]
6. Arsitektur Modern NLP
- Transformer (BERT, GPT, T5) menggantikan RNN dalam banyak tugas
- Fokus bab ini masih pada RNN + attention sebagai dasar
7. Tips
- Padding → gunakan mask_zero=True jika embedding
- Gunakan Bidirectional(LSTM(...)) untuk hasil lebih baik
Attention bisa dibuat sendiri atau pakai keras.layers.Attention()
