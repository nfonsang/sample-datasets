# Documentation of Datasets

## 📁 Dataset: Customer Satisfaction Data
This synthetic customer satisfaction dataset ([customer_satisfaction_data.csv](./customer_satisfaction_data.csv)) represents customer interactions and outcomes across various retail stores. It includes transaction details, product categories, employee experience, and customer satisfaction scores.

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


## 📁 Dataset: Customer Churn Data 
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


## 📁 Dataset: Insurance Charges Data 

This dataset ([insurance_data.csv](./insurance_data.csv)) contains information on individuals’ demographics and health-related attributes, commonly used to estimate medical insurance charges. It includes personal details such as age, sex, body mass index (BMI), number of children, smoking status, residential region, and the insurance charges incurred.

This dataset is well-suited for regression-based supervised learning tasks, with the target variable: charges.

There are 1338 records in total, and the dataset includes the following columns:

| Column Name | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `age`       | Age of the individual (in years).                                           |
| `sex`       | Gender of the individual (`male` or `female`).                              |
| `bmi`       | Body Mass Index (BMI), a measure of body fat based on height and weight.   |
| `children`  | Number of children/dependents covered by the insurance.                     |
| `smoker`    | Smoking status (`yes` or `no`).                                             |
| `region`    | Residential region in the US (`northeast`, `northwest`, `southeast`, `southwest`). |
| `charges`   | Individual medical insurance charges billed by the insurer (in USD).        |


## 📁 Dataset: Loan Application Data ([loan_data.csv](./loan_data.csv))
This dataset provides a snapshot of loan applicants, including their financial status, credit history, and loan details. It’s particularly useful for binary classification tasks such as credit risk modeling — predicting whether a loan will be classified as good or bad.

There are 9857 records in total, and the dataset includes the following columns:

| Column Name                  | Description                                                                 |
|-----------------------------|-----------------------------------------------------------------------------|
| `funded_amnt`               | Amount of money funded to the borrower (in USD).                           |
| `term`                      | Loan term length (`term_36` or `term_60` months).                           |
| `int_rate`                  | Interest rate on the loan (in %).                                           |
| `sub_grade`                 | Loan subgrade, reflecting credit risk (e.g., A1, C4, D1).                   |
| `addr_state`                | US state where the borrower resides.                                       |
| `verification_status`       | Whether the borrower's income was verified |
| `annual_inc`                | Annual income of the borrower (in USD).                                    |
| `emp_length`                | Length of employment (e.g., `emp_5`, `emp_ge_10`, `emp_lt_1`, `emp_unk`).   |
| `delinq_2yrs`               | Number of delinquencies in the past 2 years.                               |
| `inq_last_6mths`            | Number of credit inquiries in the past 6 months.                           |
| `revol_util`                | Revolving line utilization rate (percentage of credit used).               |
| `acc_now_delinq`            | Number of accounts currently delinquent.                                   |
| `open_il_6m`                | Number of installment accounts opened in the last 6 months.                |
| `open_il_12m`               | Number of installment accounts opened in the last 12 months.               |
| `open_il_24m`               | Number of installment accounts opened in the last 24 months.               |
| `total_bal_il`             | Total current balance on all installment accounts.                         |
| `all_util`                  | Ratio of total balances to total credit limits across all credit lines.    |
| `inq_fi`                    | Number of finance-related inquiries.                                       |
| `inq_last_12m`              | Number of credit inquiries in the past 12 months.                          |
| `delinq_amnt`               | Total amount delinquent (in USD).                                          |
| `num_il_tl`                 | Number of installment accounts.                                            |
| `total_il_high_credit_limit`| Total high credit/credit limit for all installment accounts.               |
| `Class`                     | Loan status label (`good` or `bad`).                                       |


## 📁 Dataset: Wage and Employment Data
This dataset ([wage_data.csv](./wage_data.csv))contains individual-level employment information, including wages, educational background, work experience, and demographic variables. It is well-suited for regression tasks (e.g., predicting wage) and for analyzing the relationships between education, experience, and earnings.

There are 28,155 records in total, and the dataset includes the following columns:

| Column Name | Description                                                                 |
|-------------|-----------------------------------------------------------------------------|
| `wage`      | Weekly wage of the individual (in USD).                                     |
| `education` | Years of formal education completed.                                        |
| `experience`| Number of years of work experience.                                         |
| `ethnicity` | Ethnic group of the individual (e.g., `cauc`, `afam`, `hisp`, `other`).     |
| `smsa`      | Whether the individual lives in a Standard Metropolitan Statistical Area (`yes` or `no`). |
| `region`    | Region of residence in the U.S. (e.g., `northeast`, `south`, etc.).         |
| `parttime`  | Whether the job is part-time (`yes` or `no`).                               |
