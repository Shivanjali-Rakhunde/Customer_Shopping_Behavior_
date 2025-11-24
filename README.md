📊 Customer Shopping Behavior Analysis
📝 Project Overview

This project analyzes customer shopping behavior using a dataset of 3,900 purchase records.
The goal is to uncover insights into customer demographics, spending patterns, product interest, and subscription behavior to support business decision-making.

The workflow includes Python for EDA, MySQL for structured analysis, and Power BI for visualization.

📁 Dataset Summary

Rows: 3,900

Columns: 18

Key Features Include:

Demographics: Age, Gender, Location, Subscription Status

Purchase info: Item Purchased, Category, Amount, Color, Size, Season

Behavior: Discount Applied, Promo Code Used, Review Rating, Purchase Frequency, Shipping Type

Missing Values: 37 missing entries in Review Rating (imputed)

🧹 Data Preparation & Cleaning (Python)

Key preprocessing steps:

✔ Data Loading & Exploration

Loaded dataset using pandas

Used .info() and .describe() for structure and summary

✔ Handling Missing Data

Replaced missing review ratings using median rating per product category

✔ Column Standardization

Converted column names to snake_case

✔ Feature Engineering

Added:

age_group (binned age ranges)

purchase_frequency_days (derived from purchase timestamps)

✔ Redundancy Fix

Confirmed promo_code_used was redundant with discount_applied → dropped the column

✔ Database Integration

Exported the cleaned dataset into MySQL for SQL-based analysis

🧮 SQL Analysis (MySQL)

MySQL queries were used to solve major business questions:

Revenue by Gender – Which gender contributes more?

High-Spending Discount Users – Customers who still spend above average with discounts.

Top 5 Products by Rating

Shipping Type Spend Comparison – Standard vs Express.

Subscribers vs Non-Subscribers – Spend differences & total revenue.

Discount-Dependent Products – Products frequently purchased on discount.

Customer Segmentation – New, Returning, Loyal.

Top 3 Products per Category

Repeat Buyers & Subscription Likelihood

Revenue by Age Group

📊 Power BI Dashboard

A dynamic Power BI dashboard visualizes:

Revenue trends

Customer behavior

Top-selling products

Subscription insights

Shipping type performance

Demographic breakdowns

💡 Business Recommendations
🔹 Boost Subscriptions

Promote unique benefits to convert more customers.

🔹 Strengthen Loyalty Programs

Encourage frequent buyers to move into the Loyal segment.

🔹 Optimize Discount Strategy

Balance discount incentives with profitability.

🔹 Feature High-Rated Products

Use top-rated/top-purchased items in marketing.

🔹 Target High-Value Demographics

Focus on age groups and shipping preferences that generate higher revenue.

🛠 Tech Stack
Tool	Purpose
Python (pandas, numpy)	EDA, preprocessing
MySQL	SQL analysis
Power BI	Dashboard visualizations
Jupyter Notebook	Development environment
