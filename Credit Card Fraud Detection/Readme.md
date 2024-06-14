Fraud Detection Model with Logistic Regression
Step 1: Importing necessary libraries
This step imports all the required libraries for data handling, model training, evaluation, and visualization. Key libraries include pandas for data manipulation, scikit-learn for machine learning operations, imbalanced-learn for handling class imbalance, and matplotlib/seaborn for plotting.

Step 2: Load the dataset from Google Drive
The dataset fraudTest.csv is loaded from Google Drive using the Google Colab environment. Ensure to replace 'path_to_your_file.csv' with the actual path in your Google Drive where the dataset is located.

Step 3: Exploratory Data Analysis
Head of the dataset: Displays the first few rows of the dataset to understand its structure.
Checking for missing values: Summarizes the count of missing values in each column.
Descriptive statistics: Provides statistical information about the numerical columns in the dataset.
Record count for each label: Shows the distribution of the target variable (is_fraud) to understand class balance.
Step 4: Data Preprocessing
Separate features and target variable: Splits the dataset into features (X) and the target (y).
Encode categorical variables: Converts categorical variables into numeric format using Label Encoding.
Normalize numeric columns: Standardizes numeric features to have a mean of 0 and variance of 1.
Step 5: Balancing the dataset
Uses SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance by oversampling the minority class (is_fraud) to match the majority class.

Step 6: Train-test split
Splits the balanced dataset (X_balanced, y_balanced) into training and testing sets (80% training, 20% testing) to evaluate the model's performance.

Step 7: Model Training
Trains a Logistic Regression model on the training data with default parameters and a maximum of 1000 iterations.

Step 8: Model Evaluation
Accuracy scores: Calculates and prints the training and testing accuracies of the model.
Classification Reports: Displays precision, recall, F1-score, and support for both training and testing data to evaluate model performance.
Confusion Matrix: Visualizes the confusion matrix of the model predictions on the test set using a heatmap.
ROC Curve: Plots the Receiver Operating Characteristic (ROC) curve and computes the Area Under the Curve (AUC) score to assess the model's ability to distinguish between classes.
Precision-Recall Curve: Plots the precision-recall curve to evaluate the trade-off between precision and recall.
Conclusion
This workflow outlines the steps from data loading and preprocessing to model training and evaluation for a fraud detection problem using logistic regression. Each step is designed to ensure clarity and reproducibility of the model building process.


<img width="421" alt="Screenshot 2024-06-14 205328" src="https://github.com/SalmanAhmed03/Encryptix-MachineLearning/assets/124187700/6b449b66-f101-4b2b-9c67-968be29d8eb1">

<img width="433" alt="Screenshot 2024-06-14 205411" src="https://github.com/SalmanAhmed03/Encryptix-MachineLearning/assets/124187700/bef56ccd-6105-4b33-a1dc-738676e4fa3b">

<img width="425" alt="Screenshot 2024-06-14 205431" src="https://github.com/SalmanAhmed03/Encryptix-MachineLearning/assets/124187700/30750a21-521f-472b-ac32-adb7a8016cbc">


