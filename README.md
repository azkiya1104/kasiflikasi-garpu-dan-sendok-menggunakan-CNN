# Klasifikasi Gambar Garpu dan Sendok dengan CNN VGG16
Proyek ini merupakan implementasi model klasifikasi gambar biner untuk membedakan antara objek garpu dan sendok. Kami menggunakan pendekatan transfer learning dengan model pra-terlatih VGG16 untuk mencapai akurasi tinggi dengan waktu pelatihan yang efisien.

1. Deskripsi Proyek
Tujuan dari proyek ini adalah membangun model Convolutional Neural Network (CNN) yang mampu mengklasifikasikan gambar garpu dan sendok secara otomatis. Metode yang digunakan adalah transfer learning dengan memodifikasi lapisan klasifikasi akhir dari model VGG16, yang sudah dilatih pada dataset ImageNet. Dataset kustom yang terdiri dari 200 gambar digunakan untuk melatih dan mengevaluasi model.

2. Dataset
Dataset yang digunakan dalam proyek ini terdiri dari 200 foto, dengan rincian 100 foto untuk kelas garpu dan 100 foto untuk kelas sendok. Gambar-gambar tersebut dikumpulkan dari berbagai sudut untuk meningkatkan variasi dan membantu model dalam generalisasi.

3. Implementasi Model
   - Arsitektur: VGG16 (pra-terlatih)
   - Teknik: Transfer Learning
   - Preprocessing: Resizing (224x224), augmentasi data (horizontal flip, color jitter, rotasi), dan normalisasi.
   - Pengaturan:
     ~ Epoch: 20
     ~ Batch Size: 32
     ~ Optimizer: AdamW
     ~ Loss Function: BCEWithLogitsLoss

4. Hasil
   Model yang diimplementasikan berhasil mencapai performa yang luar biasa pada data validasi:
   - Akurasi Validasi Akhir: 100%
   - Hasil Evaluasi: Confusion Matrix dan Learning Curve menunjukkan konvergensi yang sangat cepat dan tidak ada tanda-tanda overfitting yang signifikan.

5. Tautan Proyek
Kaggle Notebook: https://www.kaggle.com/code/negaakiyowoo/tugas-4

Dokumen : https://drive.google.com/drive/folders/1bX6F-E3HndJ_1XIiivnJmEJMrULNes5e?usp=sharing
