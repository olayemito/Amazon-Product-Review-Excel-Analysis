# Amazon-Product-Review-Excel-Analysis
Comprehensive Documentation of My Analysis for the DSA Amazon Product Review Capstone Project

## Overview
This repository presents an Exploratory Data Analysis (EDA) conducted on the [Amazon Product Rewiew] dataset using Microsoft Excel.

## EDA Steps
1. [Data Import](#data-import)
2. [Data Cleaning](#data-cleaning)
3. [Descriptive Statistics](#descriptive-statistics)
4. [Data Visualization](#data-visualization)
5. [Insights and Conclusions](#insights-and-conclusions)

### Data Import
I launched Excel, imported the Amazon Study Case file and imported it into the excel workspace.

### Data Cleaning
I created different sheets for each process of the analysis, from 'raw data' to 'dashboard'.
- I created a new sheet called 'Data Cleaning Sheet' to perform the processes below:
- I removed duplicated Product IDs by using the remove duplicate command to have unique products.
- I separated the category column to have the main category from other sub categories of each products  using the 'text to column' command and use the delimiter '|' to make the split.
- I removed blanks from the rating column using filter button.
- Removed a product that did not have a rating content using the filter button as well as a product.
- Created the "Total Product Revenue" column using theh Product Function (product of the actual price and the rating count).
- I created the 'Discount Percentage Range' column from the discount percentage column using the functions below:
          '=IF(K2<50%, "<50%", "50% or more")'
- Created the discounted price column using the formula:
          'actual price * (discountpercentage/100%)' 
- I used the Proper function to correct the product names.
- I Splited the review IDs using the text to columns and delimiter into individual IDs and used count to create another column to have the number of each products number of review IDs.
- I created another sheet named 'Cleaned Data Set'
- I ensured that all columns datatype were correctly aligned with the type of data they contain.
Here, I moved all the cleaned dataset and created a table with them.

### Descriptive Statistics
Here, I used the table from the cleaned dataset to make pivot tables based on the analysis tasks given on a new sheet titled 'Pivot Tables':
I created the first pivot table to find the Average Discount % by Product Category by using the Product Category (Row bucket) and discount Percentage (Values bucket).
Total Products listed in each Category with product Category (Row bucket) and Count of Product ID (values bucket).
Total number of reviews per category and categories with highest ratings with Product Category (Row bucket) and Sum of rating count (values bucket).
Average Price vs Discounted Price by Category with product category (row bucket) and average of actual and discounted prices (values bucket).
Products with the Highest number of Reviews with Product Name (row bucket) and Sum of rating_count (values bucket); top 10 products.
Products that have a discount of 50% or more with Product ID (row bucket) and count of product ID (values bucket) with filters on selecting 50% or more.
Distribution of product ratings with rating (row bucket) and count of product name (values bucket).
Total Potential Revenue by Category with product category (row bucket) and sum of Total Potential Revenue (values bucket).
Number of Unique Products per Price Range Bucket with Discount Price Range Bucket (row bucket) and Count of product ID (values bucket).
Rating related to the level of discount with Discount percentage (row bucket) and Average of rating (values bucket).
Products with fewer than 1,000 Reviews with product ID (row bucket) and Sum of rating count (values bucket), used filter option 'Less than or equal to' to set the sum count to 1,000 reviews and less then used the count function to count the total number of products with less tha 1,000 reviews.
Products Category with the Highest Discounts with Product Category (row bucket) and maximum of discount percentage (values bucket).
Top 5 Products by Rating and Number of Reviews Combined with Product name (row bucket) and sum of combined Score (values bucket). I created a calculated column to calculated the combined score with the formula:
                              'Combined Score= (Average Rating * Sum of Reviews)'

### Data Visualisation
Here, I created a new sheet to create my Excel Dashboard from the pivot tables I create from the previous sheet. I create appropriate charts and cards based on each pivot table already created. I used Piecharts, Donutchart, line graphs, clustered columns, textboxes as cards and clustered bars to visualise each table appropriately.

### Insights and Conclusions


