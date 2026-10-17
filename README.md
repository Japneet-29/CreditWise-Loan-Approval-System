# CreditWise Loan Approval System

## Overview
CreditWise is a machine-learning project that explores historical loan application data and predicts the recorded loan approval outcome. It includes data cleaning, exploratory data analysis, preprocessing, model comparison, cross-validation, hyperparameter tuning, and final model evaluation.

## Dataset
The notebook expects `loan_approval_data.csv` in the same folder as the notebook.

The dataset includes applicant and financial attributes such as income, employment status, credit score, existing loans, debt-to-income ratio, savings, loan amount, loan purpose, and the `Loan_Approved` target.

**Before publishing the CSV:** confirm that you have permission to redistribute it and that it contains no personal or confidential applicant information. If not, do not commit the dataset; explain in this README how authorized users can obtain it.

## Models
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes

The notebook evaluates models with accuracy, precision, recall, F1-score, ROC-AUC, classification reports, and confusion matrices. Model selection uses cross-validation on the training data, followed by evaluation on a held-out test set.

## Setup
1. Install Python 3.
2. Clone or download this repository.
3. Install dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Place `loan_approval_data.csv` beside the notebook.
5. Open `CreditWise_revised_concise.ipynb` in VS Code or Jupyter and run all cells.

## Important limitations
This is an educational ML project, not a production credit-decision system. Historical approval labels can reflect prior bias, and model performance on this dataset may not generalize to other applicants or future conditions. Real lending use would require appropriate legal and fairness review, explainability, privacy and security controls, monitoring, and human oversight.

## Reproducibility
The notebook uses a fixed random seed for the train-test split and cross-validation. Metrics can still vary with dataset changes, library versions, and data characteristics.
