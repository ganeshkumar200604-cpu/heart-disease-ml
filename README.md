# ❤️ Heart Disease Prediction using Machine Learning

## 📌 Problem Statement
Heart disease is one of the leading causes of death worldwide. Early detection can help in timely treatment and reduce risks.  
This project aims to build a machine learning model to predict whether a person has heart disease based on clinical features.

---

## 📊 Dataset
- Source: UCI / Kaggle Heart Disease Dataset
- Initial size: **1025 rows**
- After cleaning: **302 rows**

### ⚠️ Data Cleaning (Important)
- Found **723 duplicate rows**
- Removed duplicates to prevent **data leakage**
- This step significantly improved model reliability

---

## ⚙️ Features Used

### Numerical Features
- age  
- trestbps (resting blood pressure)  
- chol (cholesterol)  
- thalach (max heart rate)  
- oldpeak  

### Categorical Features
- sex  
- cp (chest pain type)  
- fbs (fasting blood sugar)  
- restecg  
- exang  
- slope  
- ca  
- thal  

---

## 🔧 Preprocessing
- Numerical features → **StandardScaler**
- Categorical features → **OneHotEncoder**
- Combined using **ColumnTransformer**
- Built using **Scikit-learn Pipeline** (to avoid data leakage)

---

## 🤖 Models Used

### 1. Logistic Regression
- Simple and effective for small datasets
- Performs well on linearly separable data

### 2. Random Forest
- Captures nonlinear relationships
- Initially overfitted due to duplicate data

---

## 📈 Results

| Model | Accuracy | ROC-AUC |
|------|--------|--------|
| Logistic Regression | ~78.7% | ~0.86 |
| Random Forest | ~73.7% | ~0.85 |

---

## 📉 ROC Curve

![ROC Curve](roc_curve.png)

---

## 🔍 Key Insights
- Logistic Regression performed slightly better than Random Forest
- Random Forest overfitted when duplicate data was present
- Removing duplicates was **critical for correct evaluation**
- ROC-AUC provided better evaluation than accuracy

---

## 🧠 Learnings
- Importance of **data cleaning (duplicates removal)**
- Avoiding **data leakage**
- Using **pipelines for preprocessing + modeling**
- Comparing models using **ROC-AUC instead of only accuracy**
- Debugging real ML issues (overfitting, pipeline errors)

---

## 🛠️ Technologies Used
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
