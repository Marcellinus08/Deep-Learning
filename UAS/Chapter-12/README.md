Chapter 12: Custom Models and Training with TensorFlow

1. Mengapa Custom Model?
- Model sequential cocok untuk struktur linier.
- Untuk arsitektur kompleks (multi-input/output, conditional path, custom loss) gunakan subclassing.
2. Subclassing Model
- Turunan dari keras.Model, mendefinisikan layer di __init__ dan forward logic di call()
- Kelebihan:
  + Sangat fleksibel
  + Cocok untuk eksperimen
- Kekurangan:
  + Tidak bisa dipetakan otomatis (tidak model.summary() penuh)
  + Lebih sulit untuk debugging
3. Layer Custom
- Turunan dari keras.layers.Layer
- Implementasi build() untuk inisialisasi weight
- Implementasi call() untuk forward pass
4. Custom Loss
- Bisa subclass keras.losses.Loss
- Atau pakai fungsi Python biasa (custom metric/loss)
5. Manual Training Loop (advanced)
- Gunakan GradientTape untuk menghitung dan apply gradient
- Memberikan kontrol penuh untuk riset tingkat lanjut
