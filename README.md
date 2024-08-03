### Exploratory Data Analysis for Car Loan
#### Problem Statement
Assume that You work for a financial institution that provides car loans to customers. The organization has collected a dataset containing information about various car loan applications they've received over the past year.

The customers are approaching to a finance company for a car loan. In order to better understand the factors influencing car loan approval/amount requested, perform exploratory data analysis on the dataset and prepare the data for Model building.

The dataset contains the following features: Cust id, Amount.Requested, Amount.Funded.By.Investors to company, Interest.Rate, Loan duration, Family income, credit score, employment length, owning a two wheeler, age band & debt to income ratio

#### Data Cleaning and Preparation
- Dropped unnecessary columns (e.g., Unnamed: 1).
- Cleaned and transformed features:
- Interest_Rate: Removed the % symbol and converted to numeric.
- Debt_To_Income_Ratio: Removed the % symbol and converted to numeric.
- Converted columns Cust_ID, Amount_Requested, Amount_Funded_By_Investors, Interest_Rate, Family_Income to numeric.
- Employment_Length: Removed text (e.g., year, years, <) and converted to numeric.
- Owning_A_Two_Wheeler: Cleaned values by replacing yess ! with yes and noo with no.
- Credit_Score: Replaced all string characters, split the range, calculated the average, and created a single numeric column.
- Age_Band: Replaced empty values with the mode, split the range, calculated the average, and created a single numeric column.
Created dummy variables for Owning_A_Two_Wheeler and Loan_Duration.

#### Exploratory Data Analysis (EDA)
Performed comprehensive EDA to uncover insights and patterns within the data. Visualizations included:
- Loan Duration Analysis: A pie chart showing the distribution of loan durations:
36 months: 78.63%
60 months: 21.37%
- Employment Length Impact: Longer employment lengths correlate with higher rates of two-wheeler ownership, peaking at 10.0 years.
- Loan Duration Preferences: Borrowers generally prefer 36-month loans (78.63%) over 60-month loans (21.37%), especially noticeable among those with longer employment histories.
- Income and Loan Amounts: Lower-income applicants primarily seek smaller loan amounts, although outliers request larger sums despite lower incomes.
- Age and Loan Approval: Applicants aged 35-40 receive the highest loan approvals, suggesting greater financial stability or creditworthiness in this demographic.
- Loan Amount Distribution: Requests are skewed towards smaller amounts, indicating most borrowers seek modest financial assistance.

#### Outcome
This analysis provided actionable insights into loan approval dynamics, emphasizing factors such as employment length, age, income, and loan preferences. These findings are crucial for refining loan products and improving customer engagement strategies.




  
