# 🚀 Task 15: End-to-End ML Pipeline

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit_Learn-orange?logo=scikit-learn)

## 📖 Overview
**Task 15** simulates a real-world production environment. Instead of manual data cleaning, I built a **Scikit-Learn Pipeline** that automates preprocessing and modeling.

## ⚙️ The Pipeline Architecture
1.  **ColumnTransformer:** Splits data into two streams:
    * **Numerical Stream:** Imputes missing values (Median) → Scales Data (`StandardScaler`).
    * **Categorical Stream:** Imputes missing values (Most Frequent) → One-Hot Encodes (`OneHotEncoder`).
2.  **Classifier:** The processed data flows into a `RandomForestClassifier`.

## 📊 Results
* **Dataset:** Titanic (Raw, containing missing values and mixed types).
* **Accuracy:** ~82% on the test set.
* **Key Achievement:** Created a single `.pkl` file that takes raw CSV data as input and outputs predictions.

## 📂 Files
* [📓 Jupyter Notebook](./Task_15.ipynb)
* [💾 Production Pipeline (.pkl)](./titanic_pipeline.pkl)
