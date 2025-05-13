# Sentiment Analysis using SVM

Proyek ini merupakan implementasi analisis sentimen sederhana menggunakan algoritma **Support Vector Machine (SVM)** dengan **scikit-learn**. Dataset yang digunakan berasal dari GitHub repository publik, dan model ini memanfaatkan teknik **TF-IDF vectorization** untuk mengubah teks menjadi fitur numerik.

## 📂 Struktur File

- `main.ipynb`: Notebook utama yang berisi seluruh proses training, evaluasi, dan prediksi model.
- `vectorizer.sav`: File model vectorizer yang disimpan setelah training.
- `classifier.sav`: File model klasifikasi SVM hasil training.
- `README.md`: Dokumentasi proyek ini.

## 🛠 Teknologi dan Library

- Python 3.x
- Pandas
- Scikit-learn
- TfidfVectorizer
- Pickle
- Jupyter Notebook

## 🚀 Langkah-langkah Eksekusi

1. Clone repository ini:
    ```bash
    git clone https://github.com/fajarwiguna/svm-sentiment-analysis.git
    cd svm-sentiment-analysis
    ```

2. Buka notebook:
    ```bash
    jupyter notebook main.ipynb
    ```

3. Jalankan setiap cell satu per satu untuk melihat hasilnya.

## 🧪 Fitur Proyek

- **Preprocessing**: Mengubah teks ke bentuk numerik menggunakan TF-IDF.
- **Training**: Menggunakan SVM dengan kernel linear.
- **Evaluasi**: Menghasilkan classification report untuk metrik akurasi, precision, recall.
- **Prediksi**: Memprediksi label sentimen dari teks input manual.

## 📊 Hasil Evaluasi Model

| Label     | Precision | Recall | F1-score | Support |
|-----------|-----------|--------|----------|---------|
| Positive  | 0.919     | 0.910  | 0.915    | 100     |
| Negative  | 0.911     | 0.920  | 0.915    | 100     |

Model ini menunjukkan performa yang seimbang dalam mengklasifikasikan review positif dan negatif, dengan rata-rata F1-score sekitar **0.915**.

## 💡 Contoh Output Prediksi

### 🔍 Sampel dari Dataset
162: pos - "odin is a great high school basketball ..."
600: pos - "bob the happy bastard's quickie review..."
659: pos - "good films are hard to find these days..."
1099: neg - "so ask yourself what '8mm' is all about..."
337: pos - "will hunting (matt damon) is a genius..."


### 🧾 Teks Manual (User Input)
Review: SUPERB, I AM IN LOVE IN THIS PHONE
Prediction: pos

Review: Do not purchase this product. My cell phone blast when I switched the charger
Prediction: neg

Review: I received defective piece display is not working properly
Prediction: neg

Review: It's not even 5 days since I purchased this product.
I would say this a specially blended worst Phone in all formats.
Prediction: neg

## 📜 Lisensi

Proyek ini dibuat hanya untuk tujuan edukasi dan eksplorasi. Bebas digunakan dengan menyertakan atribusi.
