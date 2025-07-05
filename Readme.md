# Credit Card Default Prediction
This project focuses on predicting whether a credit card holder will default on their payment in the upcoming month. Using a dataset of Taiwanese credit card clients, we apply a range of machine learning models — with a special emphasis on tree-based ensemble methods — to explore model performance, interpretability, and predictive power.
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
