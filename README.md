# bank_churn

**Project Description**

*Client*: Marketing department of "Metanprom" bank. The bank is experiencing an increased customer churn, which poses a threat to the bank's existence.

*Objective*: Identify homogeneous and highly accurate segments of churned customers, on which interventions should be focused to improve the bank's performance.

*Data Description*:
The dataset contains data about customers of "Metanprom" bank. The bank is located in Yaroslavl and the regional cities: Rostov Veliky and Rybinsk.

Columns:

- `userid` — user identifier,
- `score` — credit score,
- `City` — city,
- `Gender` — gender,
- `Age` — age,
- `equity` — equity score,
- `Balance` — account balance,
- `Products` — number of products used by the customer,
- `CreditCard` — whether the customer has a credit card,
- `last_activity` — active customer indicator,
- `estimated_salary` — customer's estimated salary,
- `Churn` — churn status (whether the customer has churned or not).

*Contents*:
1. Data Loading and Preprocessing
   - Check the correctness of column names and rename them if needed.
   - Data encoding.
   - Check data types and convert them if necessary.
   - Handle missing values.
   - Handle duplicates.
2. Exploratory Data Analysis. Explore correlations and customer profiles.
3. Identify features that influence churn. Draw conclusions.
4. Identify segments that are most prone to churn. Prioritize them.
5. Hypothesis Testing:
   1. Hypothesis on the difference in income between churned and retained customers.
   2. Hypothesis on the difference in churn rate based on the number of products used.
