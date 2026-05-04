# 🩺 Analisis dan Pemodelan Prediksi Risiko Diabetes

Proyek *end-to-end* Data Science ini bertujuan untuk membangun model *Machine Learning* yang mampu memprediksi probabilitas seseorang didiagnosis mengidap diabetes berdasarkan metrik kesehatan klinis. 

Proyek ini disusun sebagai portofolio pemenuhan **9 Unit Kompetensi** pada skema sertifikasi profesi **Junior/Associate Data Scientist** (BNSP).

## 📂 Deskripsi Dataset
Dataset yang digunakan adalah **Pima Indians Diabetes Database** yang bersumber dari UCI Machine Learning Repository. Data ini berisi 768 sampel dengan 8 atribut medis (fitur) seperti tingkat Glukosa, Tekanan Darah, Insulin, BMI, dan Umur, serta 1 kolom target klasifikasi biner (Outcome).

## 🚀 Alur Kerja & Pemetaan Unit Kompetensi

Proyek ini dikerjakan secara sistematis mengikuti standar industri data, yang direpresentasikan dalam pemenuhan 9 Kriteria Unjuk Kerja:

1. **J.62DMI00.004.1 (Mengumpulkan Data):** Mengambil dataset berformat CSV melalui metode URL HTTP request.
2. **J.62DMI00.005.1 (Menelaah Data):** Melakukan *Exploratory Data Analysis* (EDA) untuk melihat statistik dasar dan menyajikan visualisasi matriks korelasi menggunakan Matplotlib & Seaborn.
3. **J.62DMI00.006.1 (Memvalidasi Data):** Mengonversi anomali nilai `0` pada fitur vital menjadi `NaN` dan mengevaluasi keseimbangan serta kecukupan data.
4. **J.62DMI00.007.1 (Menentukan Objek Data):** Menyeleksi 8 variabel independen (fitur medis) yang terbukti relevan dan mempertahankan 100% sampel baris.
5. **J.62DMI00.008.1 (Membersihkan Data):** Mengoreksi data yang kotor/hilang dengan strategi **Imputasi Median** untuk menjaga integritas data tanpa mengurangi volume sampel.
6. **J.62DMI00.009.1 (Mengkonstruksi Data):** Melakukan *Feature Engineering* (menambahkan fitur `Status_Obesitas` dari data BMI) dan menormalisasi skala angka menggunakan `StandardScaler`.
7. **J.62DMI00.010.1 (Menentukan Label Data):** Memverifikasi kelas diskrit biner dan memisahkan kolom target (`Outcome_Diabetes`) sesuai standar *Supervised Learning*.
8. **J.62DMI00.013.1 (Membangun Model):** Melakukan pemisahan *train/test split* (80:20) dan melatih algoritma **Random Forest Classifier** yang dipadukan dengan teknik *Hyperparameter Tuning* (`GridSearchCV`).
9. **J.62DMI00.014.1 (Mengevaluasi Hasil Pemodelan):** Menguji model menggunakan *testing set* riil dan memvalidasi performa akhir.

## 📊 Hasil Evaluasi & Kesimpulan

Berdasarkan batas toleransi akurasi minimum sebesar 70% yang ditetapkan pada skenario pengujian bisnis ini, model dinyatakan **LULUS UJI**:
* **Algoritma Utama:** Random Forest Classifier (Optimized)
* **Akurasi Akhir:** **74.03%**
* **Kesimpulan:** Setelah menangani anomali data melalui imputasi median dan menormalisasi fitur, model terbukti stabil dan secara fungsional siap digunakan sebagai sistem *early warning* skrining diabetes. 

## 🛠️ Teknologi & Library
- **Lingkungan Kerja:** Google Colab / Jupyter Notebook
- **Bahasa Pemrograman:** Python 3.12.13
- **Data Manipulation:** Pandas, NumPy
- **Visualisasi:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-Learn

## 👨‍💻 Penulis
**Abdi Arya Pratama**  
Mahasiswa Informatika | Universitas Pembangunan Nasional Veteran Jakarta (UPNVJ)
