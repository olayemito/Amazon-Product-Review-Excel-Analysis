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
I created a new sheet called 'Data Cleaning Sheet' to perform the processes below:
I removed duplicated Product IDs by using the remove duplicate command to have unique products.
I separated the category column to have the main category from other sub categories of each products  using the 'text to column' command and use the delimiter '|' to make the split.
I removed blanks from the rating column using filter button.
Removed a product that did not have a rating content using the filter button as well as a product. 
Created the "Total Product Revenue" column using theh Product Function (product of the actual price and the rating count).
I created the 'Discount Percentage Range' column from the discount percentage column using the functions below:
          '=IF(K2<50%, "<50%", "50% or more")'
Created the discounted price column using the formula:
          'actual price * (discountpercentage/100%)' 
I used the Proper function to correct the product names.
I Splited the review IDs using the text to columns and delimiter into individual IDs and used count to create another column to have the number of each products number of review IDs.
I created another sheet named 'Cleaned Data Set' 
I ensured that all columns datatype were correctly aligned with the type of data they contain.
Here, I moved all the cleaned dataset and created a table with them.

### Descriptive Statistics
Here, I used the table from the cleaned dataset to make pivot tables based on the analysis tasks given on a new sheet titled 'Pivot Tables':



