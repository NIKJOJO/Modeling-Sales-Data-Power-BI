# Modeling Sales Data using Power BI

## Introduction

Welcome to my **Super Store** report, where I utilize Power BI to clean, transform, and visualize sales data in order to answer key business questions. In this project, I leverage the power of Power BI and Power Query to gain insights from the data.

## Ask

Before diving into the data analysis, it is crucial to define the business questions we aim to answer. Here are the questions we will address:

1. What were the total sales for the company in 2019?
2. Which country generated the highest average sales, and who were the top 5 customers within those countries?
3. What were the profits by product category, and which category was the most profitable?

## Prepare

To start the analysis, we import the database into PowerQuery. The dataset contains the following headers:


![data headers](https://github.com/NIKJOJO/Modeling-Sales-Data-Power-BI/blob/main/data%20headers.png)
- Order ID: All order IDs
- Customer ID: Customer information
- Customer Name: Name of the customer
- Segment: Product segments
- Country: Country of sales
- Market: Continent/market of sales
- Product ID: List of product IDs
- Category: Category of different products
- Sub-Category: Sub-category of products
- Product Name: Name of the product
- Sales: Sales of different products
- Quantity: Quantity of products sold
- Profit: Profit made

## Data Cleaning

Before conducting data analysis, it is essential to clean the data. In Power Query, the following cleaning steps were performed:
![power query](https://github.com/NIKJOJO/Modeling-Sales-Data-Power-BI/blob/main/power%20query.png)

- Removal of duplicate rows, with promotion of the second row to the header
- Adjustment of column data types to match their content appropriately
- Formatting of the "date" column to use a more consistent delimiter

## Data Transformation

Extracting specific information from the date column simplifies data analysis. I added two new columns using DAX:

- Extraction of the year from each row using the "YEAR" function
- Extraction of the month from each row using the "MONTH" function

## Data Analysis and Visualization

To gain insights from the data, the following steps were taken:

- Creation of a measure called "total sales" using the SUM function
- Utilization of a table visual to display total sales by category and year
- Generation of a bubble map visual to illustrate average sales by country
- Implementation of a pie chart to showcase profit by segment
- Inclusion of a list of the top 5 customers
	- Enabled drill-down functionality on the pie chart to view subcategories
- Addition of slicers to enhance interactivity



![overview of report](https://github.com/NIKJOJO/Modeling-Sales-Data-Power-BI/blob/main/Overview%20Report.gif)

## Answering the Original Questions

Based on the visualizations and analysis, we can provide answers to the original questions:

1. The total sales for the company in 2019 amounted to $1.8 Million.


![question1](https://github.com/NIKJOJO/Modeling-Sales-Data-Power-BI/blob/main/Question1.gif)


2. The country that generated the highest average sales is Lesotho. The top 5 customers within those countries are Volz, Rosenberg and Haberlin.


![question2](https://github.com/NIKJOJO/Modeling-Sales-Data-Power-BI/blob/main/Question2.gif)


3. The profits by product category are shown in the image below. The most profitable category is technology.


![question3](https://github.com/NIKJOJO/Modeling-Sales-Data-Power-BI/blob/main/Question3.gif)



## Conclusion

In conclusion, this **Super Store** report showcases the effective utilization of Power BI and Power Query to clean, transform, and visualize sales data, enabling us to answer key business questions and gain valuable insights. The visualizations and interactive features provided a comprehensive view of sales trends, customer behavior, and profitability, empowering stakeholders to make data-driven decisions, optimize strategies, and drive business growth.
