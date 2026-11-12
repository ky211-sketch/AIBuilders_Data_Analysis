## Tecno Customer Churn Prediction
### Supervised Learning- Classification 

## Project Overview :
This project is a Machine Learning application developed to predict customer churn for a telecom company, to predict whether a customer is likely to leave the company using supervised learning model- Classification.

## About the Dataset :

The project uses the Telco Customer Churn dataset containing approximately 7,000 customer records, dowloaded from kaggle : 
     https://www.kaggle.com/datasets/blastchar/telco-customer-churn


Columns (Features):
- CustomerID: A unique ID that identifies each customer.
- Gender: Male, Female
- Senior Citizen:  the customer is 65 or older: Yes, No
- Dependents:  if the customer lives with any dependents: Yes, No. Dependents could be children, parents, grandparents, etc.

- Tenure (in Months):  the total amount of months that the customer has been with the company by the end of the quarter specified above.
- Multiple Lines:  the customer subscribes to multiple telephone lines with the company: Yes, No

- Internet Service: the customer subscribes to Internet service with the company: No, DSL, Fiber Optic, Cable.
- Contract: current contract type: Month-to-Month, One Year, Two Year.
- Payment Method: payment method: Bank Withdrawal, Credit Card, Mailed Check
- Paperless Billing: the customer has chosen paperless billing: Yes, No

- Monthly Charge: current total monthly charge for all their services from the company.
- Total Charges: total charges, calculated to the end of the quarter specified above.

- Churn:  the status of the customer at the end of the quarter: Churned, Stayed.Churn Label: Yes = the customer left the company this quarter. No = the customer remained with the company. 

- Target Variable:
Churn

No → Customer stayed
Yes → Customer churned


## Data Preprocessing:
- Convert `TotalCharges` into a numerical data type, then Handle missing values appeared.
- Remove `customerID` because it is only an "identifier".
- Convert the target variable into binary.
- Select numerical and categorical features.


## Machine Learning Models:
Logistic Regression
Random Forest

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

first, we trained 2 models "Logistic Regression" and "Random Forest", then we compare.
they have very close result, but according to precision, accuracy and prediction proba we choose to improve randomforest model, using `GridSearchCV`, that increase "Recall" percentage, maintaing a close accuracy and precision.






 