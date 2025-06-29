# Telco-Customer-Churn---DT-RF

# Telco Customer Churn Prediction 📉

This project analyzes the **Telco Customer Churn** dataset to predict whether a telecom customer is likely to leave the service using tree-based machine learning models — **Decision Tree** and **Random Forest**.

> **Author**: Ejaz Ahmed  
> **Mentor**: Prof. Dr. Arghya Ray Sir  
> **Date**: June 29, 2025  
> **Dataset**: [Telco Customer Churn (Kaggle - Blastchar)](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## 📁 Project Overview

- Binary classification task: Predict churn (Yes/No)
- Supervised learning using:
  - `DecisionTreeClassifier`
  - `RandomForestClassifier`
- Dataset includes customer demographics, billing, and service subscription info.

---

## ⚙️ Tools & Libraries

- Python (Pandas, NumPy, scikit-learn)
- Matplotlib & Seaborn (for visualization)
- Graphviz & plot_tree (for model explainability)

---

## 🧠 Key Results

| Model           | Accuracy | Notes                                     |
|----------------|----------|-------------------------------------------|
| Decision Tree  | 72.42%   | Simpler, interpretable model              |
| Random Forest  | 78.82%   | Higher accuracy, better generalization    |

**Top Predictive Features**:
- `Contract`
- `tenure`
- `MonthlyCharges`
- `TechSupport`
- `InternetService`

---

## 📊 Visualizations

### 🌳 Decision Tree (Top 3 Levels)
![Decision Tree](images/decision_tree.png)

### 🌲 Random Forest - One Tree Example
![Random Forest Tree](images/random_forest_tree_0.png)

### 🔀 Feature Importance Comparison
![Feature Importance](images/feature_importance_comparison.png)

---

## 🌲 Visualizing Random Forest Internals

To explore how different trees in the Random Forest behave, we plotted **three trees side-by-side**:

![Random Forest Trees Side by Side](images/random_forest_trees.png)

Each tree is trained on a different bootstrap sample of the dataset and uses different features. This helps demystify the inner workings of the ensemble model.

---

## 📌 Business Insights

- Customers with **month-to-month contracts** are more likely to churn.
- Longer-tenure customers and those with **tech support** are more loyal.
- Churn is also higher among customers with **high monthly charges** and **no internet services**.

---

## 💡 Recommendations

- Offer bundled services like `TechSupport` and `OnlineBackup`
- Provide tenure-based loyalty discounts
- Target `Month-to-month` contract customers with personalized retention offers

---

## 🔧 How to Run

1. Clone the repository
2. Upload the CSV dataset (`WA_Fn-UseC_-Telco-Customer-Churn.csv`)
3. Run the notebook:
