Project: Banking Customer Churn Prediction 

Overview -
The Banking Customer Churn Prediction project focuses on predicting whether a customer will churn or not. By analyzing historical customer data, I aim to create a machine learning model that can predict churn, enabling the bank to take proactive steps to retain valuable customers. The project uses various machine learning models and techniques, including data preprocessing, feature engineering, and model evaluation, to understand and predict customer behavior.

Objective - The primary objectives of this project are to:
Understand the factors that contribute to customer churn using data analysis and feature importance.
Build machine learning models to predict customer churn with high accuracy.
Evaluate and compare model performance using appropriate metrics such as accuracy, AUC, and confusion matrices.
Identify actionable insights from the data to help the bank improve customer retention strategies.
Visualize model results and key insights for better decision-making.

About the Data -
The dataset contains customer information from a banking institution. The data includes demographic information, account details, and behavioral metrics. The dataset consists of both continuous and categorical variables. The target variable, Exited, indicates whether a customer has churned (1) or not (0).

Features Used - 
The dataset contains the following key features:
CreditScore: Customer’s credit score.
Age: Customer’s age.
Tenure: The number of years the customer has been with the bank.
Balance: The customer’s bank account balance.
NumOfProducts: The number of products the customer holds with the bank.
HasCrCard: Whether the customer has a credit card (1) or 0.
IsActiveMember: Whether the customer is an active member (1) or 0.
EstimatedSalary: Estimated salary of the customer.
Geography: The geographical location of the customer (categorical feature).
Gender: Gender of the customer (categorical feature).
Exited: Target variable indicating customer churn (1) or no churn (0).

Approach Used -
1. Data Preprocessing:
Handling Missing Data: Removed irrelevant columns and handled missing data where necessary.
Feature Encoding: Categorical variables such as Geography and Gender were one-hot encoded.
Feature Scaling: Standardized numerical features using StandardScaler.

2. Exploratory Data Analysis (EDA):
Visualized the distribution of features, especially the target variable (Exited), to understand the balance between churn and non-churn customers.
Investigated the correlation between features and the target variable.
Plotted histograms, boxplots, and pair plots to detect outliers, trends, and relationships.

3. Feature Engineering:
Created new features such as interaction terms (e.g., combining Age and Balance), based on domain knowledge to capture hidden patterns.
Handled skewed data distributions by transforming certain features like Balance and Age.

4. Modeling:
Evaluated four classification models:
Logistic Regression
Random Forest Classifier
XGBoost Classifier
AdaBoost Classifier
Used cross-validation to evaluate model performance and avoided overfitting.

Questions Explored - 
1. Which factors contribute most to customer churn?
2. Can we predict customer churn with a high degree of accuracy?
3. How do different machine learning models compare in terms of performance for this problem?
4. What actions can the bank take to retain high-risk customers based on model predictions?

Key Insights -
1. Model Performance: Among the models tested, Random Forest and XGBoost performed the best, with Random Forest achieving an AUC of 0.7151.
2. Feature Importance: Key features influencing churn include:
3. Balance: A low account balance is a significant factor in predicting churn.
4. Age: Older customers were less likely to churn.
5. IsActiveMember: Active members were less likely to churn.
6. Geography: Customers from Spain had a higher likelihood of churning compared to other countries.
7. Customer Segments: Customers with fewer products, lower balances, and less active accounts are more likely to churn.

Visualizations -
1. ROC Curves: Showed the trade-off between true positive and false positive rates.
2. Feature Importance Plot: Visualized the importance of each feature in predicting churn.
3. Confusion Matrices: Analyzed the distribution of correct and incorrect predictions.

Limitations -
Imbalanced Data: The dataset has a class imbalance (more non-churned than churned customers), which may affect the performance of models, particularly the recall of churned customers.
Limited Features: While we have several features, the dataset lacks behavioral data like customer interactions or satisfaction metrics, which could improve model performance.
No Real-Time Data: This analysis was done using historical data, and the churn behavior might change in the future based on evolving customer trends.
