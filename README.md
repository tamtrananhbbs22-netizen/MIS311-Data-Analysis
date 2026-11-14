# MIS311-Data-Analysis
Data analysis projects and insights for MIS 311
# Project 1: Supermarket Sales Data Analysis

## 1. Project Overview

This project focuses on analyzing supermarket sales data using Microsoft Excel and Power Query. The main purpose is to understand sales performance, prepare the dataset, calculate descriptive statistics, and identify useful business insights.

## 2. Data Overview
<img width="1057" height="796" alt="image" src="https://github.com/user-attachments/assets/aa9ec6ce-af97-4810-b791-4ea39cbc9c07" />
<img width="1211" height="355" alt="image" src="https://github.com/user-attachments/assets/7dad45b6-4adf-40e2-b441-2f848c3dbac5" />


### 2.1 Data Source

The dataset used in this project contains supermarket sales transactions, including information about branches, cities, customer types, products, quantities, and total prices.

### 2.2 Dataset Structure

The original dataset contains 253 records and 8 columns.

The main variables include:

- `sale_id`: Unique identification number for each transaction.
- `branch`: The supermarket branch.
- `city`: The city where the transaction occurred.
- `customer_type`: Customer classification.
- `product_name`: Name of the purchased product.
- `product_category`: Product category.
- `quantity`: Number of products purchased.
- `total_price`: Total price of each transaction.

### 2.3 Initial Data Inspection

The original dataset was reviewed to understand its structure, identify missing values, and check for duplicate records before performing data cleaning and preparation.
## 3. Data Cleaning and Preparation

Data cleaning and preparation were performed using Microsoft Excel and Power Query to improve data quality and ensure the dataset was suitable for further analysis.

### 3.1 Identifying Missing Values

The Column Quality feature in Power Query was used to identify missing values in the dataset. The inspection revealed blank values in the `customer_type`, `product_category`, and `quantity` columns.

### 3.2 Removing Duplicate Records

Duplicate records were identified and removed to ensure that each transaction was represented only once. After removing duplicates, the dataset contained 250 records.

### 3.3 Handling Missing Values

Missing values were handled using appropriate statistical methods:

- Customer Type: Blank values were replaced with the mode.
- Quantity: Blank values were replaced with the median.
- Product Category: Missing categories were corrected based on the corresponding product names.

### 3.4 Correcting Product Categories

A Conditional Column was created in Power Query to assign the appropriate category to each product.

The corrected product categories included:

- Shampoo – Personal Care
- Detergent – Household
- Apple – Fruits
- Orange Juice – Beverages
- Notebook – Stationery
The corrected categories improved data consistency and ensured that products were assigned to the appropriate groups.
### 3.5 Final Dataset

After completing the cleaning and transformation process, the dataset contained 250 records and was ready for further statistical analysis.
## 4. Descriptive Statistics

Descriptive statistics were used to summarize the numerical variables in the cleaned supermarket sales dataset. This analysis focused on Quantity and Total Price to understand purchasing patterns and transaction values.

### 4.1 Quantity

The Quantity variable represents the number of products purchased in each transaction. Measures such as mean, median, standard deviation, minimum, and maximum were calculated to understand product purchasing patterns.
<img width="317" height="382" alt="image" src="https://github.com/user-attachments/assets/cf1c0e5a-2cbd-4663-a37b-c969fb33ea8c" />

### 4.2 Total Price

The Total Price variable represents the total value of each sales transaction. Descriptive statistics were calculated to examine transaction values and understand customer spending patterns.
<img width="367" height="375" alt="image" src="https://github.com/user-attachments/assets/9924ca9a-bfc2-4530-8349-cb67b1d01eef" />
## 5. Data Analysis and Business Insights

After completing data cleaning and descriptive statistical analysis, further analysis was conducted to examine supermarket sales performance across different cities and branches.

### 5.1 Total Sales by City
<img width="1007" height="425" alt="image" src="https://github.com/user-attachments/assets/bd9066e4-6bf3-47af-8eea-6a260b862fbb" />

This analysis compares total sales across three cities to identify differences in sales performance.

The results show that Chicago generated the highest total sales of $11,133.05, followed closely by New York with $10,964.42. Los Angeles recorded the lowest sales at $8,948.81.

**Business Insight:** Chicago and New York demonstrated relatively similar sales performance, while Los Angeles had lower total sales. The supermarket could further investigate customer demand and sales opportunities in Los Angeles.

### 5.2 Total Sales by Branch
<img width="1012" height="410" alt="image" src="https://github.com/user-attachments/assets/9270acef-ce13-4338-b712-7e8e56815b0b" />

This analysis compares the total revenue generated by Branch A and Branch B.

Branch A achieved total sales of $22,097.47, significantly higher than Branch B, which generated $8,948.81. Branch A accounted for approximately 71.2% of total sales.

**Business Insight:** Branch A is the stronger contributor to overall revenue. The business could investigate the factors behind its performance and identify opportunities to improve sales at Branch B.
### 5.3 Total Quantity Sold by Branch
<img width="1170" height="415" alt="image" src="https://github.com/user-attachments/assets/e1675e62-2ae5-4f4e-b9a7-1058d70ead3e" />

This analysis compares the total quantity of products sold by Branch A and Branch B to evaluate their sales volume.

The results help identify which branch sold a larger number of products and provide additional information about differences in branch performance.

**Business Insight:** Comparing total quantity sold with total sales revenue can help the business understand whether a branch generates higher revenue because it sells more products or because its transactions have higher values.
