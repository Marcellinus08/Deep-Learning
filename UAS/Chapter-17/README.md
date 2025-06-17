Chapter 17: Autoencoders and GANs

1. Apa itu Autoencoder?
- Autoencoder adalah neural network yang dilatih untuk merekonstruksi inputnya.
- Struktur:
  + Encoder: mengubah input ke latent space
  + Decoder: mengubah representasi kembali ke bentuk asli
2. Tujuan Penggunaan
- Denoising
- Dimensionality reduction (nonlinear PCA)
- Anomaly detection
- Pretraining
3. Variational Autoencoder (VAE)
- Belajar distribusi dari data, bukan hanya titik
- Menghasilkan probabilistic latent representation
- Loss = reconstruction loss + KL divergence
4. Generative Adversarial Networks (GANs)
- Terdiri dari dua model:
  + Generator: membuat data palsu
  + Discriminator: membedakan data nyata vs palsu
- Latihan seperti game dua pemain:
  + Generator mencoba menipu Discriminator
  + Discriminator mencoba membedakan data palsu dari asli
5. Arsitektur Dasar DCGAN
- Gunakan Conv2DTranspose untuk Generator
- Gunakan Conv2D + BatchNorm + LeakyReLU untuk Discriminator
6. Tantangan Melatih GAN
- Sulit konvergen
- Mode collapse (generator hanya menghasilkan satu jenis output)
- Teknik: label smoothing, learning rate decay, minibatch discrimination
7. Aplikasi
- Image synthesis
- Super-resolution
- Style transfer
