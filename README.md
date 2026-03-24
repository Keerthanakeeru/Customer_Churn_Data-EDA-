## Customer Churn – Exploratory Data Analysis
### Project Overview
This project performs Exploratory Data Analysis (EDA) on a telecom customer churn dataset to understand which customer segments are more likely to leave the service. The analysis focuses on demographic features, subscription details, contract types, and billing patterns to explore their relationship with churn behavior.
​

The dataset contains 7,043 customers and 21 variables, including tenure, contract, internet services, monthly charges, and a binary churn label. Using Python (Pandas, NumPy, Matplotlib, Seaborn), the notebook cleans the data, summarizes key statistics, and visualizes important patterns related to churn.
​

### Objectives
Load and inspect the telecom customer churn dataset from CSV using Pandas.
​

Understand the structure of the data (rows, columns, data types, missing values).

Explore distributions of key numerical variables such as tenure, MonthlyCharges, and TotalCharges.
​

Analyze churn rates across demographics (gender, SeniorCitizen, Partner, Dependents).
​

Examine how contract type, payment method, and internet services are associated with churn.
​

Build a clear EDA foundation to guide further modeling (classification) in a separate notebook.

### Dataset Information
File used: Customer Churn.csv.
​

Rows: 7,043 customers.

Columns: 21 features, including target variable Churn.
​

### Key Columns
customerID: Unique identifier for each customer.

Demographics: gender, SeniorCitizen, Partner, Dependents.
​

Account Information: tenure, Contract (Month-to-month, One year, Two year), PaperlessBilling, PaymentMethod (Electronic check, Mailed check, Bank transfer, Credit card).
​

Services: PhoneService, MultipleLines, InternetService (DSL, Fiber optic, None), OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies.
​

Billing: MonthlyCharges, TotalCharges.
​

Target: Churn (Yes/No).
​

### Tools and Libraries
Programming Language: Python.

#### Libraries:

pandas for data loading and manipulation.
​

numpy for numerical operations.
​

matplotlib.pyplot and seaborn for visualization of distributions and relationships.
​

### EDA Steps and Key Concepts
#### Data loading and initial view:

Read the CSV into a DataFrame (pd.read_csv('Customer Churn.csv')).
​

Display the first few rows to inspect columns and example values.
​

#### Data structure and summary:

Use descriptive statistics to summarize numeric columns like SeniorCitizen, tenure, MonthlyCharges, and TotalCharges (count, mean, std, min, max, quartiles).
​

Check for potential data quality issues (e.g., numeric columns stored as object, zeros in TotalCharges).
​

#### Univariate analysis:

Distribution of tenure and charges to understand customer lifecycle and billing levels.

Frequency counts for categorical variables such as contract type, payment methods, and services.

#### Bivariate analysis (EDA for churn):

Compare churn vs non‑churn customers by tenure and billing to see which ranges are more at risk.

Analyze churn rates across contract types, internet service types, and add‑on services (security, backup, tech support, streaming).

Study churn patterns by demographics (SeniorCitizen, Partner, Dependents, gender).

#### Visualization:

Histograms and boxplots for numerical features.

Countplots / bar charts for categorical variables split by churn status.

(You can adjust this section to exactly match the plots you have in the notebook.)

### Learning Outcomes
Hands‑on practice with a full EDA workflow on a supervised learning problem (churn).

Improved understanding of how telecom business features (contracts, services, billing) relate to churn.
​

Experience with Pandas + Seaborn/Matplotlib for summarizing and visualizing real‑world tabular data.
​

A solid base notebook that can be extended into a machine learning model (logistic regression, tree‑based models, etc.) in a follow‑up project.
