# Olist-Ecommerce-Analysis

## Project Background
Olist is a Brazillian technology company that operrates as an online market place connecting small businesses to customers. The platform allows sellers to list their products, manage orders and handle payments through Olist's system.

The company has significant amount of data on it's sales that has previously been underutilized. This project thoroughly analyzes and synthesizes the data in order to uncover critical insights that will imporve Olist's commercial success.

Insihgts and recommendations are provided on the following key areas:

- Sales Trend Analysis: Evaluation of historical sales pattern focusing on revenue, order volumn and average order value
- Product level performance: An anlysis of Olist's various product categories and understanding their impact on sales
- Seller level performance: Understanding seller ratings and how they impact seller's performance
- Loyalty program: An assessment of customer's retention rate and how it impacts sales

Interactive dashboard can be found [here](Olist.pbix)

Summary of ETL and data cleaning steps can be found [here](ETL_and_data_cleaning_steps.pdf)

Data cleaning file (done in python) can be found [here](Data_Cleaning_Pandas.ipynb)

Summary of Metric/KPI validation in sql can be found [here](Data_metric_validation.pdf)

SQL queries can be accessed [here](Sql_validation.sql)

Report pdf can be found [here](Olist_report.pdf)


## Data Structure

Olist's database structue consists of nine tables namely geolocation, customers, sellers, products, orders, order_items, order_reviews & order_payments & product_category_name. The state table was added to ensure full names of state are availble and date table was added to enable flexibility of time based analysis and creating hierarchical relationships at different levels of granularity (such as Day, Week, Month, Year etc.)



![Screenshot 2025-05-26 164200](https://github.com/user-attachments/assets/9f75e785-07b6-4a46-93bc-8ba83006730e)

Prior to analyzing the data, cleaning was done in python. Python file can be found [here](Data_cleaning_pandas.pdf)

## Executive Summary

**Overview of Findings**

Total Revenue recordes is R$ 15.42 Million, total orders placed stand at 99,441 and Average Order Value is R$160. Sales and order saw a near consistent rise in revenue from October 2016 to November 2017. Ater peaking in November, 2017 there was a sharp drop in December and since then the sales and orders have been stagnant. The peak in November can be attributed to Black Friday. It was surprising not to oberve similar peaks in Carnival and Christmas season. Sao Paulo, Rio De Janeiro, and Minais Gerais contribute 62.54% of the total revenue. Bed_bath_table sells the most products followed by health_beauty and sports_leisure.

Below is the overview page from Power BI desktop and more examples are included throughout the report. The entire dashboard can be downloaded from [here](Olist.pbix)


![Screenshot 2025-05-26 185949](https://github.com/user-attachments/assets/e2c39b4a-f05c-4ffa-9615-558a2fde0d0c)

**Revenue and Orders Trend Analysis**

Revenue and orders show a consistent increase in revenue and orders from October 2016 to peaking in November 2017, the revenue and orders have remained stagnant since. A sharp rise in revenue was observed in November 2017. Furhter analyzing the daily revenue, we uncover that 24th November, 2017 recorded the highest daily revenue ever of R$175,250 which is more than 3 times the second highest daily revenue. Unfortunately, we don't ahve the data available for November 2016 and November 2018 which would have enabled us to gain deeper insights on the effect of Black Friday sales. However, one thing is certain from our Black Friday peak is that festivites and sale drive high revenue. Hence, it was surprising when we didn't observe similar peaks in Carnival and Christmas 

![Screenshot 2025-05-26 195320](https://github.com/user-attachments/assets/acea2d59-1657-417c-8c5f-679c8e1e6195)



