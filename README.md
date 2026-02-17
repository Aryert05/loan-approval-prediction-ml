Loan Approval Prediction using Machine Learning
📌 Overview
This project builds classification models to predict whether a loan application will be approved based on demographic and financial features.
The objective is to evaluate different classification algorithms and compare their performance using multiple evaluation metrics.
📊 Dataset
491 loan applications
14 predictive features
Target variable: Loan_Status (Approved / Rejected)
Slight class imbalance (~70% approved)
⚙️ Data Preprocessing
Removed identifier columns (Loan_ID, Unnamed: 0)
Handled missing values:
Categorical features filled using mode
Numerical features filled using median
Applied one-hot encoding to categorical variables
Converted boolean columns to numeric format
Used stratified train-test split (80/20)
🤖 Models Implemented
1️⃣ Logistic Regression
Accuracy: 83.8%
AUC: 0.85
Strong probability separation ability
Stable overall performance
2️⃣ Random Forest Classifier
Accuracy: 80.8%
AUC: 0.82
Captured nonlinear feature interactions
📈 Evaluation Metrics
Accuracy
Precision
Recall
F1-Score
Confusion Matrix
ROC Curve & AUC
🔎 Key Insights
Logistic Regression performed best overall.
Class imbalance affects recall for rejected loans.
AUC provided better insight into model discrimination ability.
Accuracy alone is insufficient for classification evaluation.
🧠 Conclusion
Logistic Regression achieved the strongest performance with an AUC of 0.85, demonstrating reliable classification capability.
This project emphasizes proper evaluation of classification models beyond simple accuracy metrics.
🚀 Future Improvements
Hyperparameter tuning
Cross-validation
Class imbalance handling (SMOTE)
Model deployment using Streamlit
# loan-approval-prediction-ml
