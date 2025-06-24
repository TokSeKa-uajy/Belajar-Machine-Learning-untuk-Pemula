# Analisis Performa Kapal menggunakan Machine Learning

## Deskripsi Proyek
Proyek ini mengimplementasikan pipeline machine learning untuk menganalisis dan memprediksi performa kapal menggunakan kombinasi teknik clustering dan klasifikasi. Dataset yang digunakan berasal dari [Ship Performance Dataset](https://www.kaggle.com/datasets/jeleeladekunlefijabi/ship-performance-clustering-dataset).

## Tahapan Project

### 1. Clustering Analysis
- Implementasi K-Means clustering untuk mengelompokkan kapal berdasarkan karakteristik performa
- Fitur yang dianalisis mencakup:
  - Karakteristik Kapal: Ship_Type, Engine_Type
  - Metrik Performa: Speed, Engine Power, Efficiency
  - Faktor Operasional: Route_Type, Maintenance_Status
  - Indikator Finansial: Operational_Cost, Revenue_per_Voyage
- Normalisasi data menggunakan MinMaxScaler
- Label encoding untuk fitur kategorikal
- Visualisasi hasil clustering untuk validasi pemisahan kelompok

### 2. Classification Model
- Implementasi multiple classification models:
  - K-Nearest Neighbors (KNN)
  - Decision Tree
  - Random Forest
  - Support Vector Machine (SVM)
  - Naive Bayes
- Performa Model:
  - Hampir semua model mencapai akurasi sempurna (100%), kecuali KNN (~95%)
  - Precision, Recall, dan F1-Score yang sangat tinggi
  - Tidak ada indikasi overfitting (performa konsisten antara training dan testing)

## Teknologi yang Digunakan
- Python
- Libraries:
  - pandas & numpy: Data manipulation
  - scikit-learn: Machine learning algorithms
  - seaborn & matplotlib: Data visualization

## Hasil dan Insight
- Clustering berhasil memisahkan kapal ke dalam kelompok-kelompok yang distinct
- Model klasifikasi mampu memprediksi cluster dengan akurasi sangat tinggi
- Pemisahan yang jelas antar cluster (divalidasi melalui visualisasi dan evaluasi model)

## Future Improvements
- Pengujian pada data baru untuk validasi generalisasi model
- Implementasi untuk kasus real-time monitoring
- Penambahan fitur untuk kondisi ekstrem (cuaca ekstrem, mesin tua, rute dinamis)

## Lisensi
Data source: [Kaggle - Ship Performance Dataset](https://www.kaggle.com/datasets/jeleeladekunlefijabi/ship-performance-clustering-dataset)