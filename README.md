#Loan Approval Prediction using Machine Learning

📌 Overview
This project builds classification models to predict whether a loan application will be approved based on applicant demographic and financial features.
The objective is to evaluate different classification algorithms and compare their performance using multiple evaluation metrics to ensure reliable decision-making.

📊 Dataset
Total records: 491 loan applications
Predictive features: 14
Target variable: Loan_Status (Approved = 1, Rejected = 0)
Slight class imbalance (~70% approved, ~30% rejected)

⚙️ Data Preprocessing
Removed identifier columns (Loan_ID, Unnamed: 0)
Handled missing values:
Categorical features filled using mode
Numerical features filled using median
Applied one-hot encoding to categorical variables
Converted boolean columns to numeric format
Used stratified 80/20 train-test split to preserve class distribution

🤖 Models Implemented
1️⃣ Logistic Regression (Baseline Model)
Accuracy: 83.8%
AUC: 0.85
Strong probability separation capability
Balanced and stable performance
2️⃣ Random Forest Classifier
Accuracy: 80.8%
AUC: 0.82
Captures nonlinear feature relationships
Slightly lower overall performance compared to Logistic Regression

📈 Evaluation Metrics
Models were evaluated using:
Accuracy
Precision
Recall
F1-Score
Confusion Matrix
ROC Curve
AUC Score
AUC was used to measure the model's ability to distinguish between approved and rejected applications beyond simple accuracy.

🔎 Key Insights
Logistic Regression outperformed Random Forest overall.
Class imbalance affects recall for rejected loans.
ROC-AUC provided deeper insight into classification performance.
Accuracy alone is not sufficient for evaluating classification models.

🧠 Conclusion
Logistic Regression achieved the strongest performance with:
Accuracy: 83.8%
AUC: 0.85
The model demonstrates reliable classification capability and strong class separation ability.
This project highlights the importance of proper preprocessing, stratified sampling, and multi-metric evaluation in classification problems.

🚀 Future Improvements
Hyperparameter tuning
Cross-validation
Handling class imbalance (e.g., SMOTE)
Model deployment using Streamlit or Flask
Feature importance and explainability analysis
