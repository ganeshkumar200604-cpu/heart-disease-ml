# Heart Disease Prediction using Machine Learning

## 📌 Problem
Predict whether a person has heart disease using clinical features.

## 📊 Dataset
- Heart Disease Dataset (UCI/Kaggle)
- Initial size: 1025 rows
- After cleaning: 302 rows (duplicates removed)

## ⚠️ Data Cleaning
- Removed 723 duplicate rows to avoid data leakage

## ⚙️ Preprocessing
- Numerical features → StandardScaler
- Categorical features → OneHotEncoder
- Used ColumnTransformer + Pipeline

## 🤖 Models Used
- Logistic Regression
- Random Forest

## 📈 Results
| Model | Accuracy | ROC-AUC |
|------|---------|--------|
| Logistic Regression | ~78% | ~0.86 |
| Random Forest | ~73% | ~0.85 |

## 📉 Key Insights
- Logistic Regression performed slightly better
- Random Forest overfit due to small dataset
- Data cleaning was critical

## 📊 ROC Curve
(Add screenshot here)

## 🚀 Technologies
- Python
- Pandas
- Scikit-learn
- Matplotlib

## 🧠 Learnings
- Importance of removing duplicates
- Avoiding data leakage
- Using pipelines properly