# Dataset Description

### 📁 Dataset: Customer Satisfaction Data
This synthetic dataset simulates customer interactions and outcomes across various retail stores. It includes transaction details, product categories, employee experience, and customer satisfaction scores.

The dataset is ideal for demonstrating supervised learning techniques, particularly for a regression task with the target variable: `Satisfaction`.

There are 1,000 records, and the dataset includes the following columns:

| Column Name    | Description                                                                |
| -------------- | -------------------------------------------------------------------------- |
| `ID`           | Unique identifier for each record.                                         |
| `Date`         | Date of the transaction or customer interaction (YYYY-MM-DD format).       |
| `Store`        | Store location or identifier (e.g., A, B, C...).                           |
| `ProdCat`      | Product category involved in the transaction (e.g., Clothing, Toys, Home). |
| `Certified`    | Whether the product or service was certified (`Yes` or `No`).              |
| `Sales`        | Total sales value in currency units for the transaction.                   |
| `TimeSpent`    | Time (in hours) the customer spent during the visit.                       |
| `Transactions` | Number of individual transactions or items purchased.                      |
| `YrsExp`       | Years of experience of the employee assisting the customer.                |
| `Returned`     | Whether the product was returned (`True` or `False`).                      |
| `Satisfaction` | Customer satisfaction score (scale from 1.0 to 10.0).                      |


### 📁 Dataset: Customer Churn Data 
This churn dataset captures customer profiles and banking activity, commonly used for modeling customer churn, predicting whether a customer will leave or stay with the bank.

It supports supervised classification tasks, with the target variable: Exited, where:

1 = the customer churned (left the bank)

0 = the customer stayed

 Available Versions
Large Churn Dataset ([churn_data_large.csv](./churn_data_large.csv)): 165,034 records: 

Small Churn Dataset ([churn_data_small.csv](./churn_data_small.csv)): 10,000 records, randomly sampled from the large churn dataset

Each record represents an individual customer, with associated demographic and behavioral features.

| Column Name       | Description                                                               |
| ----------------- | ------------------------------------------------------------------------- |
| `id`              | Record index (may be redundant with `CustomerId`).                        |
| `CustomerId`      | Unique identifier for each customer.                                      |
| `Surname`         | Customer’s last name (included for realism; not needed for modeling).     |
| `CreditScore`     | Customer’s credit score (higher = better creditworthiness).               |
| `Geography`       | Country where the customer resides (e.g., France, Spain, Germany).        |
| `Gender`          | Gender of the customer (`Male`, `Female`).                                |
| `Age`             | Customer's age (in years).                                                |
| `Tenure`          | Number of years the customer has been with the bank.                      |
| `Balance`         | Customer’s bank account balance.                                          |
| `NumOfProducts`   | Number of products the customer uses (e.g., savings, credit card).        |
| `HasCrCard`       | Whether the customer has a credit card (`1` = Yes, `0` = No).             |
| `IsActiveMember`  | Whether the customer is considered active (`1` = Active, `0` = Inactive). |
| `EstimatedSalary` | Estimated yearly salary of the customer.                                  |
| `Exited`          | Target variable: whether the customer churned (`1`) or remained (`0`).    |


📁 Dataset: Insurance Charges Data ([churn_data_small.csv](./churn_data_small.csv))

This dataset contains information on individuals’ demographics and health-related attributes, commonly used to estimate medical insurance charges. It includes personal details such as age, sex, body mass index (BMI), number of children, smoking status, residential region, and the insurance charges incurred.

This dataset is well-suited for regression-based supervised learning tasks, with the target variable: charges.

There are 1338 records in total, and the dataset includes the following columns:

Column Name	Description
age	Age of the individual (in years).
sex	Gender of the individual (male or female).
bmi	Body Mass Index (BMI), a measure of body fat based on height and weight.
children	Number of children/dependents covered by the insurance.
smoker	Smoking status (yes or no).
region	Residential region in the US (northeast, northwest, southeast, southwest).
charges	Individual medical insurance charges billed by the insurer (in USD).