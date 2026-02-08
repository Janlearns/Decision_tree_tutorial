# Decision_tree_tutorial

## Apa Itu Decision Tree?

Decision Tree (Pohon Keputusan) adalah algoritma machine learning yang menggunakan struktur pohon untuk memprediksi nilai target. Setiap node dalam pohon mewakili sebuah fitur (kolom) dalam dataset, setiap cabang mewakili aturan keputusan, dan setiap leaf node mewakili hasil prediksi. Decision Tree mudah diinterpretasikan dan divisualisasikan, sehingga cocok untuk memahami bagaimana fitur-fitur dalam data mempengaruhi hasil prediksi.

## Cara Install dan Menggunakan

### Instalasi

Untuk menjalankan kode ini, Anda memerlukan Python dan beberapa library berikut:

-   pandas
-   scikit-learn
-   numpy

Anda dapat menginstall library-library ini menggunakan pip:

```bash
pip install pandas scikit-learn numpy
```

## Langkah-Langkah dalam Decision_tree.py

Kode `Decision_tree.py` melakukan langkah-langkah berikut:

1.  **Import Library:** Mengimpor library yang diperlukan seperti pandas, scikit-learn, dan numpy.
2.  **Siapkan Data:** Memuat dataset Iris menggunakan `datasets.load_iris()` dari scikit-learn dan mengubahnya menjadi pandas DataFrame.
3.  **Pisahkan Fitur dan Target:** Memisahkan fitur (data input) dari target (data yang ingin diprediksi).
4.  **Bagi Data menjadi Training dan Testing:** Membagi data menjadi set training dan testing menggunakan `train_test_split` dari scikit-learn.
5.  **Inisialisasi dan Latih Model:** Membuat objek `DecisionTreeClassifier` dan melatihnya menggunakan data training dengan `model.fit(X_train, y_train)`.
6.  **Prediksi:** Menggunakan model yang sudah dilatih untuk memprediksi target pada data testing dengan `model.predict(X_test)`.
7.  **Evaluasi Akurasi:** Menghitung akurasi model dengan membandingkan hasil prediksi dengan nilai target sebenarnya menggunakan `accuracy_score`.
