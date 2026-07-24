# Heart Disease Prediction Analysis

An end-to-end data analysis and machine learning project that explores patient health data to identify risk factors for heart disease and build predictive models.

##  Project Overview

This project walks through a complete data science pipeline — from raw data to actionable insights — using a heart disease dataset sourced from Kaggle. The goal is to understand which clinical and lifestyle factors are most associated with heart disease, and to build a model that can predict risk based on patient attributes.

##  Objectives

- Explore and clean the dataset to understand its structure and quality
- Identify key risk factors through exploratory data analysis (EDA)
- Build and evaluate machine learning models to predict heart disease presence
- Summarize insights in a way that's useful for both technical and non-technical audiences

## 🗂️ Dataset

- **Source:** Kaggle
- **Description:** Patient-level clinical data including features such as age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, ECG results, max heart rate, exercise-induced angina, and target diagnosis (presence/absence of heart disease)

## 🛠️ Tools & Technologies

- **Language:** Python
- **Libraries:** pandas, NumPy, matplotlib, seaborn, scikit-learn (KNeighborsClassifier, LogisticRegression, RandomForestClassifier, GridSearchCV, RandomizedSearchCV)
- **Environment:** Jupyter Notebook (VS Code)

##  Project Workflow

1. **Data Cleaning** — Handled missing values, checked data types, removed inconsistencies
2. **Exploratory Data Analysis (EDA)** — Visualized distributions, correlations, and relationships between features and heart disease outcomes
3. **Feature Engineering** — Prepared and transformed features for modeling
4. **Model Building** — Trained and compared three classification models: K-Nearest Neighbors, Logistic Regression, and Random Forest
5. **Hyperparameter Tuning** — Optimized models using RandomizedSearchCV and GridSearchCV
6. **Model Evaluation** — Assessed performance using accuracy, precision, recall, F1-score, confusion matrix, and ROC curve
7. **Feature Importance** — Analyzed model coefficients to identify the strongest predictors of heart disease
8. **Insights & Recommendations** — Summarized key findings and their practical implications

##  Key Findings

- **Logistic Regression was the best-performing model**, achieving ~90% baseline accuracy and 88.5% after hyperparameter tuning (C = 0.191, solver = liblinear) — outperforming Random Forest (88.5% → 86.9% after tuning) and KNN (67.2% → 75.4% after tuning)
- The final model achieved **89% precision and 91% recall** for detecting heart disease cases, with an overall accuracy of 89% on the test set
- **Chest pain type (cp)** and **ST segment slope** were the strongest positive predictors of heart disease presence
- **Sex, thalassemia (thal), and number of major vessels (ca)** were the strongest negative predictors in this dataset
- Chest pain type showed the highest correlation (0.43) with heart disease diagnosis among all features

## 📁 Repository Structure

```
heart-disease-analysis/
│
├── Heart Disease.ipynb    # Main analysis notebook
├── .gitignore              # Files/folders excluded from version control
└── README.md               # Project documentation
```

##  How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/Dam1234seg/heart-disease-analysis.git
   ```
2. Open the folder in VS Code or Jupyter
3. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
4. Run `Heart Disease.ipynb` cell by cell

##  Author

**Damilola Oluwasegun**
Data Analyst | Aspiring ML Practitioner
[GitHub Profile](https://github.com/Dam1234seg)

---

*This project is part of an ongoing portfolio demonstrating skills in data cleaning, exploratory analysis, and predictive modeling using Python.*