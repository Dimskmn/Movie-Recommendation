# Movie-Recommendation-System
# Peningkatan Akurasi Rekomendasi Film Menggunakan Neural Collaborative Filtering dengan Arsitektur RecommenderNet

[![SINTA 3](https://img.shields.io/badge/Journal-SINTA_3-blue.svg)](https://sinta.kemdikbud.go.id/)
[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?style=flat&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)

Proyek ini mengimplementasikan sistem rekomendasi film berbasis **Deep Learning** menggunakan pendekatan **Neural Collaborative Filtering (NCF)**. Riset ini telah dipublikasikan dalam Jurnal Algoritma (Institut Teknologi Garut) dan telah melalui proses _peer-review_.

## 📄 Publikasi Ilmiah

Penelitian terkait proyek ini dapat diakses secara resmi melalui tautan berikut:

- **Judul:** Peningkatan Akurasi Rekomendasi Film Menggunakan Neural Collaborative Filtering dengan Arsitektur RecommenderNet
- **Jurnal:** Jurnal Algoritma, Vol. 22 No. 2 (2025)
- **Akreditasi:** SINTA 3
- **DOI:** [10.33364/algoritma/v.22-2.3013](https://doi.org/10.33364/algoritma/v.22-2.3013)

---

## 🚀 Ringkasan Proyek

Tujuan utama dari proyek ini adalah mengatasi masalah _choice overload_ pada platform konten digital dengan menyediakan rekomendasi yang sangat personal. Berbeda dengan Collaborative Filtering tradisional (seperti Matrix Factorization), model ini memanfaatkan kekuatan Neural Network untuk mempelajari interaksi non-linear antara pengguna dan item.

### Fitur Utama:

- **Arsitektur RecommenderNet:** Menggunakan lapisan _Embedding_ untuk pengguna dan film guna menangkap fitur laten.
- **Deep Learning approach:** Menggunakan _dot product_ antara vektor laten ditambah dengan _bias_ untuk prediksi rating yang lebih akurat.
- **Optimized Performance:** Menggunakan Adam Optimizer dan Binary Crossentropy loss function pada data yang telah dinormalisasi.

---

## 📂 Dataset

Menggunakan dataset **MovieLens (ml-latest-small)**:

- **610** Pengguna unik.
- **9.724** Film unik.
- **100.836** Interaksi rating.

---

## 🛠️ Alur Kerja & Metodologi

1. **Data Preprocessing:**
   - Melakukan _label encoding_ pada `userId` dan `movieId`.
   - Normalisasi nilai rating ke rentang [0, 1] menggunakan Min-Max Scaling.
2. **Modeling:**
   - Membangun kelas `RecommenderNet` menggunakan Keras Model Subclassing.
   - Dimensi embedding: 50.
3. **Evaluation:**
   - Metrik utama: **Root Mean Squared Error (RMSE)**.
   - Pembagian data: 80% Training, 20% Validation.

---

## 📈 Hasil Eksperimen

Berdasarkan hasil pengujian yang tercantum dalam artikel ilmiah, model ini menunjukkan penurunan error (RMSE) yang signifikan selama proses pelatihan, membuktikan bahwa arsitektur RecommenderNet efektif dalam memprediksi preferensi pengguna secara akurat dibandingkan metode baseline.

---

## ⚙️ Instalasi & Penggunaan

1. Clone repository:
   ```bash
   git clone [https://github.com/Dimskmn/Movie-Recommendation.git](https://github.com/Dimskmn/Movie-Recommendation.git)
   ```
