# Predict-Customer-Churn

## Introduction 

Customer churn occurs when customers or subscribers stop doing business with a company or service, also known as customer attrition. It is also referred to as loss of clients or customers. One industry in which churn rates are particularly useful is the telecommunications industry because most customers have multiple options from which to choose within a geographic location.

Logistic Regression, Decision Tree, and Random Forest will be introduced in R and will be used for the predictive workflow. 

## Data

The data was downloaded from IBM Sample Data Sets. Each row represents a customer, each column contains that customer’s attributes:

* customerID
* gender (female, male)
* SeniorCitizen (Whether the customer is a senior citizen or not (1, 0))
* Partner (Whether the customer has a partner or not (Yes, No))
* Dependents (Whether the customer has dependents or not (Yes, No))
* tenure (Number of months the customer has stayed with the company)
* PhoneService (Whether the customer has a phone service or not (Yes, No))
* MultipleLines (Whether the customer has multiple lines r not (Yes, No, No phone service)
* InternetService (Customer’s internet service provider (DSL, Fiber optic, No)
* OnlineSecurity (Whether the customer has online security or not (Yes, No, No internet service)
* OnlineBackup (Whether the customer has online backup or not (Yes, No, No internet service)
* DeviceProtection (Whether the customer has device protection or not (Yes, No, No internet service)
* TechSupport (Whether the customer has tech support or not (Yes, No, No internet service)
* streamingTV (Whether the customer has streaming TV or not (Yes, No, No internet service)
* streamingMovies (Whether the customer has streaming movies or not (Yes, No, No internet service)
* Contract (The contract term of the customer (Month-to-month, One year, Two years)
* PaperlessBilling (Whether the customer has paperless billing or not (Yes, No))
* PaymentMethod (The customer’s payment method (Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)))
* MonthlyCharges (The amount charged to the customer monthly — numeric)
* TotalCharges (The total amount charged to the customer — numeric)
* Churn ( Whether the customer churned or not (Yes or No))

The raw data contains 7043 rows (customers) and 21 columns (features). The “Churn” column is our target.

## Project's Summary
### For a more thorough detailed workflow process check the "detailed_workflow" document

The results displays that Logistic Regression, Decision Tree and Random Forest can be used for customer churn analysis for this particular dataset equally fine.

Throughout the analysis, several important things were observed:

* Features such as tenure_group, Contract, PaperlessBilling, MonthlyCharges, and InternetService appear to play a role in customer churn.

* There does not seem to be a relationship between gender and churn.

* Customers in a month-to-month contract, with PaperlessBilling and are within 12 months tenure, are more likely to churn; On the other hand, customers with one or two-year contracts, with longer than 12 months tenure, are not using PaperlessBilling, are less likely to churn.
