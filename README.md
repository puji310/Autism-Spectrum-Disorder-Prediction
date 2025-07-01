# 🧠 Autism Prediction using Machine Learning

This project predicts the likelihood of Autism Spectrum Disorder (ASD) using structured clinical and behavioral data. The models are trained on screening survey responses and demographic data using machine learning algorithms in Jupyter Notebooks.

---

## 📂 Project Structure

| File | Description |
|------|-------------|
| `ML10000.ipynb` | Full dataset model with 10,000+ samples. Trains ML models and evaluates performance. |
| `ML_800.ipynb`  | Smaller-scale version for quick testing and debugging (800 samples). |

---

## 🧪 Features

- ✅ Predicts ASD likelihood based on questionnaire responses (A1–A10)
- 📊 Uses demographic and medical history features
- 🧠 Implements multiple ML models (Random Forest, SVM, Logistic Regression)
- 📈 Performance metrics: Accuracy, Confusion Matrix, ROC Curve
- 🔍 Exploratory Data Analysis (EDA)
- 📉 Works with small (800) and large (10,000) datasets

---

## 📊 Dataset Overview

- Collected from standard autism screening datasets
- Includes:
  - Behavioral screening answers (A1 to A10)
  - Age, gender, ethnicity
  - Family history, jaundice, and prior screenings
- Label: Class (ASD Positive or Negative)

> *Note: Data is anonymized and used only for academic purposes.*

---

## 🛠 Technologies Used

- Python 3.x
- Jupyter Notebook
- NumPy, Pandas
- Matplotlib, Seaborn
- Scikit-learn

---
## 🧪 Results

After training and testing various machine learning models on both the smaller (800 samples) and larger (10,000+ samples) datasets, the results were as follows:

| Model                        | Dataset Size | Accuracy | Precision | Recall | ROC-AUC |
| ---------------------------- | ------------ | -------- | --------- | ------ | ------- |
| Logistic Regression          | 800          | \~90%    | 89%       | 91%    | 0.92    |
| Random Forest                | 10,000       | \~96%    | 95%       | 97%    | 0.98    |
| Support Vector Machine (SVM) | 800          | \~88%    | 87%       | 89%    | 0.90    |

---

## 🔍 Observations:

- Random Forest consistently performed the best in terms of accuracy and robustness across both datasets.
- Logistic Regression gave competitive results with fewer false positives, making it suitable when interpretability is needed.
- SVM worked well on smaller datasets but was slightly less effective than ensemble methods on larger datasets.
  
----

## 📉 Visual Outputs:

- Confusion Matrices showed strong true positive rates, indicating accurate ASD classification.
- ROC Curves indicated excellent model separation ability (especially Random Forest with AUC ≈ 0.98).
- Feature Importance Analysis highlighted that some behavioral questions (A6, A9, A1) and demographic features (age, family history) significantly contributed to predictions.

---
