# Credit Card Default Prediction
This project focuses on predicting whether a credit card holder will default on their payment in the upcoming month. Using a dataset named "Credit Default Dataset" prepared by PhD. Scholars under Department of Management Studies, IIT Roorkee, I applied a range of Machine Learning models — with a special emphasis on tree-based ensemble methods — to explore model performance, interpretability, and predictive power.
## Data Preprocessing
Started by cleaning the dataset, encoding categorical variables, and engineering meaningful features such as:
- Delay trends (from repayment history)
- Utilization ratios (credit usage behavior)
## Handling Class Imbalance
Since defaulters were underrepresented, we used SMOTE (Synthetic Minority Oversampling Technique) to balance the dataset, ensuring better model generalization.
## Model Training
Trained and fine-tuned a wide set of models using pipelines and RandomizedSearchCV:
- Logistic Regression
- Random Forest
- AdaBoost
- XGBoost
- LightGBM
- CatBoost
## Model Evaluation
Compared model performance using key metrics:
- F1 Score
- ROC AUC
- Precision & Recall
- Confusion Matrices
- ROC Curves
## Feature Importance
The Tree-based models allowed to identify the most impactful predictors. I compared feature importance rankings across models to draw consistent insights.
# Results & Insights
## Top Performing Models
- Random Forest and XGBoost provided the best trade-off between F1 score and recall, making them strong candidates for credit risk prediction.
### Most Influential Features
- Maximum payment delay
- Credit limit (LIMIT_BAL)
- Utilization ratios
- Payment history trends
## Demographic Insight
While demographic factors like age, sex, and education were less impactful on their own, they contributed meaningfully through interactions with behavioral features.
## Conclusion:
Tree-based ensemble models — especially under class imbalance — are highly effective for financial risk modeling in credit scoring scenarios.
## Dataset Overview
This dataset contains information on 30,000 credit card clients in Taiwan, tracked over a 6-month period like:
- Demographics:	AGE, SEX, EDUCATION, MARRIAGE
- Payment Behavior:	PAY_0 to PAY_6 (monthly repayment status)
- Financials:	BILL_AMT1–6, PAY_AMT1–6, LIMIT_BAL
- Target:	default.payment.next.month (1 = default, 0 = no default)

Source: Credit Default Dataset prepared by PhD. Scholars under DoMS, IIT Roorkee
