# Amazon Product Review Analysis - Excel Dashboard
Comprehensive Exploratory Data Analysis for DSA Capstone Project

## Overview
This repository documents an Excel-based Exploratory Data Analysis (EDA) of Amazon product reviews, featuring a dynamic dashboard for actionable insights.

## EDA Steps
1. Data Import
2. Data Cleaning
3. Descriptive Statistics
4. Data Visualization
5. Insights and Conclusions

### Data Import
Imported raw dataset ("Amazon Study Case") into Excel workspace

### Data Cleaning
(Executed in dedicated 'Data Cleaning Sheet')
- Removed duplicate Product IDs
- Split category column using | delimiter to isolate primary categories
- Filtered out blank ratings and incomplete entries
- 
**Generated key metrics:**
- Total Product Revenue: Actual Price × Rating Count
- Discounted Price: Actual Price × (1 - Discount Percentage)
- Discount Tier: Categorized discounts as <50% or ≥50%
- Standardized product names with PROPER() function
- Separated Review IDs and calculated review counts
Finalized structured dataset in 'Cleaned Data Set' sheet

### Descriptive Statistics
(Pivot Tables in dedicated sheet)

|Analysis Focus | Key Metrics | Fields Used|
----------------|-------------|------------|
|Category Performance | Avg. Discount %, Product Count| Category × Discount %|
|Review Analysis | Total Reviews, Top-Rated Categories | Category × Rating Count|
|Pricing Strategy | Avg. Actual vs. Discounted Price | Category × Price Metrics|
|High-Impact Products | Top 10 by Reviews, Top 5 by Combined Score| Product × Rating Count|
|Discount Dynamics | Products with ≥50% discount, Max Discount by Category | Discount Tier × Product Count|
|Revenue Forecasting | Total Potential Revenue by Category | Category × Revenue|
|Rating Distribution | Score frequency | Rating × Product Count|

### Data Visualization
Built interactive dashboard with:
Pie/Donut Charts: Category distribution
Clustered Columns: Pricing analysis
Bar Graphs: Review performance
Text Cards: Key KPIs
Line Graphs: Trend identification

### Insights & Conclusions
Download Full Analysis [here](Amazon-case-Study-Solutions.xlsx)
(Dashboard highlights actionable insights for pricing optimization, inventory planning, and category strategy)
