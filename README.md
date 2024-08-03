## Exploratory Data Analysis for Car Loan
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



## A Comprehensive Statistical Analysis of Used Car Data
#### The objective of this statistical analysis is to demonstrate the importance of using:
- Descriptive statistics, Probability and Inferential statistics.
- Explore the dataset and answer various research questions to draw meaningful conclusions from data and make informed decisions using Python.
  
#### Data Preprocessing
- Cleaned and transformed features:
- Mileage: Removed 'kmpl' and 'km/kg' and converted to numeric
- Engine: Removed 'CC' and converted to numeric
- Max_power: Removed 'bhp' and converted to numeric
- Converted Sales_ID and Postal_code to object datatype

#### Research Questions and Insights
- Characteristics of Cars:
      - Average Mileage: 19.42 kmpl
      - Average Selling Price: ₹649,813.72
      - Price Range: ₹9,970,001
      - Interquartile Range of Prices: ₹420,000
      - Most Common Fuel Type: Diesel
      - Most Common Transmission Type: Manual

- Significant Differences:
      - Selling Price by Seller Type:
      - Dealer: ₹1,459,910
      - Individual: ₹507,706
      - Trustmark Dealer: ₹801,839

- Transmission Type Preference:
      - Manual: 86.83%
      - Automatic: 13.17%
Manual transmissions are more common, suggesting higher availability for buyers preferring manual cars.

- Price Variation with Mileage, Engine Size, and Year:
 Mileage: Weak negative correlation (-0.126), indicating higher mileage slightly decreases selling price.

Engine Size: Moderate positive correlation (0.456), indicating larger engines generally have higher prices.

Year of Manufacture: Moderate positive correlation (0.412), indicating newer cars generally have higher prices.

- Covariance between Selling Price and Mileage:
Negative covariance (-414,682.41) suggests an inverse relationship; higher mileage tends to decrease selling price.

- Probability of Automatic Transmission for Cars over ₹10,000:13.17%

#### Hypothesis Testing:
- Significant difference in selling prices based on fuel type (Petrol vs. Diesel): T-statistic: -18.12, P-value: 5.96e-72
- Significant difference in the number of seats between cars with automatic and manual transmissions: P-value close to 0
- Strong association between car models and owner types: Chi-square statistic and corresponding p-value indicate a significant relationship.

#### Outcome
This statistical analysis provided deep insights into the used car market, highlighting factors influencing car prices, buyer preferences, and the impact of various car attributes on selling prices. The findings are crucial for developing pricing strategies and improving inventory management for pre-owned vehicles.

  
