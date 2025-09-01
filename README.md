# Walmart-Sales-Data
## 📌 **About**

This project focuses on analyzing Walmart sales data to understand customer behavior, product performance, and branch-level trends. The main goal is to uncover insights that help improve sales strategies, identify top-performing branches and products, and study customer preferences.

The dataset used is a transactional sales record from Walmart branches, containing detailed information about invoices, product lines, customers, payments, and ratings.

## 🎯 **Purposes of the Project**

The objectives of this project are to:

Analyze sales trends across different branches and cities.

Identify the best-performing product lines and customer segments.

Understand how time (day, month, hour) impacts sales.

Gain insights into customer ratings and satisfaction.

Optimize sales strategies using data-driven decisions.

## 📊 **About the Data**

The dataset contains 1000 rows and 17 columns. Each row represents a customer transaction.

| Column Name               | Description                                   | Data Type      |
| ------------------------- | --------------------------------------------- | -------------- |
| `Invoice ID`              | Unique invoice number of the transaction      | VARCHAR(30)    |
| `Branch`                  | Branch code (A, B, C) where the sale happened | VARCHAR(5)     |
| `City`                    | City where the branch is located              | VARCHAR(30)    |
| `Customer type`           | Type of customer (e.g., Member, Normal)       | VARCHAR(30)    |
| `Gender`                  | Gender of the customer                        | VARCHAR(10)    |
| `Product line`            | Category of the product sold                  | VARCHAR(100)   |
| `Unit price`              | Price of a single unit                        | DECIMAL(10, 2) |
| `Quantity`                | Number of units purchased                     | INT            |
| `Tax 5%`                  | Tax charged on the purchase (5%)              | FLOAT(6, 4)    |
| `Total`                   | Final purchase amount (with tax)              | DECIMAL(12, 4) |
| `Date`                    | Date of the purchase                          | DATE           |
| `Time`                    | Time of the purchase                          | TIME           |
| `Payment`                 | Mode of payment (Cash, Credit card, Ewallet)  | VARCHAR(20)    |
| `cogs`                    | Cost of Goods Sold                            | DECIMAL(10, 2) |
| `gross margin percentage` | Gross margin percentage                       | FLOAT(11, 9)   |
| `gross income`            | Gross profit from the transaction             | DECIMAL(12, 4) |
| `Rating`                  | Customer rating (scale of 1–10)               | FLOAT(2, 1)    |


## 🔎 **Analysis Approach**
1. Data Wrangling

Created a MySQL database and imported the dataset.

Checked for NULL values (none found, as all fields were NOT NULL).

Verified data types for accuracy.


### 2. **Feature Engineering**


To make the analysis more insightful, additional columns were derived:

time_of_day → Categorized into Morning, Afternoon, Evening.

day_name → Extracted weekday name from the date.

month_name → Extracted month name from the date.

These features helped analyze sales by time, weekday, and month.

### 3. **Exploratory Data Analysis (EDA)**

SQL queries were written to answer key business questions related to products, sales, and customers.

## ❓ **Business Questions Answered**
## 🛒 **Product Analysis**

How many distinct product lines are there?

Which product line sells the most?

Which product line generates the highest revenue?

Which product line has the highest average rating?

Which product line incurs the most VAT?

## 💰 **Sales Analysis**

What is the total revenue by month?

Which month recorded the highest Cost of Goods Sold (COGS)?

Which branch sells more products than average?

Which city generates the highest revenue?

What are sales trends by time of day and day of week?

## 👥 **Customer Analysis**

How many unique customer types exist?

Which customer type generates the highest revenue?

Which customer type pays the most VAT?

Which gender shops the most?

What is the gender distribution per branch?

Which day/time do customers give the highest ratings?

## 🛠️ **Tools & Technologies Used**

MySQL – Database management and queries.

CSV Data Import – For Walmart sales dataset.

SQL Queries – For data cleaning, feature engineering, and analysis.

Workbench/CLI – For executing and visualizing queries.

## ✅ **Outcomes & Insights**

Discovered which product lines perform best and worst.

Identified the most profitable city and branch.

Learned about customer preferences in payment methods and product categories.

Understood peak sales times during the day and week.

Found out how customer ratings vary by time and branch.
