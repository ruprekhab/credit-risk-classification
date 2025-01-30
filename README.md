# credit-risk-classification
## Purpose of the analysis:
The objective of this analysis is to train and evaluate a machine learning model to classify loans as either 'healthy' or 'high-risk' based on borrowers' financial data.
## About the Dataset:
The dataset contained the following financial information of the borrowers:
* Loan size
* Interest rate
* Borrower income
* Debt to income ratio
* Number of accounts
* Derogatory marks
* Total debt. 
The target variable (y) represents the loan status, indicating whether a loan is classified as 'healthy' or 'high-risk.' 

## Machine Learning Model Used:
Logistic Regression, a classification algorithm, was used for this analysis. It estimates the outcome based on the input features. 

## Stages of Machine Learning Process:
* **Data Preparation:** The Data was loaded into a Pandas DataFrame. The features (X) and target variable (y) were separated. Then, the data was split into training and testing sets using train_test_split().
* **Model selection and training:** Logistic Regression was chosen as the lassification algorithm. The model was initialized with random_state= 1 and trained using fit() on the training data. Predictions were made on the test dataset using predict().

* **Evaluation:** The model was evaluated using a confusion matrix and a classification report. Key performance metrics like precision, recall and accuracy were analyzed

## Result Summary:
* Accuracy score: 0.99
* Precision score:
    - Healthy loan: 1.00
    - High Risk: 0.84
* Recall score:    
    - Healthy loan: 0.99
    - High Risk: 0.94

## Conclusion:         
The Logistic Regression model performed exceptionally well, achieving 99% overall accuracy. 

<p> For healthy loans, with a perfect precision score of 100% and almost perfect recall score of 99%, the model almost never misclassified healthy loans.</p>

<p> For high risk loans, with a precision score of 84% and recall score of 94%, the model did predict some false positives but is still remained highly effective in identifying high risk loans.</p>  
<p> Given the high accuracy and balanced performance, Logistic Regression is a strong choice for this task. </p>







