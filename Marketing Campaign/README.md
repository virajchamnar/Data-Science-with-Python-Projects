Marketing Campaign Analysis
Project Overview

This project focuses on analyzing customer behavior across marketing campaigns using Exploratory Data Analysis (EDA), data cleaning, feature engineering, visual analytics, and hypothesis testing.
The dataset provides demographic, spending, and campaign interaction details and ties directly to the 4 Ps of Marketing — People, Product, Place, Promotion.

The goal is to extract insights that help improve customer acquisition, campaign targeting, and marketing strategy effectiveness.

Problem Statement

A retail company wants to understand how different customer segments respond to marketing campaigns. The task is to analyze spending patterns, channel usage, campaign success, and demographic behavior to derive business insights.

You must:

Clean and preprocess the dataset

Engineer key features

Perform EDA and create insightful visualizations

Conduct hypothesis testing as required

Summarize business implications

Objectives

Understand the factors influencing customer acquisition

Identify revenue-driving product categories

Compare campaign acceptance across demographics and countries

Analyze shopping behavior across channels

Test hypotheses that relate age, children, channels, and geography to spending

Dataset Description

The dataset includes:

People: Birth year, education, marital status, income

Product: Spending on wine, meat, fruits, sweets, gold

Place: Purchases across store, web, catalog

Promotion: Campaign acceptances, complaint history

Datasets used:

marketing_data.csv

Data Preparation & Cleaning
1. Initial Inspection

Loaded dataset and checked data types

Inspected summary stats & missing values

Identified formatting issues in Income, Education, and Marital Status

2. Key Cleaning Steps

Cleaned column names

Fixed Income format (removed $, commas, etc.)

Standardized marital status categories (Married, Single, Previously_Married)

Standardized education levels into defined groups

Converted Dt_Customer to datetime

Imputed missing Income using median of (Education + Marital Status) groups

Removed unrealistic age values (Age > 100)

Feature Engineering

Newly created variables:

TotalChildren = Kidhome + Teenhome

Age = Current year – Year_Birth

TotalSpending = Sum of all product spending

TotalPurchases = Web + Store + Catalog purchases

Exploratory Data Analysis
Univariate & Bivariate Analysis

Distribution plots (histograms, boxplots)

Outlier treatment (capping Income at 1st & 99th percentiles)

Correlation heatmap for numerical features

Visual Insights

Revenue breakdown across product categories

Campaign acceptance across countries

Spending patterns by number of children

Complaints segmented by education level

Hypothesis Testing
Hypothesis A: Older customers prefer in-store shopping

Pearson correlation between Age & Store Purchases

Result: Very weak relationship — hypothesis not supported

Hypothesis B: Customers with more children prefer online shopping

Spearman correlation between TotalChildren & Web Purchases

Result: Opposite trend — customers with more children shop less overall

Hypothesis C: Online/Catalog sales cannibalize store sales

Pearson correlations among all purchase channels

Result: No cannibalization — channels grow together

Hypothesis D: US customers outperform others in spending

Mann–Whitney U test

Result: No significant difference

Key Findings
Product Insights

Wine and Meat generate the highest revenue

Fruits and Gold contribute the least

High spenders consistently purchase premium categories

Customer Demographics

High-value customers are typically:

Older adults

Higher income

No children

Campaign Performance

Spain has the highest acceptance rate

Age does not meaningfully influence campaign acceptance

Multi-channel shoppers show the highest spending

Customer Complaints

Most complaints come from customers with a Graduation education level

Business Recommendations

Focus marketing campaigns on Spain — most responsive region

Promote premium product bundles to high-income, no-children customers

Encourage multi-channel shopping through cross-channel incentives

Improve support and communication for Graduation-level customers

Target low-response categories (fruits, gold) with product-specific promotions

Files Included

Marketing_Campaign.ipynb — Full analysis notebook

marketing_campaign_problem_statement.pdf — Project instructions

Marketing_Campaign - Project.pdf — Final report summary

Conclusion

This project successfully demonstrates the end-to-end data science process:

Data cleaning

Feature engineering

EDA

Hypothesis testing

Business interpretation

The insights provide clear, data-backed direction for improving campaign performance, enhancing customer segmentation, and optimizing marketing strategies.