# E-commerce Inventory Intelligence: SQL-Based Business Analysis
I analyzed a real-world e-commerce inventory dataset to uncover pricing inefficiencies, stock risks, and revenue opportunities using SQL

Problem Statement:- E-commerce platforms often struggle with:
Inconsistent pricing formats
Duplicate SKUs across product variations
Stockouts in high-value products
Unclear visibility into revenue potential

In this project, I built a structured SQL workflow to clean, analyze, and extract actionable insights from such data.

📂 Dataset Overview
Source: Zepto inventory dataset (Kaggle)
Granularity: SKU-level data
Real-world characteristics: duplicates, inconsistencies, mixed units
Key Columns:
sku_id – Unique product identifier
name – Product name
category – Product category
mrp – Maximum Retail Price (₹)
discountPercent – Discount applied
discountedSellingPrice – Final price
availableQuantity – Inventory units
weightInGms – Product weight
outOfStock – Stock availability
quantity – Units per package

⚙️ Tech Stack
SQL (PostgreSQL)
pgAdmin
CSV Data Processing

My Approach
🏗️ Data Setup
Designed SQL table with appropriate schema
Imported raw dataset into PostgreSQL
Resolved encoding issues (UTF-8 errors)
🔍 Data Exploration
Analyzed SKU distribution and category spread
Identified null values and inconsistencies
Compared in-stock vs out-of-stock products
Detected duplicate SKUs (product variations)
🧹 Data Cleaning
Removed invalid records (MRP = 0)
Converted pricing from paise to rupees
Standardized pricing columns for consistency
📊 Business Analysis

I focused on solving real business questions:

Which products offer the highest discounts?
Which high-value products are out of stock?
What is the revenue potential by category?
Which products are overpriced relative to value?
Which products deliver best value per gram?
💡 Key Business Findings
High-value products (₹500+) frequently go out of stock → direct revenue leakage
Some categories rely heavily on discounts → potential margin pressure
Price-per-gram analysis exposed hidden overpriced products
Duplicate SKUs indicate catalog visibility optimization strategies
📈 Business Impact

This analysis can directly support:

📦 Inventory optimization (reduce stockouts)
💰 Pricing strategy improvements
📊 Revenue estimation at category level
🛒 Better product positioning
🧩 SQL Skills Demonstrated
Aggregations (SUM, AVG, COUNT)
Filtering & conditional logic
CASE WHEN (segmentation)
Data cleaning using SQL
Derived metrics (price per gram, revenue estimation)
Ranking & sorting (Top-N analysis)
