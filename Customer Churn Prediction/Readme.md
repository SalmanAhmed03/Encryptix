Customer Churn Prediction

This project aims to develop a model to predict customer churn for a subscription-based service or business. The dataset used includes historical customer data with features such as usage behavior and customer demographics. The following machine learning algorithms are used for prediction:

Logistic Regression

Random Forest

Gradient Boosting

Table of Contents
Installation
Data Preprocessing
Model Training
Model Evaluation
Results
License
Installation
To run this project, you need to have Python installed along with the required libraries. You can install the necessary dependencies using pip:

bash
Copy code
pip install pandas scikit-learn imbalanced-learn matplotlib seaborn
Data Preprocessing
Load the Data: The dataset is loaded from a CSV file.
Drop Unnecessary Columns: Remove columns that are not needed for the analysis (RowNumber, CustomerId, Surname).
Encode Categorical Variables: Convert categorical variables (Geography, Gender) into numerical values using label encoding.
Split the Data: Divide the data into training and testing sets (80% training, 20% testing).
Standardize the Features: Standardize the feature values to have a mean of 0 and a standard deviation of 1.
Model Training
Three machine learning models are trained using the processed data:

Logistic Regression: A simple yet effective linear model for binary classification.
Random Forest: An ensemble learning method that constructs multiple decision trees.
Gradient Boosting: An ensemble technique that builds models sequentially to minimize prediction errors.
Model Evaluation
Each model is evaluated using the following metrics:

Accuracy: The percentage of correct predictions.
Confusion Matrix: A table to describe the performance of the classification model.
Classification Report: Includes precision, recall, f1-score, and support.
ROC-AUC: The area under the ROC curve, which represents the model's ability to distinguish between classes.
Additionally, the ROC curve is plotted for the Logistic Regression model.

Results
The evaluation results for each model are printed, including accuracy, confusion matrix, and classification report for both training and testing data. The ROC curve for the Logistic Regression model is also plotted.

Example Output
Logistic Regression
yaml
Copy code
Evaluation for Logistic Regression
Accuracy: 0.866
Confusion Matrix:
 [[1547   48]
 [ 216  189]]
Classification Report:
               precision    recall  f1-score   support

           0       0.88      0.97      0.92      1595
           1       0.80      0.47      0.59       405

    accuracy                           0.87      2000
   macro avg       0.84      0.72      0.75      2000
weighted avg       0.86      0.87      0.85      2000
ROC Curve

Heatmaps


License
This project is licensed under the MIT License.
