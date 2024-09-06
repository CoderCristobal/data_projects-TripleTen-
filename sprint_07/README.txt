Megaline Plan Recommendation Model
Project Overview
Megaline, a mobile carrier, discovered that a significant portion of their subscriber base is still using legacy plans. To encourage the transition to their newer plans, Smart and Ultra, the company aims to build a predictive model that analyzes subscriber behavior and recommends the most suitable plan. The objective of this project is to develop a machine learning model that predicts whether a user should be on the Smart or Ultra plan based on their monthly usage.

The goal was to achieve the highest possible model accuracy, with a minimum accuracy threshold of 0.75. The analysis and model selection were carried out on a dataset of users who had already switched to one of the new plans.

Project Details
Data Description
The dataset provided by Megaline contains monthly behavior information for each user, including the following features:

calls: The number of calls made.
minutes: Total call duration in minutes.
messages: The number of text messages sent.
mb_used: Internet traffic used in megabytes (MB).
is_ultra: Whether the user is currently on the Ultra plan (1) or Smart plan (0).
Methodology
Data Exploration: We began by loading and inspecting the data, understanding its structure, and ensuring the data types were correctly formatted.

Data Splitting: The data was split into three sets:

Training Set: Used to train the model.
Validation Set: Used to tune hyperparameters.
Test Set: Used to evaluate the final model's performance.
Modeling and Hyperparameter Tuning: We experimented with multiple models, including decision trees, logistic regression, and random forests. Through hyperparameter tuning, the RandomForestClassifier emerged as the top performer.

Best Model:
RandomForestClassifier with:

max_depth=10
n_estimators=20
random_state=12345
This model provided the highest accuracy while meeting the minimum required threshold.

Model Evaluation: The model was evaluated on the test set to ensure it generalizes well. Various metrics, including accuracy, were calculated.

Visualizations
Model Comparison

Feature Importance

Results
After testing a variety of models and fine-tuning their hyperparameters, the RandomForestClassifier with the above configuration was selected for its ability to deliver a high level of accuracy. The model exceeded the accuracy threshold of 0.75 when tested on the validation set, demonstrating a reliable ability to predict whether a subscriber would benefit from the Smart or Ultra plan.

Key findings include:

Subscribers with higher internet usage (MB used) are more likely to be recommended the Ultra plan.
Total call duration and the number of text messages were less influential than expected in determining the plan, but still contributed to the overall model performance.
Conclusion and Suggestions
The project successfully produced a model that met the target accuracy and can now be used to recommend either the Smart or Ultra plan to subscribers based on their usage patterns.

Further Improvements:
Incorporate More Features: Additional behavioral data such as roaming charges, data overages, or international call duration might improve model accuracy.
Temporal Analysis: Analyzing trends over time (e.g., seasonal changes in data usage) could provide a more comprehensive recommendation system.
Real-Time Predictions: Implement the model in a real-time recommendation system to dynamically adjust plan suggestions based on live usage data.
By integrating these enhancements, Megaline could further optimize their service offerings and increase customer satisfaction, ultimately reducing churn and increasing conversions to the newer plans.











