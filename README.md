# ML-Model-for-Predicting-Customer-Loan-Eligibility
Bank Loan Approval Prediction Using Machine Learning  This project builds a machine learning model to predict whether a customer is eligible for a bank loan. The project includes full data preprocessing, visualization, model training, and evaluation using Stratified Cross-Validation.
Project Overview

Banks usually receive many loan applications, and manually evaluating each one is time-consuming.
This project uses a classification model to automate the loan approval process using customer information such as:

Gender

Married status

Education

Income

Loan amount

Credit history

Property area

etc.

Data Preprocessing

The following preprocessing steps are applied:

✔ Handle missing values
✔ Convert categorical columns to numeric (Label Encoding)
✔ Feature scaling using StandardScaler
✔ Train/test split
✔ Stratified 5-Fold Cross Validation to avoid bias
✔ Evaluation using Accuracy, Precision, Recall, and F1-score

Model Evaluation (Stratified K-Fold)

A 5-fold StratifiedKFold ensures the class ratio (Approved vs Not Approved) stays consistent in every split.

This gives a more fair and stable evaluation, especially for imbalanced datasets.

Final performance metrics are calculated using:

from sklearn.metrics import f1_score, accuracy_score, classification_report


The best model is selected based on highest F1-score.

Final Output

The notebook prints:

Best model performance

F1-score and accuracy

Confusion matrix

Cross-validation scores

Final prediction results

You can easily replace the model or add hyperparameter tuning.

How to Run

1.Clone the repository

2.Open Bank_Loan.ipynb

3.Run all cells in order

Replace dataset path if necessary


Author

Sajjad — Data Science & Machine Learning Learner
This project is part of your ML practice portfolio.
