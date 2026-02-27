
# Liquefaction Potential Index (LPI) Prediction Using Gaussian Process Regression

## 📌 Project Overview
This research presents a Machine Learning-based framework to predict Liquefaction Potential Index (LPI) using Gaussian Process Regression (GPR). The model evaluates earthquake-induced liquefaction potential for multiple earthquake magnitudes (Mw 6.5, 7.0, and 7.5).

This work was developed as part of an undergraduate thesis in Civil Engineering.

---

## 🎯 Objectives
- Develop a predictive model for LPI using borehole data
- Compare multiple Machine Learning algorithms
- Identify the best-performing model
- Generate magnitude-wise LPI predictions

---

## 📊 Dataset Description
The dataset includes:

- Borehole ID
- Latitude & Longitude
- Depth-wise SPT-N values
- Peak Ground Acceleration (PGA / amax)
- Calculated LPI values

Earthquake scenarios used:
- Mw 6.5 (0.25g)
- Mw 7.0 (0.28g)
- Mw 7.5 (0.31g)

---

## ⚙️ Methodology

### 1️⃣ Data Preprocessing
- Removal of duplicate rows
- Removal of zero-variance columns
- Outlier removal using IQR method
- Robust scaling

### 2️⃣ Feature Engineering
- Dense layer count derived from SPT values

### 3️⃣ Dimensionality Reduction
- Principal Component Analysis (PCA)

### 4️⃣ Model Training
The following models were evaluated:

- Linear Regression
- Support Vector Machine (SVM)
- Random Forest
- Gradient Boosting
- XGBoost
- LightGBM
- Gaussian Process Regression (GPR)

### 5️⃣ Model Evaluation Metrics
- R² Score
- Root Mean Square Error (RMSE)
- Mean Absolute Error (MAE)

---

## 🏆 Best Model
Gaussian Process Regression (GPR) showed the best predictive performance among all tested models.

---

## 📁 Output Files
The final prediction files include:

- `Final_GPR_LPI_Predictions_6.5.xlsx`
- `Final_GPR_LPI_Predictions_7.0.xlsx`
- `Final_GPR_LPI_Predictions_7.5.xlsx`

Each file contains:
- Borehole ID
- Latitude
- Longitude
- Predicted LPI
- Actual LPI

---

## 🚀 How to Run

1. Open the notebook in Google Colab
2. Upload required dataset files
3. Run all cells sequentially
4. Output prediction files will be generated automatically

---

## 🛠 Tools & Libraries
- Python
- Scikit-learn
- Pandas
- NumPy
- XGBoost
- LightGBM

---

## 📚 Academic Context
This project focuses on earthquake-induced soil liquefaction modeling using Machine Learning techniques and is developed as part of a Civil Engineering undergraduate thesis.

---

### Author
Your Name  
Department of Civil Engineering  
University Name  
Year
