# Credit Card Approval Prediction

This project focuses on predicting credit card approval decisions using machine learning. A Logistic Regression model is developed to classify applications as **approved or rejected** based on applicant attributes. The workflow demonstrates a complete and structured machine learning pipeline, including data loading, preprocessing, model training, evaluation, and hyperparameter tuning.

---

## Dataset

* **File:** `cc_approvals.data`
* **Records:** 690 applications
* **Features:** 15 input attributes (numeric and categorical)
* **Target:** Credit card approval decision (`+ / -`)
* **Missing values:** Represented by `?` and handled during preprocessing

---

## Methodology

### 1. Data Loading and Inspection

* Raw data loaded using Pandas
* Examined structure, data types, summary statistics, and missing values

### 2. Handling Missing Values

* Numeric features imputed using mean values
* Categorical features imputed using most frequent values

### 3. Data Preprocessing

* Categorical variables encoded using LabelEncoder
* Features prepared for modeling
* Split into training and testing sets
* Min-Max normalization applied for feature scaling

### 4. Model Training

* Logistic Regression trained on scaled training data
* Default hyperparameters used as baseline

### 5. Model Evaluation

* Metrics used: Accuracy and Confusion Matrix
* Test Accuracy: 84.21%
* The model demonstrates strong predictive capability with balanced performance across approval and rejection classes

### 6. Hyperparameter Tuning

* Grid Search with 5-fold cross-validation applied
* Parameters tuned: `max_iter`, `tol`
* Best Cross-Validated Accuracy: ~85.1%
* Best Parameters:
  `max_iter = 100`
  `tol = 0.01`

---

## Results Summary

* Logistic Regression provides reliable performance for credit approval prediction
* Proper preprocessing and scaling significantly improve model stability
* Hyperparameter tuning yields consistent but marginal performance gains

---

## Project Structure

```
Credit-Card-Approval-Prediction/
│
├── credit_card_approval_prediction.ipynb
├── cc_approvals.data
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
```

**requirements.txt**

```
pandas==2.3.3
numpy==2.3.3
scikit-learn==1.3.3
```

---

## How to Run

1. Clone the repository
2. Install dependencies
3. Open the notebook `credit_card_approval_prediction.ipynb`
4. Run all cells sequentially

---

## Pro Tip for Recruiters / Collaborators

This project demonstrates a complete machine learning workflow applied to a real-world binary classification problem. It highlights practical skills in:

* Data cleaning and preprocessing of mixed numerical and categorical data
* Handling missing values using statistical and frequency-based methods
* Feature encoding and normalization for model readiness
* Building and evaluating classification models using Logistic Regression
* Model validation using accuracy metrics, confusion matrices, and cross-validation
* Hyperparameter tuning with Grid Search to improve model performance

This repository demonstrates a machine learning workflow for a real-world problem with clear, interpretable models. It highlights practical skills in **data science and machine learning.**

---

**Author:**
Sumayya Samreen, M.Sc. in Artificial Intelligence
Focused on applied machine learning, data-driven decision systems, and building reliable models for real-world classification tasks.