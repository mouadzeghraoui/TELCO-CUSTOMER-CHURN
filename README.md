### Problem statement

Churn is most commonly expressed as the percentage (or number) of  service subscribers who discontinue their subscriptions within a given  time period.

-----

### Table of content
- Data Description Report
- Data Cleaning
- Exploratory Data Analysis
- Feature Engineering
- Data Preprocessing
- Model Training
- HyperParameter Tuning
- Model Testing

-----

### DataSet

You can download the dataset from kaggle : [Telco_Customer_Churn](https://www.kaggle.com/blastchar/telco-customer-churn)

-----

### Data Dictionary 

- customerID: customer ID
- gender: whether the customer is a male or a female
- SeniorCitizen: whether the customer is a senior citizen or not (1, 0)
- Partner: whether the customer has a partner or not (Yes, No)
- Dependents: whether the customer has dependents or not (Yes, No)
- tenure: number of months the customer has stayed with the company
- PhoneService: whether the customer has a phone service or not (Yes, No)
- MultipleLines: whether the customer has multiple lines or not (Yes, No, No phone service)
- InternetService: customer’s internet service provider (DSL, Fiber optic, No)
- OnlineSecurity: whether the customer has online security or not (Yes, No, No internet service)
- OnlineBackup: whether the customer has online backup or not (Yes, No, No internet service)
- DeviceProtection: whether the customer has device protection or not (Yes, No, No internet service)
- TechSupport: whether the customer has tech support or not (Yes, No, No internet service)
- StreamingTV: whether the customer has streaming TV or not (Yes, No, No internet service)
- StreamingMovies: whether the customer has streaming movies or not (Yes, No, No internet service)
- Contract: the contract term of the customer (Month-to-month, One year, Two year)
- PaperlessBilling: whether the customer has paperless billing or not (Yes, No)
- PaymentMethod: the customer’s payment method (Electronic check,  Mailed check, Bank transfer (automatic), Credit card (automatic))
- MonthlyCharges: the amount charged to the customer monthly
- TotalCharges: the total amount charged to the customer
- Churn: whether the customer churned or not (Yes or No)

-----

### Data Description Report

We have 13 Categorical variables, 6 Boolean, and 2 Numerical

-----

### Data Preparation

- We have 0 missing values
- We have some features with high cardinality 
- We have some features that we have to convert to numerical.

----

### Exploratory Data Analysis

- 27% of the customers in our dataset have churned.

- The split between male and female is almost excatly 50/50. This feature  does not seem to have significance when it comes to predicting the  churn.
- The number of senior citizen is 1,042, which represent 26% of the total customers. However, senior citizen seem more likely to churn as 42% have cancelled their subscription compare with  24% for the non senior citizen.

NEEEEED TO ADD MORE

-----

### Model Train

We used a Random Forrest to predict wether a customer is going churn or not. We achived 80% accuracy with this model.

We have only about 26.5% of the churn cases, so, if you always guess that a customer is not churning, you will be right  about 74% of the time. It's because the Dataset is unbalanced

Since the dataset is unbalanced, we need to check the precision, recall, and F1-Score metrics.

we have a bad F1-Score, so we try to do some hyperParameter tuning to increase the performance of our model.









We then created a graph to plot the level of importance of each of the features in predicting the customer churn.

The top four features in predicting the customers churn are

-----

### Model Testing

