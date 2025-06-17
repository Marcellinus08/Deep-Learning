Chapter 5: Support Vector Machines (SVM)

1. Konsep Inti
- SVM adalah model ML untuk klasifikasi dan regresi.
- Inti dari SVM: mencari hyperplane optimal yang memisahkan kelas dengan margin maksimum.
2. Linear SVM
- Cocok untuk dataset yang linearly separable
- Hard margin: tanpa toleransi kesalahan
- Soft margin: mengizinkan kesalahan kecil agar lebih toleran terhadap outlier
3. Nonlinear SVM
Gunakan kernel trick untuk memetakan data ke dimensi lebih tinggi tanpa benar-benar menghitung transformasinya.
Kernel Populer:
- Polynomial kernel: cocok untuk data yang berbentuk polinomial
- RBF (Gaussian): cocok untuk distribusi melingkar atau kompleks
4. Parameter Penting
- C: trade-off antara margin besar dan kesalahan kecil
   + Nilai besar: margin kecil, kurang toleran outlier
   + Nilai kecil: margin besar, toleran outlier
- gamma: memengaruhi area pengaruh masing-masing data (RBF)
  + Besar → model overfit
  + Kecil → model underfit
5. SVM untuk Regresi
- Support Vector Regression (SVR)
- Tujuannya adalah mencari hyperplane di mana data berada dalam margin toleransi ε.
- Kelebihan SVM:
  + Cocok untuk dataset kecil sampai menengah
  + Sangat efektif di ruang dimensi tinggi
  + Mendukung margin dan regularisasi bawaan
- Kekurangan:
  + Lambat di dataset besar
  + Sulit dituning
