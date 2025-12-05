# midterm-machine-learning
# 🚀 Midterm Exam: Machine Learning Portfolio

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange) ![Pandas](https://img.shields.io/badge/Library-Pandas-green)

## 👤 Student Identification
* **Name**: [Masukkan Nama Lengkap Anda Disini]
* **NIM**: [Masukkan NIM Anda Disini]
* **Class**: [Masukkan Kelas Anda, misal: IF-44-01]

---

## 📝 Purpose of the Repository
This repository is submitted to fulfill the **Midterm Exam** requirements for the Machine Learning course. The main objective is to demonstrate the ability to design and implement **End-to-End Machine Learning Pipelines** across three fundamental domains:
1.  **Regression**: Predicting continuous values (Song Release Year).
2.  **Clustering**: Unsupervised customer segmentation (Credit Card Usage).
3.  **Classification**: Fraud detection with imbalanced data.

---

## 📚 Project Overview & Results

### 1. Regression: Song Year Prediction
* **Goal**: Predict the release year of a song based on its audio features (timbre, signal characteristics).
* **Dataset**: `midterm-regresi-dataset.csv` (90 audio features).
* **Methodology**:
    * **Preprocessing**: Handling missing values with Mean Imputation and feature scaling using `StandardScaler`.
    * **Model**: **Ridge Regression** (L2 Regularization) to handle multicollinearity among audio features.
* **Evaluation Metrics**:
    * **RMSE (Root Mean Squared Error)**: [Masukkan Angka RMSE, contoh: 8.52] years.
    * **R² Score**: [Masukkan Angka R2, contoh: 0.65].

### 2. Clustering: Customer Segmentation
* **Goal**: Group credit card customers based on their spending and payment behavior to identify distinct user profiles.
* **Dataset**: `clusteringmidterm.csv`.
* **Methodology**:
    * **Preprocessing**: Removing ID columns, handling missing values, and Standard Scaling.
    * **Optimal K**: Determine the number of clusters using the **Elbow Method**.
    * **Model**: **K-Means Clustering**.
    * **Visualization**: Dimensionality reduction using **PCA (Principal Component Analysis)** to visualize clusters in 2D.
* **Results**:
    * **Number of Clusters**: [Masukkan Jumlah Cluster, contoh: 4] clusters.
    * **Insights**: Customers were segmented into groups such as "Big Spenders," "Installment Users," and "Cash Advance Users."

### 3. Classification: Fraud Detection
* **Goal**: Detect fraudulent online transactions in a highly imbalanced dataset.
* **Dataset**: `train_transaction.csv` (Labeled) & `test_transaction.csv` (Unlabeled).
* **Methodology**:
    * **Preprocessing**: Label Encoding for categorical features and handling missing values with a placeholder (-999).
    * **Handling Imbalance**: Utilized `class_weight='balanced'` in the model and Stratified Splitting.
    * **Model**: **Random Forest Classifier**.
* **Evaluation Metrics**:
    * **ROC-AUC Score**: [Masukkan Skor AUC, contoh: 0.85].
    * **Confusion Matrix**: Analyzed to minimize False Negatives.

---

## 📂 Repository Structure

How to navigate this repository:

```text
├── 📂 data/                   # (Optional) Folder containing csv files
├── 📓 1_Regression_Song.ipynb # End-to-end pipeline for Song Prediction
├── 📓 2_Clustering_Credit.ipynb # End-to-end pipeline for Customer Segmentation
├── 📓 3_Classification_Fraud.ipynb # End-to-end pipeline for Fraud Detection
└── 📄 README.md               # Project Documentation
