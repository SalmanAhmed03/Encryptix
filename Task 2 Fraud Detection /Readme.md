Fraud Detection Model with Logistic Regression

Step 1: Importing necessary libraries This step imports all the required libraries for data handling, model training, evaluation, and visualization. Key libraries include pandas for data manipulation, scikit-learn for machine learning operations, imbalanced-learn for handling class imbalance, and matplotlib/seaborn for plotting.

Step 2: Load the dataset from Google Drive The dataset fraudTest.csv is loaded from Google Drive using the Google Colab environment. Ensure to replace 'path_to_your_file.csv' with the actual path in your Google Drive where the dataset is located.

Step 3: Exploratory Data Analysis Head of the dataset: Displays the first few rows of the dataset to understand its structure. Checking for missing values: Summarizes the count of missing values in each column. Descriptive statistics: Provides statistical information about the numerical columns in the dataset. Record count for each label: Shows the distribution of the target variable (is_fraud) to understand class balance. Step 4: Data Preprocessing Separate features and target variable: Splits the dataset into features (X) and the target (y). Encode categorical variables: Converts categorical variables into numeric format using Label Encoding. Normalize numeric columns: Standardizes numeric features to have a mean of 0 and variance of 1. Step 5: Balancing the dataset Uses SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance by oversampling the minority class (is_fraud) to match the majority class.

Step 6: Train-test split Splits the balanced dataset (X_balanced, y_balanced) into training and testing sets (80% training, 20% testing) to evaluate the model's performance.

Step 7: Model Training Trains a Logistic Regression model on the training data with default parameters and a maximum of 1000 iterations.

Step 8: Model Evaluation Accuracy scores: Calculates and prints the training and testing accuracies of the model. Classification Reports: Displays precision, recall, F1-score, and support for both training and testing data to evaluate model performance. Confusion Matrix: Visualizes the confusion matrix of the model predictions on the test set using a heatmap. ROC Curve: Plots the Receiver Operating Characteristic (ROC) curve and computes the Area Under the Curve (AUC) score to assess the model's ability to distinguish between classes. Precision-Recall Curve: Plots the precision-recall curve to evaluate the trade-off between precision and recall. Conclusion This workflow outlines the steps from data loading and preprocessing to model training and evaluation for a fraud detection problem using logistic regression. Each step is designed to ensure clarity and reproducibility of the model building process.


