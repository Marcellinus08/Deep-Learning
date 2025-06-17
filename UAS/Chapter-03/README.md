Chapter 3: Classification

1. Konsep Dasar
- Klasifikasi adalah tugas Machine Learning untuk memetakan input ke kategori (kelas).
- Dataset MNIST digunakan sebagai contoh — kumpulan gambar digit tangan 0–9.
2. Binary vs Multiclass
- Binary Classification: memisahkan dua kelas (misalnya: "apakah ini angka 5?")
- Multiclass: banyak kelas (0–9)
- Multilabel: lebih dari satu label per instance (misal: “angka ganjil” & “>7”)
3. Evaluasi Model
a. Confusion Matrix
- Tabel 2x2 untuk binary, NxN untuk multiclass
- Menunjukkan TP, FP, TN, FN
b. Precision & Recall
- Precision = TP / (TP + FP)
- Recall = TP / (TP + FN)
- Trade-off antara keduanya berguna saat kita peduli pada salah satu lebih dari lainnya.
c. F1 Score
- Harmonic mean dari precision dan recall
d. ROC Curve & AUC
- ROC: kurva antara TPR vs FPR pada berbagai threshold
- AUC: Area under curve → metrik untuk membandingkan model
4. Klasifikasi Multiclass
 One-vs-All (OvA): melatih satu classifier per kelas
- One-vs-One (OvO): melatih satu classifier untuk setiap pasangan kelas
5. Multilabel & Multioutput
- Multilabel: contoh memiliki beberapa label (e.g., digit ganjil DAN >7)
- Multioutput: target berupa vektor (e.g., output gambar)
6. Teknik-Teknik Tambahan
- Cross-validation (cross_val_score, cross_val_predict)
Decision function & threshold tuning
