Credit Scoring Model using Machine Learning
Objective

To predict an individual’s creditworthiness using historical financial data by framing the problem as a binary classification task.

Dataset

German Credit Dataset (features only).
Since the original file did not contain a default label, a synthetic risk variable was created based on high credit amount and long loan duration to simulate risky borrowers.
This is for academic demonstration only.

Features

Age

Job

Housing

Saving Accounts

Checking Account

Credit Amount

Duration

Purpose

Sex

Categorical features were one-hot encoded.

Models Used

Logistic Regression (Binomial, L2 regularized, class-weight balanced)

Decision Tree

Random Forest

Evaluation Metrics

Precision

Recall

F1-Score

ROC-AUC

Special focus was given to Recall for the risky class (1), as missing a defaulter is more costly than rejecting a safe applicant.

Workflow

Data preprocessing and encoding

Synthetic target (Risk) creation

Train–test split with stratification

Feature scaling for Logistic Regression

Model training

Performance comparison using ROC-AUC and classification report

Conclusion

Logistic Regression provides interpretable probability estimates and serves as a strong baseline model for credit risk.
Random Forest generally achieves higher ROC-AUC due to its ability to capture non-linear patterns but lacks transparency.
Decision Trees offer rule-based interpretability but are less stable.

Technologies

Python

Pandas, NumPy

Scikit-learn

Google Colab
