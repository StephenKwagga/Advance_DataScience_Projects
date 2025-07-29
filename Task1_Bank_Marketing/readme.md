# Bank Marketing Campaign Analysis 

# Objective 
This project analyzes a bank marketing dataset to predict whether customers will subscribe to a term deposit based on demographic and campaign-related features.  

# Dataset 
Source: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)  
Features:  
- Demographics: age, job, marital, education, default, balance, housing, loan  
- Campaign Details: contact, day, month, duration, campaign, pdays, previous, poutcome  
- Target Variable: deposit (binary: "yes" or "no")  

# Approach 

# 1. Data Loading & Preprocessing 
- Loaded the dataset using pandas.read_csv().  
- Checked structure with .info(), .head(), and .isnull().sum() (no missing values found).  
- Encoded categorical variables (deposit → binary: 1="yes", 0="no") using .map().  
- Applied one-hot encoding (pd.get_dummies()) for categorical features.  

# 2. Exploratory Data Analysis (EDA)
- *Summary Statistics*: Analyzed distributions of numerical features (age, balance, duration).  
- *Correlation Analysis*: Checked relationships between features and the target variable.  
  Visualizations:  
  - Histograms for numerical feature distributions.  
  - Box plots for outlier detection.  
  - Pairwise scatter plots to identify trends.  

# 3. Model Training & Evaluation  
Models Used:  
  - Logistic Regression (Baseline classification)  
  - Random Forest (Ensemble method for better accuracy)  
  Evaluation Metrics:  
  - Accuracy  
  - F1-Score (handles class imbalance)  
  - ROC-AUC (measures model discrimination ability)  

# 4. Explainability with LIME  
- Used LIME (Local Interpretable Model-agnostic Explanations) to interpret model predictions.  
- Analyzed feature importance for 5 sample predictions per model.  

# Key Insights  
  Demographic Influence:  
  - Older customers and those with higher balances are more likely to subscribe.  
  - Customers with housing loans are less likely to opt for term deposits.  
  Campaign Impact:  
  - Longer call durations (duration) correlate with higher subscription rates.  
  - Previous campaign success (poutcome) strongly influences new subscriptions.
