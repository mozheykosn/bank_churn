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


*Conclusion:*

Overall churn rate across all data: 18.33%.

After analyzing all the indicators, we have identified several churn-related features:
- Scores ranging from 830 to 950.
- Age groups of 50-60 and 25-30.
- Male customers are more likely to churn.
- Balances between 100,000 and 120,000, and 140,000-180,000.
- Higher churn rate in Yaroslavl.
- Customers without a credit card.
- Customers with 3, 4, or 5 products.
- Equity scores ranging from 3 to 9, especially 6, 7, and 9.
- Salaries between 100,000 and 220,000.

More loyal bank customers exhibit the following characteristics:
- Scores between 690 and 820.
- Age groups of 36-45 and 60+.
- Balances between 140,000 and 180,000.
- Salaries between 0 and 90,000.
- Reside in Rybinsk.
- Female customers.
- Have a credit card.
- Have 1 product with the bank.
- Have equity scores between 0 and 2.
- 
Based on the correlation matrix, there is no strong dependency between the indicators. The highest correlations with churn are observed for the number of products (30%) and equity scores (27%). However, this is not sufficient to assert a definite relationship. Male customers are more prone to churn than female customers. Additionally, Yaroslavl exhibits a higher tendency for churn compared to other cities, but the dependency is weak.

Segments

After a comprehensive data analysis, several highly churn-prone segments (with churn rates exceeding 43% within the segment) can be identified:
- Males with 3 to 5 products (376 individuals).
- All customers with scores ranging from 700 to 950 and with 3 to 5 products (579 individuals).
- Customers with salaries between 90,000 and 230,000 and with 3 to 5 products (369 individuals).
- Customers with equity scores between 3 and 9 and with 3 to 5 products (522 individuals).

These are narrow segments but exhibit a high churn rate. Additionally, there are broader segments with churn rates higher than the average:
- Males from Yaroslavl (710 individuals).
- All customers with balances between 100,000 and 120,000, and 140,000-180,000 (405 individuals).
