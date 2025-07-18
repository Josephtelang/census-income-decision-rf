# census-income-decision-rf
👨‍💼 census-income-decision-rf
🧠 Census Income Classification Using Machine Learning
This project predicts whether an individual's income exceeds $50K/year using U.S. census data. It demonstrates end-to-end classification using Decision Tree and Random Forest models, including data cleaning, preprocessing, hyperparameter tuning, evaluation, and insightful visualizations.

🔍 Problem Statement
Build a binary classification model to predict the income class:

0 → Income ≤ $50K

1 → Income > $50K

📊 Dataset Overview
Inspired by the UCI Adult Census Income dataset

Contains demographic and employment-related information

Key features include:

age, education_num, hours_per_week, capital_gain, occupation, marital_status, etc.

Preprocessed to have 56 features and ~22,000 rows

⚙️ Project Workflow
1. Data Cleaning
Handled missing values

Removed redundant and duplicate columns

2. Feature Engineering
Converted categorical variables with one-hot encoding

Ensured numeric columns were scaled if needed

3. Modeling
Trained DecisionTreeClassifier (baseline)

Trained RandomForestClassifier with tuned hyperparameters

Handled class imbalance with class_weight ({0:1, 1:1.5})

4. Hyperparameter Tuning
Used GridSearchCV on:

n_estimators, max_depth, max_leaf_nodes, max_samples, min_samples_split, class_weight

Evaluated using accuracy with cv=5

5. Evaluation
Compared train/test accuracy

Plotted confusion matrix

Analyzed feature_importances_ to identify key predictors

📈 Results
Best model: Random Forest

Validation accuracy: ~90%

Important predictors: education level, age, capital gain, occupation

Class imbalance handled successfully

Random Forest showed higher generalization compared to Decision Tree

🛠️ Technologies Used
Python 3

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Jupyter Notebook

📁 Project Structure
Copy
Edit
📦census-income-decision-rf
 ┣ 📜 Census_Income_Classification_Using_Decision_Trees_&_Random_Forests.ipynb
 ┣ 📄 README.md
 ┗ 📄 requirements.txt
🚀 How to Run
👉 Run in Google Colab
Click below to launch the notebook:
[Open in Colab](https://colab.research.google.com/drive/1SbOjxIa64R7Y0yPSCPO0ge_zfpRWJ6Sq#scrollTo=JsQEtQZtTcXT)

