# 🪔 Diwali Sales Analysis — Exploratory Data Analysis (EDA) with Python

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4c72b0?style=for-the-badge)

## 📌 Executive Summary
During high-traffic festive seasons such as Diwali, consumer purchasing patterns shift dramatically. This project analyzes **11,250+ sales transactions** from an Indian retail business to understand customer demographics, high-value customer cohorts, regional demand, and category preferences. The objective is to extract actionable business insights that enable sales teams and marketers to optimize inventory, improve target segmentation, and boost festive revenues.

---

## 🎯 Business Problem & Questions Answered
1. **Who buys more?** What is the breakdown between male and female purchasers in terms of transaction count and total spend?
2. **What age group dominates festive spending?** Which age cohort should marketing budget be targeted toward?
3. **Which geographic markets lead sales?** Which states and zones contribute the largest share of orders and total revenue?
4. **How does occupation correlate with spending power?** Which professions spend the most per order?
5. **Which product categories drive the highest revenue?** Which items are the top volume movers vs. margin drivers?

---

## 📊 Dataset Structure
The dataset (`Diwali Sales Data.csv`) contains **11,251 rows and 15 columns**:

| Column Name | Description |
|---|---|
| `User_ID` | Unique identifier for each customer |
| `Cust_name` | Customer full name |
| `Product_ID` | Unique identifier for each product |
| `Gender` | Gender of customer (`M` / `F`) |
| `Age Group` | Categorized age ranges (e.g., `0-17`, `18-25`, `26-35`, `36-45`, `46-50`, `51-55`, `55+`) |
| `Age` | Exact customer age |
| `Marital_Status` | Marital status indicator (`0` = Single, `1` = Married) |
| `State` | Customer's delivery state |
| `Zone` | Geographic zone (Northern, Southern, Western, Central, Eastern) |
| `Occupation` | Industry/Profession (IT, Healthcare, Aviation, Banking, Govt, etc.) |
| `Product_Category` | Category of purchased item (Food, Clothing, Electronics, Footwear, etc.) |
| `Orders` | Quantity of items ordered in the transaction |
| `Amount` | Total transaction value in INR |

---

## 🛠️ Data Cleaning & Preparation Workflow
1. **Handling Missing Values**:
   - Identified and dropped unpopulated tracking columns (`Status`, `unnamed1`).
   - Removed null values present in the `Amount` field to maintain calculation integrity.
2. **Data Type Casting**:
   - Converted float amounts into integer formatting for monetary aggregation.
3. **Statistical Validation**:
   - Checked distributions, summary statistics (`describe()`), and unique value cardinalities.

---

## 💡 Key Insights & Findings

### 1. Gender Spending Disparity
* **Women generate ~65%+ of total sales revenue** and command significantly higher order volume than men.

### 2. High-Converting Age Bracket
* The **26–35 age group** is the largest spender, contributing the highest order count and total gross merchandise value (GMV), followed by the 36–45 cohort.

### 3. Regional Powerhouses
* **Uttar Pradesh, Maharashtra, and Karnataka** dominate the top 3 state positions in both order quantity and total sales revenue.

### 4. Profession vs. Spending Capacity
* Customers working in **IT Sector, Healthcare, and Aviation** exhibit the highest average order value and total expenditure.

### 5. Best-Selling Product Lines
* **Food, Clothing & Apparel, and Electronics & Gadgets** generated the vast majority of festive revenue.

---

## 🚀 Strategic Business Recommendations
* **Target Audience Persona**: Married working women aged 26–35 living in urban areas of UP, Maharashtra, and Karnataka working in IT and Healthcare sectors.
* **Campaign Strategy**: Run targeted social media campaigns highlighting festive bundle discounts (e.g., matching apparel + sweets/food packs + electronics gifts).
* **Inventory Stocking**: Proactively allocate 60%+ warehouse capacity in Western and Northern regional hubs to avoid out-of-stock bottlenecks on top-selling SKUs.

---

## 💻 How to Run This Project
1. Clone this repository:
   ```bash
   git clone https://github.com/Salehaparween/Diwali_Sales_Analysis.git
   cd Diwali_Sales_Analysis
