# credit-risk-classification
## Purpose of the analysis:
The objective of this analysis is to train and evaluate a machine learning model to classify loans as either 'healthy' or 'high-risk' based on borrowers' financial data.

## Files and Folders:
* credit_risk_classification.ipynb: Jupyter Notebook containing the complete machine learning model analysis, including data preprocessing, training, evaluation, and results.
* lending_data.csv: The original dataset with borrower financial details used for training and testing the model.
* installed_packages.txt: A list of all installed Python packages in the environment to ensure reproducibility and consistent execution across different setups.


## About the Dataset:
The dataset contained the following financial information of the borrowers:
* Loan size
* Interest rate
* Borrower income
* Debt to income ratio
* Number of accounts
* Derogatory marks
* Total debt. 
<p>The target variable (y) represents the loan status, indicating whether a loan is classified as 'healthy' or 'high-risk.' </p>

## Machine Learning Model Used:
Logistic Regression, a classification algorithm, was used for this analysis. It estimates the outcome based on the input features. 

## Stages of Machine Learning Process:
* **Data Preparation:** The Data was loaded into a Pandas DataFrame. The features (X) and target variable (y) were separated. Then, the data was split into training and testing sets using train_test_split().
* **Model selection and training:** Logistic Regression was chosen as the lassification algorithm. The model was initialized with random_state= 1, max_iter=200 and trained using fit() on the training data. Predictions were made on the test dataset using predict().

* **Evaluation:** The model was evaluated using a confusion matrix and a classification report. Key performance metrics like precision, recall and accuracy were analyzed

## Result Summary:
* Accuracy score: 0.99
* Precision score:
    - Healthy loan: 1.00
    - High Risk: 0.84
* Recall score:    
    - Healthy loan: 0.99
    - High Risk: 0.94

    ![Alt text](Credit_Risk/score.png)
<p> With an accuracy score of 99%, the Logistic Regression model performed exceptionally well. 
<p> For healthy loans, with a perfect precision score of 100% and almost perfect recall score of 99%, the model almost never misclassified healthy loans.</p>
<p> For high risk loans, with a precision score of 84% and recall score of 94%, the model did predict some false positives but is still remained highly effective in identifying high risk loans.</p>  

<P>I would highly recommend this model for use by company due to its high accuracy and strong performance. The 100% precision score for healthy loans ensures that all approved loans are truly low-risk supporting business growth. Additionally, the high recall score for high-risk loans (94%) ensures that the majority of risky loans are correctly identified reducing potential losses. This makes the model a reliable tool for approving loans wisely while reducing risk.

## Set Up:

To download the required libraries, run the following in your console:

* pip install -r installed_packages.txt









