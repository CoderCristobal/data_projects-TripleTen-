Customer Churn Prediction for Beta Bank
Project Overview
Beta Bank is facing a customer churn problem, where clients are leaving the bank on a monthly basis. Since retaining existing customers is more cost-effective than acquiring new ones, the objective of this project is to build a machine learning model that predicts whether a customer will leave the bank. By doing so, Beta Bank can take proactive steps to retain customers.

The primary goal is to develop a model with an F1 score of at least 0.59 on the test set. Additionally, the AUC-ROC metric will be measured and compared with the F1 score to assess the model's overall performance.

Project Details
Data Description
The dataset contains information on customers’ historical behavior, including their personal and financial details, as well as whether they have exited the bank. The key features are:

RowNumber: Data string index
CustomerId: Unique customer identifier
Surname: Customer's surname
CreditScore: Credit score of the customer
Geography: Country of residence
Gender: Customer's gender
Age: Customer's age
Tenure: Number of years the customer has been with the bank
Balance: Account balance
NumOfProducts: Number of banking products the customer uses
HasCrCard: Whether the customer has a credit card (1 = yes, 0 = no)
IsActiveMember: Whether the customer is an active member (1 = yes, 0 = no)
EstimatedSalary: Customer’s estimated salary
Exited: Target variable (1 = customer left the bank, 0 = customer stayed)
Methodology
Data Preprocessing:

Loaded the dataset and inspected the features.
Cleaned and prepared the data by encoding categorical features such as Geography and Gender, and scaling numerical features to ensure model compatibility.
Checked for missing values, which were not present.
Class Imbalance:

The target variable was imbalanced, with significantly fewer customers leaving than staying. This imbalance was addressed using two techniques:
Upsampling: Increased the number of samples in the minority class.
Class Weight Adjustment: Applied a balanced class weight to models.
Model Selection and Training: Several models were trained, including:

Logistic Regression
Decision Tree
Random Forest
Hyperparameters were tuned using grid search, and validation metrics were compared across models. Upsampling and adjusting class weights were used to handle the imbalance.

Best Model: After testing different models, the RandomForestClassifier with the following hyperparameters was selected as the best model:

class_weight='balanced'
max_depth=10
n_estimators=13
This model provided the best balance between precision and recall, achieving the required F1 score and strong AUC-ROC results.

Results
The final RandomForestClassifier model achieved a balanced F1 score, with relatively high recall. This indicates the model effectively identified customers likely to churn. However, the precision score was moderate, suggesting a reasonable proportion of true positives among all positive predictions.

The AUC-ROC value was also high, demonstrating that the model is effective at distinguishing between customers who will stay and those who will leave.

Conclusion and Recommendations
The RandomForestClassifier proved to be the most effective model in predicting customer churn for Beta Bank. With an F1 score surpassing the 0.59 threshold and a strong AUC-ROC value, the model is reliable for identifying customers at risk of leaving.

Ideas for Further Improvement:
Feature Engineering: Additional features, such as transaction frequency or recent account activity, could provide more context and improve model accuracy.
Real-Time Predictions: Implementing the model for real-time churn prediction can help Beta Bank take immediate action to retain customers.
Targeted Retention Strategies: The model can be integrated into marketing efforts, allowing the bank to offer personalized retention strategies for customers predicted to churn.
By implementing these improvements, Beta Bank can reduce churn, improve customer satisfaction, and increase revenue.
