# Thyroid-Prediction-System
# 🧠 Thyroid Disease Prediction & Analysis System

A comprehensive **multi-task machine learning framework** for thyroid disease diagnosis, hormone level prediction, and patient clustering using the UCI Thyroid Dataset.

---

## 📌 Overview

This project implements an end-to-end ML pipeline that:

* Classifies thyroid conditions (Normal, Hypothyroid, Hyperthyroid)
* Predicts hormone levels (TSH, T3, TT4)
* Discovers hidden patient patterns using clustering
* Provides a real-time interactive dashboard using Streamlit

The system combines **supervised learning, regression, and unsupervised learning** into a single unified framework for clinical decision support.

---

## 🚀 Features

### 🔍 1. Classification

* Models used:

  * Logistic Regression
  * Random Forest
  * CatBoost (Best Performer)
* Achieved:

  * ✅ **93.6% Accuracy**
  * ✅ **91.4% Recall (disease detection)**

---

### 📈 2. Hormone Level Prediction

* Predicts:

  * TSH
  * T3
  * TT4
* Performance:

  * TT4 → R² = 0.96 (Highly accurate)
  * T3 → R² = 0.71
  * TSH → R² = 0.35 (biological variability)

---

### 🧩 3. Clustering & Pattern Discovery

* Algorithms:

  * K-Means
  * Hierarchical Clustering
* Optimal clusters: **k = 3**
* Represents:

  * Hypothyroid
  * Hyperthyroid
  * Normal patients

---

### 📊 4. Interactive Dashboard

Built with **Streamlit**, includes:

* Patient input form
* Real-time prediction
* Probability visualization
* SHAP-based model interpretability
* PCA cluster visualization

---

## 🗂 Dataset

* Source: **UCI Machine Learning Repository**
* Size: ~3,100 patient records
* Features:

  * Demographics (Age, Sex)
  * Clinical indicators
  * Hormone levels (TSH, T3, TT4, T4U, FTI)

---

## ⚙️ Tech Stack

* **Languages:** Python
* **Libraries:**

  * Scikit-learn
  * CatBoost
  * Pandas, NumPy
  * Matplotlib, Seaborn
  * SHAP
* **Visualization:** Plotly, PCA
* **Deployment:** Streamlit

---

## 🧪 Methodology

1. Data Preprocessing

   * Missing value imputation (median/mode)
   * Feature scaling (StandardScaler)
   * Label encoding

2. Model Training

   * Stratified train-test split (80/20)
   * Hyperparameter tuning (GridSearchCV)

3. Evaluation Metrics

   * Classification: Accuracy, Precision, Recall, F1-score
   * Regression: R², MAE, RMSE
   * Clustering: Silhouette Score

---

## 📊 Results Summary

| Task           | Model    | Performance       |
| -------------- | -------- | ----------------- |
| Classification | CatBoost | 93.6% Acc         |
| Regression     | TT4      | R² = 0.96         |
| Clustering     | K-Means  | Silhouette = 0.58 |

---

## 💻 Installation

```bash
git clone https://github.com/your-username/thyroid-ml-project.git
cd thyroid-ml-project
pip install -r requirements.txt
```

---

## ▶️ Run the App

```bash
streamlit run app.py
```

---

## 📸 Screenshots (Optional)

* Classification Output
* SHAP Feature Importance
* PCA Cluster Visualization

*(Add images here if available)*

---

## 🔮 Future Work

* Add longitudinal patient data (time-series analysis)
* Include thyroid antibody markers
* Apply deep learning models
* Deploy using cloud (AWS/GCP)
* Clinical validation with real-world data

---

## 🙌 Acknowledgements

* UCI Machine Learning Repository
* IEEE Research Framework
* Contributors & academic support

