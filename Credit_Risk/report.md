Purpose of the Analysis:
The purpose of this analysis is to develop machine learning models to predict the loan status based on financial information. The goal is to accurately classify loans as either healthy (0) or high-risk (1). The analysis aims to evaluate different models and assess their performance metrics to determine the most effective approach for loan status prediction.

Financial Information and Prediction Task:
The dataset used in the analysis contains financial information related to loans. The target variable is the "loan_status" column, which indicates whether a loan is healthy (0) or high-risk (1). The objective is to build models that can predict the loan status based on the available features.

Variables and Data Summary:

The "loan_status" variable: It consists of two classes - 0 and 1, representing healthy and high-risk loans, respectively. The count of each class is as follows:
Healthy loans (0): 18,765 instances
High-risk loans (1): 619 instances
Stages of the Machine Learning Process:
The analysis involved several stages of the machine learning process, including:

Data Loading and Exploration:
The lending data was loaded from a CSV file into a Pandas DataFrame.
The dataset was examined by displaying the head of the DataFrame to understand the structure and content of the data.

Data Preprocessing and Splitting:
The data was split into features (X) and the target variable (y).
The dataset was divided into training and testing sets using the train_test_split function, with a random_state of 1 for reproducibility.
Model Training and Evaluation (Model 1):
The LogisticRegression model was instantiated and fitted using the training data.
Predictions were made on the testing data.
Performance metrics such as accuracy, precision, recall, and F1-score were calculated and presented using the classification report and confusion matrix.
Data Resampling and Model Training (Model 2):
Random oversampling using the RandomOverSampler was performed to address class imbalance in the dataset.
The resampled data was split into training and testing sets.
Another LogisticRegression model was instantiated and trained using the resampled training data.
Predictions were made on the resampled testing data.
Performance metrics were calculated and reported using the classification report and confusion matrix.
Machine Learning Model Results:

Machine Learning Model 1:
Accuracy Score: 0.9520
Precision (Label 0): 1.00
Precision (Label 1): 0.85
Recall (Label 0): 0.99
Recall (Label 1): 0.91
F1-score (Label 0): 1.00
F1-score (Label 1): 0.88
Machine Learning Model 2:
Accuracy Score: 0.99
Precision (Label 0): 0.99
Precision (Label 1): 0.99
Recall (Label 0): 0.99
Recall (Label 1): 0.99
F1-score (Label 0): 0.99
F1-score (Label 1): 0.99

Summary:
Based on the results of the machine learning models, it is observed that both models achieved high accuracy and performance metrics. However, Model 2, which employed random oversampling to address class imbalance, demonstrated slightly better performance across all metrics.
