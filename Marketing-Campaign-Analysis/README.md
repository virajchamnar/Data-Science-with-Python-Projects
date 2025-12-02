# Marketing Campaign Analysis

## 📌 Project Overview
This project analyzes customer demographics, spending behavior, and campaign responses to evaluate marketing campaign effectiveness.  
The goal is to understand which customer segments respond better, what drives higher spending, and how future campaigns can be optimized for better targeting.

## 🎯 Objectives
- Evaluate the effectiveness of multiple marketing campaigns  
- Understand customer response behavior and spending patterns  
- Identify high-value customer segments  
- Generate insights to improve future marketing strategies  

## 📁 Dataset Information
The dataset contains information related to:

**People**: Birth year, education, marital status, income, customer onboarding date  
**Product**: Spending on wine, meat, fruits, sweets, gold  
**Place**: Purchases via store, web, and catalog channels  
**Promotion**: Campaign acceptances, previous complaints, last interaction

Files Provided:
- `marketing_data.csv`
- `Data Dictionary - Response to marketing campaigns.pdf`
- `marketing_campaign_problem_statement.pdf`

## 🧹 Data Cleaning & Preprocessing
Key steps performed:
- Cleaned and standardized column names  
- Removed symbols from Income and converted to numeric  
- Standardized inconsistent categories in Education & Marital Status  
- Converted Dt_Customer to datetime  
- Imputed missing Income using median grouped by (Education + Marital Status)  
- Removed unrealistic ages (>100 years)  
- Treated Income outliers using percentile capping  

## 🧠 Feature Engineering
Created new features to enhance analysis:
- **TotalChildren** = Kidhome + Teenhome  
- **Age** (based on birth year)  
- **TotalSpending** (sum of all product spending)  
- **TotalPurchases** (combined purchases from all channels)

## 📊 Exploratory Data Analysis
- Distribution of income, spending, and age  
- Correlation heatmap for numerical features  
- Customer segmentation based on children, education, and income  
- Visualization of product spending patterns  
- Campaign acceptance by country and age group  
- Comparison of spending across families  

## 🧪 Hypothesis Testing
1. **Older customers prefer in-store shopping** → *Not supported*  
2. **Customers with children prefer online shopping** → *Opposite — they spend less*  
3. **Online/catalog channels cannibalize store sales** → *No evidence*  
4. **US customers spend more than others** → *Difference not significant*  

## 📈 Key Insights
- Wine and meat generate the highest revenue  
- Spain shows the strongest campaign acceptance  
- Customers with no children spend significantly more  
- Age has minimal influence on campaign acceptance  
- Multi-channel shoppers are high-value customers  
- Graduation-level customers recorded most complaints  

## 💼 Business Recommendations
- Focus marketing initiatives on highly responsive regions like Spain  
- Create exclusive bundles for premium product buyers  
- Promote multi-channel shopping via loyalty incentives  
- Improve customer experience for Graduation-educated complainants  
- Prioritize child-free, higher-income segments for campaigns  

## 📂 Files Included
- `Marketing_Campaign.ipynb`  
- `Marketing_Campaign - Project.pdf`  
- `Data Dictionary - Response to marketing campaigns.pdf`  
- `marketing_campaign_problem_statement.pdf`  
- `marketing_data.csv`

## ✔ Conclusion
This project provides deep insights into customer behavior, product performance, and campaign effectiveness.  
The analysis supports data-driven marketing strategy development with actionable recommendations.
