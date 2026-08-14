# E-commerce Cohort & Retention Analysis
## Overview

This project focuses on analyzing e-commerce customer purchasing behavior using cohort analysis, customer retention analysis, Customer Lifetime Value (CLTV), and regional segmentation.

The project uses transactional sales data to understand customer purchasing patterns, measure retention over time, identify valuable customer segments, and generate business insights for customer retention and marketing decisions.

The final processed datasets are used to develop an interactive Power BI dashboard.
## Project Objective

The main objectives of this project are:

Prepare and clean the raw transactional dataset for analysis.
Perform Exploratory Data Analysis (EDA) to understand the dataset.
Create customer cohorts based on each customer's first purchase month.
Build a Customer Retention Matrix to analyze customer retention over time.
Calculate monthly customer retention percentages.
Compute Customer Lifetime Value (CLTV) using key financial metrics.
Segment customers by geographic region for comparative analysis.
Generate business insights to support customer retention and marketing decisions.
Prepare processed datasets for Power BI dashboard visualization.

## Tools Used

- SQL
- Power BI
- Excel
- Git & GitHub

## Dataset

The project uses an e-commerce transactional dataset named sales.csv.

## Data Cleaning & EDA

The raw dataset was loaded into Jupyter Notebook using Pandas.

The following steps were performed:

Checked dataset shape and structure.
Examined column names and data types.
Checked missing values.
Checked customer IDs.
Converted order_date into datetime format.
Converted Customer Since into datetime format.
Checked order status values.
Created the Sales column.
Created the OrderMonth column.
Prepared the cleaned dataset for further analysis.

The cleaned dataset was saved as sales_clean.csv.

## Cohort Analysis

Customers were grouped into cohorts based on their first purchase month.
### Cohort Month
The earliest purchase month of each customer was identified as their CohortMonth.
### Order Month
The transaction date was converted into a monthly period called OrderMonth.
Cohort Index
The difference between the customer's Order Month and Cohort Month was used to determine the Cohort Index.

## Customer Retention Matrix
The Customer Retention Matrix was created by grouping customers according to:
CohortMonth
CohortIndex
Unique customers were counted using nunique().

## Retention Percentage

Monthly retention percentage was calculated using:
Retention Percentage = (Retained Customers ÷ Initial Cohort Size) × 100
Month 0 represents the initial cohort size and is treated as the starting point for calculating subsequent retention percentages.

## Regional Segmentation

Customers were segmented based on their geographic Region.
For each region, the following metrics were analyzed:

Revenue
Average Order Value
Purchase Frequency
Historical CLTV
