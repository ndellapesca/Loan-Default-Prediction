# Loan-Default-Prediction
In this project, I leveraged a loan dataset to predict the probability of defaulting using various machine learning techniques. After performing variable selection, I fitted and compared multiple models based on their accuracy and AUC scores. Additionally, I implemented a user input feature that allows banks, companies, or lenders to input specific variables and obtain a default probability for potential borrowers.
Each model attempts to balance the trade-off between complexity, accuracy, and the risk of overfitting. This tool is valuable for enhancing decision-making in loan approvals and can aid companies and banks in conducting more effective risk analysis.

| Method                | Accuracy | Sensitivity | Specificity | AUC   |
|-----------------------|----------|-------------|-------------|-------|
| Logistic Regression   | 0.6149   | 0.6006      | 0.6297      | 0.6792|
| Random Forest         | 0.7777   | 0.7871      | 0.7680      | 0.8560|
| xgBoost               | 0.8129   | 0.8334      | 0.7920      | 0.8962|
| Support Vector Machine| 0.7331   | 0.7618      | 0.7033      | 0.8035|

One reason the Logistic Regression model has lower metrics compared to the other models could be due to the nonlinearity of the data.
The Random Forest model appears to strike a good balance between complexity and accuracy with a relatively low risk of overfitting.
While being more accurate, the xgBoost model is prone to overfitting due to the complexity of the model. Early stopping and sensitivity parameter tuning were utilized to counteract this.
While being accurate, the kernel for the Support Vector Machine struggles to capture the entirety of the data, which could be a reason that it did not perform as well as the other black box models.
