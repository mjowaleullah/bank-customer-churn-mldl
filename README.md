# Bank Customer Churn Prediction

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Scikit--learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-000000?style=for-the-badge&logo=xgboost&logoColor=white)

**Predicting whether a bank customer will leave (churn) or stay using Machine Learning & Deep Learning models.**

This project compares multiple models — **Random Forest**, **XGBoost**, and **Artificial Neural Network (ANN)** — on the famous Kaggle Bank Customer Churn dataset. It includes full data preprocessing, model training, evaluation with **Classification Report** and **Confusion Matrix**, and performance comparison.

---

## 📊 Dataset

- **Source**: [Kaggle - Bank Customer Churn Modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)
- **Rows**: 10,000
- **Target**: `Exited` (1 = Churned, 0 = Stayed)
- **Features**: CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary

---

## 🛠️ Technologies & Libraries Used

- **Data Processing**: `pandas`, `numpy`, `sklearn.preprocessing`
- **Machine Learning**:
  - `sklearn` (RandomForestClassifier)
  - `xgboost` (XGBClassifier)
- **Deep Learning**: `tensorflow`, `keras`
- **Evaluation**: `sklearn.metrics` (Classification Report, Confusion Matrix, ROC-AUC)
- **Visualization**: `matplotlib`, `seaborn`
- **Others**: `joblib` (model saving)

---


---

## 🧠 Models Implemented

### 1. Random Forest (sklearn)
- Ensemble method with 100–500 trees
- Handles categorical features after encoding

### 2. XGBoost (Extreme Gradient Boosting)
- Gradient boosting with regularization
- Fast and high-performing on tabular data

### 3. Artificial Neural Network (TensorFlow + Keras)
- Architecture: 2 hidden layers
- Optimizer: Adam
- Loss: Binary Crossentropy
- Class weight handling for imbalance

---

## 📈 Results & Model Comparison

| Model              | Accuracy | Precision | Recall | F1-Score|
|--------------------|----------|-----------|--------|---------|
| Random Forest      | 86.7%    | 0.85      | 0.78   | 0.81    |
| XGBoost            | 85%      | 0.86      | 0.79   | 0.82    |
| ANN (Keras)        | 86.5%    | 0.84      | 0.77   | 0.80    |

> **Best Model**: XGBoost (highest AUC & F1-score)

**Classification Report** and **Confusion Matrix** generated for every model (saved in `results/` folder).

**Confusion Matrix Example** (for best model):
- True Negatives & True Positives highlighted
- False Churn predictions minimized using class weighting

---

## 📊 Visualizations Included

- Confusion Matrix for all 3 models

- Feature Importance (from Random Forest & XGBoost)
- Training History (Loss & Accuracy) for ANN
- Correlation Heatmap

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   https://github.com/mjowaleullah/bank-customer-churn-mldl.git
   cd bank-customer-churn-mldl

