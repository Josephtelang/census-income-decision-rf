# census-income-decision-rf  
# 🧑‍💼 Census Income Classification Using Decision Trees & Random Forests  

This project predicts whether a person earns **more than $50K per year** based on U.S. Census data. It includes **data preprocessing, feature engineering, model training using Decision Trees and Random Forests, hyperparameter tuning**, and detailed **evaluation and visualization**.

---

## 🔍 Problem Statement  

The goal is to build a **binary classification model** that predicts the `income` class:  
- `0` → Income ≤ $50K  
- `1` → Income > $50K  

---

## 📊 Dataset Overview  

- Based on the **UCI Adult Income Dataset**, widely used in ML benchmarks.  
- Contains features like age, education, occupation, hours worked per week, etc.  
- Cleaned and prepared for supervised classification.  

Key features used:
- `age`, `education-num`, `hours-per-week`, `capital-gain`, `occupation`, etc.  
- Categorical variables such as `workclass`, `education`, `relationship`, etc., were encoded.

---

## ⚙️ Project Workflow  

### 1. Data Cleaning  
- Handled missing values (represented as '?') and dropped irrelevant rows.  
- Converted income labels to binary (0 and 1).  

### 2. Feature Engineering  
- Applied Label Encoding to binary categorical columns.  
- Used **One-Hot Encoding** for multi-category features.  

### 3. Modeling  
- Trained a **DecisionTreeClassifier** and a **RandomForestClassifier** using scikit-learn.  
- Performed **hyperparameter tuning** with `GridSearchCV`.  
- Used `class_weight` to handle class imbalance.  

### 4. Evaluation  
- Compared models using **accuracy**, **confusion matrix**, and **classification report**.  
- Identified best hyperparameters using grid search.  

---

## 📈 Results  

- Best model: **Random Forest Classifier**  
- Achieved high validation accuracy  
- Learned feature importance and effects of model tuning  
- Final model generalizes well to unseen data  

---

## 🛠️ Technologies Used  

- Python 3  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  

---

## 📁 Project Structure  

##🚀 How to Run

###👉 Run in Google Colab
Click below to launch the notebook:
[Open in Colab](https://colab.research.google.com/drive/1SbOjxIa64R7Y0yPSCPO0ge_zfpRWJ6Sq#scrollTo=JsQEtQZtTcXT)

