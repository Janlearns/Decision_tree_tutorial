# Decision Tree Tutorial

Tutorial komprehensif mengenai implementasi algoritma Decision Tree menggunakan Python dan scikit-learn.

---

## 📋 Daftar Isi

- [Pengenalan Decision Tree](#pengenalan-decision-tree)
- [Prasyarat Sistem](#prasyarat-sistem)
- [Instalasi dan Konfigurasi](#instalasi-dan-konfigurasi)
- [Struktur Proyek](#struktur-proyek)
- [Alur Implementasi](#alur-implementasi)
- [Penggunaan](#penggunaan)
- [Lisensi](#lisensi)

---

## Pengenalan Decision Tree

### Apa Itu Decision Tree?

Decision Tree (Pohon Keputusan) merupakan salah satu algoritma machine learning yang paling populer dan mudah dipahami. Algoritma ini menggunakan struktur pohon untuk melakukan prediksi terhadap nilai target berdasarkan fitur-fitur input.

**Komponen Utama Decision Tree:**

- **Node (Simpul):** Mewakili fitur atau atribut dalam dataset yang digunakan untuk membuat keputusan
- **Branch (Cabang):** Mewakili aturan keputusan yang menghubungkan satu node dengan node lainnya
- **Leaf Node (Node Daun):** Merupakan hasil prediksi atau klasifikasi akhir

**Keunggulan Decision Tree:**

- ✅ Mudah diinterpretasikan dan divisualisasikan
- ✅ Tidak memerlukan normalisasi data
- ✅ Dapat menangani data kategorikal maupun numerik
- ✅ Berguna untuk memahami pengaruh fitur terhadap hasil prediksi

---

## Prasyarat Sistem

Sebelum menjalankan proyek ini, pastikan sistem Anda memenuhi persyaratan berikut:

- Python 3.7 atau lebih tinggi
- pip (Python Package Manager)
- Memory RAM minimal 2 GB
- Disk space minimal 500 MB

---

## Instalasi dan Konfigurasi

### Langkah 1: Instal Library yang Diperlukan

Proyek ini memerlukan library-library berikut untuk menjalankan Decision Tree:

| Library | Versi | Deskripsi |
|---------|-------|-----------|
| pandas | >= 1.2.0 | Manipulasi dan analisis data |
| scikit-learn | >= 0.24.0 | Algoritma machine learning |
| numpy | >= 1.19.0 | Komputasi numerik |

#### Instalasi via pip:

```bash
pip install pandas scikit-learn numpy
```

#### Atau menggunakan requirements.txt:

```bash
pip install -r requirements.txt
```

---

## Struktur Proyek

```
Decision_tree_tutorial/
├── Decision_tree.py      # Script utama untuk implementasi Decision Tree
├── README.md             # Dokumentasi proyek
└── requirements.txt      # Daftar dependencies (opsional)
```

---

## Alur Implementasi

Script `Decision_tree.py` mengimplementasikan langkah-langkah berikut dalam mengembangkan model Decision Tree:

### 1. Impor Library
Mengimpor semua library yang diperlukan untuk pengolahan data dan machine learning

### 2. Persiapan Data
Memuat dataset Iris menggunakan `datasets.load_iris()` dari scikit-learn dan mengkonversinya menjadi pandas DataFrame untuk memudahkan manipulasi data

### 3. Pemisahan Fitur dan Target
Memisahkan fitur-fitur input (X) dari nilai target yang ingin diprediksi (y)

### 4. Pembagian Data Training dan Testing
Membagi dataset menjadi dua subset:
- **Training Set:** Digunakan untuk melatih model (biasanya 70-80% dari total data)
- **Testing Set:** Digunakan untuk mengevaluasi performa model (biasanya 20-30% dari total data)

### 5. Inisialisasi dan Pelatihan Model
Membuat instance `DecisionTreeClassifier` dan melatihnya menggunakan data training dengan memanggil method `fit(X_train, y_train)`

### 6. Prediksi
Menggunakan model yang telah dilatih untuk melakukan prediksi pada data testing dengan method `predict(X_test)`

### 7. Evaluasi Model
Mengevaluasi performa model dengan menghitung akurasi menggunakan `accuracy_score`, membandingkan hasil prediksi dengan nilai target sebenarnya

---

## Penggunaan

### Menjalankan Script

Untuk menjalankan Decision Tree tutorial, gunakan perintah berikut:

```bash
python Decision_tree.py
```

### Output yang Diharapkan

Script akan menampilkan:
- Akurasi model pada data testing
- Laporan klasifikasi lengkap
- Insights mengenai performa model

---

## Lisensi

Proyek ini bebas digunakan untuk keperluan pendidikan dan penelitian.


halo branch