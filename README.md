# Proyek Prediksi Harga Rumah | House Price Prediction Project

Repositori ini berisi proyek *machine learning end-to-end* untuk memprediksi harga jual properti di Ames, Iowa. Proyek ini mencakup pembersihan data, *feature engineering*, pelatihan model, dan evaluasi.
<br>
*This repository contains an end-to-end machine learning project to predict property sale prices in Ames, Iowa. The project covers data cleaning, feature engineering, model training, and evaluation.*

---

## 🇮🇩 Bahasa Indonesia

### 📝 Deskripsi
Tujuan dari proyek ini adalah untuk membangun sebuah model regresi yang akurat menggunakan algoritma **XGBoost** untuk mengestimasi harga properti. Analisis mendalam dilakukan untuk memahami faktor-faktor kunci yang paling mempengaruhi harga sebuah rumah.

### 📁 Dataset
Dataset yang digunakan adalah **"Ames Housing Dataset"**.
- **Sumber:** Kaggle
- **Karakteristik:** Terdiri dari 2.930 baris dan 82 kolom fitur yang menjelaskan berbagai aspek properti, mulai dari luas tanah hingga kualitas garasi.

### ⚙️ Proses Pengerjaan
1.  **Pembersihan Data:** Menangani nilai yang hilang (*missing values*) dengan strategi imputasi (mengisi dengan median/modus) dan menghapus kolom dengan data kosong lebih dari 50% beserta menghapus kolom yang tidak relevan.
2.  **Feature Engineering:** Mengubah variabel kategorikal menjadi format numerik menggunakan *One-Hot Encoding* agar dapat diproses oleh model.
3.  **Pelatihan Model:** Melatih model menggunakan `XGBRegressor` pada data latih (80% dari total data).
4.  **Evaluasi Model:** Mengukur performa model pada data tes (20% sisa data) menggunakan metrik **R-squared (R²)** dan **Mean Absolute Error (MAE)**.
5.  **Analisis Fitur Penting:** Mengidentifikasi dan memvisualisasikan fitur-fitur yang paling berpengaruh dalam menentukan prediksi harga.

### 📊 Hasil
- Model berhasil mencapai skor **R-squared sebesar 0.9261** pada data tes.
- **Tiga Fitur Teratas** yang paling mempengaruhi harga jual adalah:
    1.  **Lot Frontage:** panjang lahan menghadap jalan.
    2.  **Lot Area:** luas tanah.
    3.  **MS SubClass:** tipe rumah.

### 🚀 Teknologi yang Digunakan
- **Python**
- **Pandas & NumPy:** Untuk manipulasi dan analisis data.
- **Scikit-learn:** Untuk pemrosesan data dan evaluasi model.
- **XGBoost:** Sebagai algoritma utama model regresi.
- **Matplotlib & Seaborn:** Untuk visualisasi data.

---

## 🇬🇧 English

### 📝 Description
The goal of this project is to build an accurate regression model using the **XGBoost** algorithm to estimate property prices. An in-depth analysis is conducted to understand the key factors that most significantly influence a house's price.

### 📁 Dataset
The dataset used is the **"Ames Housing Dataset"**.
- **Source:** Kaggle
- **Characteristics:** It consists of 2,930 rows and 82 feature columns describing various aspects of the properties, from lot area to garage quality.

### ⚙️ Workflow
1.  **Data Cleaning:** Handled missing values using imputation strategies (filling with median/mode) and dropping columns with more than 50% missing data and removing irrelevant columns.
2.  **Feature Engineering:** Converted categorical variables into a numerical format using *One-Hot Encoding* to be processed by the model.
3.  **Model Training:** Trained the model using `XGBRegressor` on the training set (80% of the total data).
4.  **Model Evaluation:** Measured the model's performance on the test set (the remaining 20%) using **R-squared (R²)** and **Mean Absolute Error (MAE)** metrics.
5.  **Feature Importance Analysis:** Identified and visualized the most influential features in determining price predictions.

### 📊 Results
- The model achieved an **R-squared score of 0.9261** on the test data.
- The **Top Three Most Influential Features** in predicting the sale price are:
    1.  **Lot Frontage:** length of the property facing the street.
    2.  **Lot Area:** land area.
    3.  **MS SubClass:** type of house.

### 🚀 Tech Stack
- **Python**
- **Pandas & NumPy:** For data manipulation and analysis.
- **Scikit-learn:** For data preprocessing and model evaluation.
- **XGBoost:** As the core regression model algorithm.
- **Matplotlib & Seaborn:** For data visualization.
