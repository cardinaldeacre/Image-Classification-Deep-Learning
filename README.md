# Klasifikasi Gambar Pemandangan dengan Deep Learning

Proyek klasifikasi gambar untuk 6 kategori pemandangan. Dibangun dengan Keras & TensorFlow menggunakan arsitektur ResNet50 (Transfer Learning).

---

## 📝 Daftar Isi

- [Tentang Proyek](#-tentang-proyek)
- [Dibangun Dengan](#-dibangun-dengan)
- [Struktur Dataset](#-struktur-dataset)
- [Memulai](#-memulai)
- [Hasil](#-hasil)

---

## 📖 Tentang Proyek

Proyek ini bertujuan untuk membangun model *Deep Learning* yang mampu mengklasifikasikan gambar ke dalam 6 kategori pemandangan alam dan perkotaan yang berbeda. Model ini dilatih menggunakan teknik *Transfer Learning* dengan memanfaatkan arsitektur **ResNet50** yang telah terbukti andal dalam tugas pengenalan gambar.

Dataset yang digunakan adalah **Intel Image Classification** yang berisi ribuan gambar dengan label sebagai berikut:
- `buildings` (bangunan)
- `forest` (hutan)
- `glacier` (gletser)
- `mountain` (gunung)
- `sea` (laut)
- `street` (jalan)

---

## 🛠️ Dibangun Dengan

Proyek ini dibangun menggunakan teknologi dan pustaka berikut:

- **Python**: Bahasa pemrograman utama.
- **TensorFlow & Keras**: Kerangka kerja utama untuk membangun dan melatih model *Deep Learning*.
- **Scikit-learn**: Untuk evaluasi model, termasuk *classification report* dan *confusion matrix*.
- **Numpy**: Untuk operasi numerik dan manipulasi array.
- **Matplotlib & Seaborn**: Untuk visualisasi data dan hasil model.
- **Kaggle Notebook**: Lingkungan pengembangan yang digunakan.

---

## 📁 Struktur Dataset

Pastikan Anda memiliki struktur direktori dataset seperti di bawah ini agar kode dapat berjalan dengan baik. Direktori utama berisi folder `seg_train`, `seg_test`, dan `seg_pred` yang masing-masing memiliki subfolder untuk setiap kelas gambar.

```
intel-image-classification/
├── seg_pred/
│   └── seg_pred/
│       ├── 10004.jpg
│       └── ...
├── seg_test/
│   └── seg_test/
│       ├── buildings/
│       ├── forest/
│       ├── glacier/
│       ├── mountain/
│       ├── sea/
│       └── street/
└── seg_train/
    └── seg_train/
        ├── buildings/
        ├── forest/
        ├── glacier/
        ├── mountain/
        ├── sea/
        └── street/
```

---

## 🚀 Memulai

Untuk menjalankan proyek ini, Anda dapat mengikuti langkah-langkah berikut.

### Prasyarat

Pastikan Anda memiliki akses ke lingkungan yang mendukung Python dan pustaka yang disebutkan di atas. Cara termudah adalah dengan menggunakan Kaggle.

1.  **Unduh Dataset**: Dapatkan dataset dari [Intel Image Classification di Kaggle](https://www.kaggle.com/datasets/puneet6060/intel-image-classification).
2.  **Buka di Kaggle**: Unggah file `.ipynb` dari repositori ini ke Kaggle dan tambahkan dataset di atas ke notebook Anda.

### Menjalankan Notebook

1.  Pastikan *accelerator* di notebook Kaggle Anda diatur ke **GPU** untuk mempercepat proses pelatihan.
2.  Jalankan setiap sel kode di dalam notebook `image-classification-final-project-deep-learning.ipynb` secara berurutan dari atas ke bawah.

---

## 📊 Hasil

Model dievaluasi menggunakan data validasi untuk mengukur performanya. Metrik utama yang digunakan adalah akurasi. Selain itu, *confusion matrix* juga dibuat untuk menganalisis performa model pada setiap kelas secara lebih detail.

Tujuan dari proyek ini adalah mencapai akurasi setinggi mungkin dan meminimalkan kesalahan klasifikasi antar kelas.
