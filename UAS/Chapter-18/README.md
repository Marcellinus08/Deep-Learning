Chapter 18

1. Policy Gradient (PG)
- Tujuan
  + Melatih model secara langsung untuk mempelajari kebijakan (policy), yaitu distribusi probabilitas atas tindakan pada setiap keadaan.
- Proses Pembelajaran:
  + play_one_step:
    - Mengambil satu langkah dari environment.
    - Menghitung loss terhadap aksi yang diambil, dan memperoleh gradien parameter.
  + play_multiple_episodes:
    - Melakukan iterasi beberapa episode dan menyimpan semua reward & gradien.
  + discount_rewards:
    - Menghitung reward terdiskonto untuk mempertimbangkan masa depan.
    - discount_and_normalize_rewards:
  + Training Loop:
    - Menggabungkan gradien dari semua episode secara tertimbang oleh reward terdiskonto.
    - Gradien diterapkan pada parameter model.
- Visualisasi:
  + Kurva reward rata-rata ditampilkan selama pelatihan untuk melihat perkembangan kebijakan.

2. Deep Q-Network (DQN)
Tujuan
Belajar fungsi nilai aksi (action-value function, atau Q-value) dan memilih aksi berdasarkan nilai tertinggi.



Strategi:
Epsilon-Greedy Policy:

Memungkinkan eksplorasi aksi secara acak untuk menghindari konvergensi lokal.
Epsilon menurun selama pelatihan untuk eksploitasi lebih besar.
Replay Memory:

Menghindari korelasi antar langkah dengan menyimpan pengalaman sebelumnya.
Sampling acak pengalaman untuk pembaruan model.
Training Step:

Target Q dihitung dari reward + diskonto * max Q pada next state.
Loss antara Q saat ini vs target Q dihitung dan digunakan untuk backpropagation.
Training Loop:

Setiap episode dilakukan, reward dikumpulkan.
Setelah sejumlah episode, parameter diperbarui dari replay buffer.
