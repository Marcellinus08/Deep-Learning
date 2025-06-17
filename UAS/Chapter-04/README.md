Chapter 4: Training Models

1. Linear Regression
- Model linier sederhana: y = θ₀ + θ₁x
- Tujuan: mencari nilai parameter θ yang meminimalkan mean squared error (MSE).
- Normal Equation
- Solusi analitik untuk parameter: θ = (XᵗX)⁻¹Xᵗy
- Cepat dan akurat untuk dataset kecil.
2. Gradient Descent
- Metode iteratif untuk optimasi parameter.
Tipe Gradient Descent:
- Batch GD: menghitung gradien dari seluruh dataset (lambat).
- Stochastic GD (SGD): per instance, cepat, tapi fluktuatif.
- Mini-Batch GD: kompromi, paling sering dipakai.
3. Polynomial Regression
- Regresi yang menggunakan fitur x², x³, dll. Berguna untuk data nonlinier.
4. Learning Curves
- Grafik antara error vs jumlah data training.
- Menunjukkan overfitting (gap besar) atau underfitting (semua error tinggi).
5. Regularization (Menambahkan penalti untuk mencegah overfitting)
- Ridge (L2): penalti = α‖θ‖²
- Lasso (L1): penalti = α‖θ‖₁ → bisa menghasilkan fitur nol (feature selection)
- Elastic Net: kombinasi L1 dan L2
6. Early Stopping
- Menghentikan training lebih awal ketika performa validasi mulai menurun.
