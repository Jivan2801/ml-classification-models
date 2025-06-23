# Machine Learning Classification Assignment

This repository contains solutions to a comprehensive machine learning assignment covering classic algorithms such as the Perceptron, Naive Bayes, and Logistic Regression. The work includes both custom implementations and scikit-learn-based models, complete with evaluations and visualizations.

---

## 📁 Files Included
- `ml-classification-models.ipynb`: Main Jupyter Notebook with code and outputs
- `lab02_dataset_1.csv`: 3D dataset for Perceptron learning
- `lab02_dataset_2.xlsx`: Vehicle classification dataset for Naive Bayes
- `lab02_dataset_3.csv`: Loan classification dataset for Logistic Regression

---

## 📌 Problem 1: Perceptron Learning (Manual Implementation)
- Implemented `my_perceptron()` to find linear separator using perceptron algorithm.
- Dataset: 3D binary classification (`Positive`, `Negative`).
- Terminated training once misclassification rate < 1%.
- Visualized the data points and decision boundary in 3D.

---

## 📌 Problem 2: Naive Bayes Classification
- Used categorical features: `CAR_TYPE`, `OCCUPATION`, `EDUCATION`
- Encoded using `OrdinalEncoder`
- Trained `CategoricalNB` with various Laplace smoothing values.
- Identified best `alpha` = 100 with accuracy = 87.32%.
- Calculated predicted class probabilities and conditional probabilities `P(Xi | Yj)`.
- Visualized histogram of predicted class probabilities.
- Misclassification rate using custom threshold (0.6): 86.79%
- Evaluated predictions on custom test cases.

---

## 📌 Problem 3: Logistic Regression
- Used 8 numeric features initially.
- Scaled using `StandardScaler`, followed by 80-20 train-test split.
- Accuracy with numeric features: 82.44%
- Identified most important features by coefficient magnitude:
  - `loan_percent_income`
  - `loan_int_rate`
  - `loan_amnt`
- Added 3 top categorical features with highest correlation to target:
  - `previous_loan_defaults_on_file`
  - `loan_percent_income`
  - `loan_int_rate`
- Final model accuracy improved to: **82.69%**

---

## 🔧 Requirements
```bash
pandas
numpy
scikit-learn
matplotlib
seaborn
```

Install all dependencies using:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## 📷 Output Highlights
- 3D decision boundary for perceptron
- Naive Bayes class/feature probabilities
- Predicted class distributions and custom test predictions
- Logistic regression coefficient analysis
- Correlation heatmaps for feature selection

---

## 📬 Author
**Jivan Singh**  
M.S. Computer Science - Illinois Institute of Technology  
Patent Holder | Smart India Hackathon Winner

---

## 📜 License
This project is intended for academic and learning purposes.
