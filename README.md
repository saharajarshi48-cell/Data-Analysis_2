Telecom Customer Churn Analysis — Project Summary & Key Insights
This project performs an end-to-end exploratory data analysis (EDA) on a Telecom Customer Churn dataset to understand the factors influencing customer churn. The analysis includes data cleaning, feature transformation, univariate and bivariate analysis, and visual exploration of churn patterns across customer demographics, service usage, and payment behaviors.

Project Summary
The dataset contains customer demographic details, subscription information, service usage, and churn labels. The notebook walks through the following key steps:
1. Data Import & Inspection
Loaded the dataset using Pandas.
Inspected structure using df.info(), df.describe(), and null-value checks.
Verified presence of duplicate customerID entries.

2. Data Cleaning & Preprocessing
Fixed incorrect formatting in the TotalCharges column by converting blank values to zero and casting to float.
Converted the SeniorCitizen binary column (0/1) to categorical labels ("Yes"/"No") for better readability.
Checked for missing values and cleaned data accordingly.

3. Univariate Analysis
Visualized distributions of key categorical and numerical variables, including:

Churn Distribution
Gender
Contract Type
Payment Method
Tenure
Countplots, bar labels, and histograms were used to understand customer composition and churn proportions.

4. Bivariate Analysis (Churn vs. Features)
Examined how churn varies across:
Gender
Partner / Dependents
Internet & Phone Services
OnlineSecurity / TechSupport / OnlineBackup / DeviceProtection
Streaming services (TV & Movies)
Contract Types

Payment Methods
Used grouped bar charts, hue-based countplots, and percentage breakdowns.
Key Insights From the Analysis
1. Churn Rate
A notable fraction of customers have churned, indicating potential dissatisfaction or competitive pressure.

2. Contract Type Is a Major Predictor
Month-to-month contract customers churn the most.
Two-year contract customers churn the least, suggesting long-term contracts reduce customer turnover.

3. Tenure Strongly Influences Churn
Newer customers (low tenure) churn significantly more.
Customers retained for over a year show much lower churn rates.

4. Service Protection Reduces Churn
Customers without the following services show higher churn:
Online Security
Tech Support
Device Protection
Online Backup
These optional services appear to increase customer stickiness.

5. Internet Service Type Also Matters
Customers using Fiber Optic internet churn more than DSL users.
Possibly linked to higher prices or service issues.

6. Payment Method & Billing
Electronic check users have the highest churn, suggesting dissatisfaction or billing friction.
Automatic payments (bank transfer / credit card) correlate with lower churn.

7. Demographics Have Weak Impact
Gender does not significantly affect churn.
Having a partner or dependents slightly reduces churn, but the effect is small.

Overall Conclusion
Churn is most strongly influenced by contract type, service protection add-ons, tenure, payment method, and internet service type. Customer retention strategies should focus on:
Incentivizing long-term contracts
Improving onboarding for new customers
Offering bundled security/tech support services
Streamlining billing for electronic check users
Addressing potential issues with Fiber Optic service users
