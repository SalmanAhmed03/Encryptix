SPAM SMS Detection

This project builds a machine learning model to classify SMS messages as either spam or legitimate (ham). We utilize techniques like TF-IDF for text feature extraction and classifiers such as Naive Bayes, Logistic Regression, and Support Vector Machines (SVM) to identify spam messages.

Table of Contents

1.Introduction

2.Data

3.Preprocessing

4.Model Training and Evaluation

5.Results

6.Usage

7.License

Introduction


Spam detection is a crucial task in text processing. This project demonstrates how to build a spam detection model using Python and popular machine learning libraries. The model classifies SMS messages as spam or ham based on their content.

Data

The dataset used in this project is a collection of SMS messages labeled as ham (legitimate) or spam. The dataset includes two main columns:

label: The class of the message (ham or spam).

text: The content of the SMS message.



Usage

To use this code, follow these steps:

Clone the repository.

Ensure you have all required libraries installed (pandas, scikit-learn, seaborn, matplotlib).

Load the dataset and run the script to train and evaluate the models.

License

This project is licensed under the MIT License. See the LICENSE file for details.
