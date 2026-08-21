# 🚢 Titanic Survival Classification
 
A machine learning project predicting passenger survival on the Titanic, comparing five classification algorithms — Logistic Regression, KNN, Naive Bayes, Decision Tree, and SVM.
 
## 📋 Overview
 
Using the classic Titanic dataset, this project cleans passenger data, encodes categorical features, and trains multiple classifiers to predict survival based on attributes like class, sex, age, fare, and family size aboard.
 
## 🧠 Pipeline
 
1. Load data and drop redundant/leaky columns
2. Handle missing values (age, embarked)
3. Encode categorical features (`sex`, `embarked`)
4. Train-test split (80/20)
5. Train & evaluate 5 models, with feature scaling where needed
6. Validate results with 5-fold cross-validation
## 📈 Model Results
 
| Model | Test Accuracy | Cross-Val Accuracy |
|---|---|---|
| Logistic Regression | 80.45% | 79.24% |
| KNN | 82.12% | 79.80% |
| Naive Bayes | 77.65% | 78.57% |
| Decision Tree | 63.13% | 76.99% |
| **SVM (RBF kernel)** | **81.01%** | **82.83%** |
 
SVM delivered the most consistent performance across cross-validation, while KNN scored highest on the single test split.
 
## 🛠️ Tech Stack
 
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
 
## 📁 Files
 
| File | Purpose |
|---|---|
| `project.ipynb` | Data cleaning, model training, evaluation & cross-validation |
 
## ▶️ How to Run
 
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook project.ipynb
