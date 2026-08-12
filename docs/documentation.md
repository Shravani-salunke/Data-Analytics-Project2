<!-- Objectives -->
Prepare and clean the raw transactional dataset for analysis.
Perform Exploratory Data Analysis (EDA) to understand the dataset.
Create customer cohorts based on each customer's first purchase month.
Build a Customer Retention Matrix to analyze customer retention over time.
Calculate monthly customer retention percentages.
Compute Customer Lifetime Value (CLTV) using key financial metrics.
Segment customers by geographic region for comparative analysis.
Generate business insights to support customer retention and marketing decisions.
Prepare processed datasets for Power BI dashboard visualization.

<!-- Tasks Completed -->
Week 1 –
Data Cleaning & Wrangling
Loaded the sales.csv dataset into Jupyter Notebook.
Imported Python libraries (Pandas, NumPy, Matplotlib, Seaborn).
Explored dataset structure (shape, columns, info(), describe()).
Checked and handled missing values.
Converted order_date to datetime format.
Filtered successful transactions based on the status column.
Verified customer IDs (cust_id) for missing values.
Created the Order Month.
Calculated the Cohort Month (customer's first purchase month).

Week 2 –
Cohort Retention Analysis
Calculated the Cohort Index.
Grouped customers by Cohort Month and Cohort Index.
Built the Customer Retention Matrix using groupby() and pivot_table().
Calculated the number of retained customers.
Computed monthly retention percentages.
Exported the retention matrix for visualization.
Analyzed customer retention trends.

Week 3 – 
Customer Lifetime Value (CLTV)
Calculated transaction-level Sales.
Computed Total Revenue.
Calculated Total Orders.
Calculated Total Customers.
Calculated Average Order Value (AOV).
Calculated Purchase Frequency.
Computed Historical CLTV.
Segmented customers by Region.
Calculated Region-wise Revenue, AOV, Purchase Frequency, and Historical CLTV.
Identified high-performing and low-performing regions.
Exported the CLTV dataset for dashboard development.

<!-- Formulae Used -->
1. Sales
Formula:
Sales = (Price × Quantity Ordered) − Discount Amount

2. Total Revenue
Total Revenue = Sum of Sales

3. Total Orders
Total Orders = Number of Unique Order IDs

4. Total Customers
Total Customers = Number of Unique Customer IDs

5. Average Order Value (AOV)
AOV = Total Revenue ÷ Total Orders

6. Purchase Frequency
Purchase Frequency = Total Orders ÷ Total Customers

7. Historical Customer Lifetime Value (CLTV)
Historical CLTV = Average Order Value × Purchase Frequency

8. Retention Percentage
Retention Percentage =
(Retained Customers ÷ Initial Cohort Size) × 100

Week 4 – Power BI Dashboard Development

Add this after Week 3:

Week 4 – Power BI Dashboard & Reporting
Imported the processed datasets into Power BI.
Connected the cohort retention and CLTV datasets.
Created KPI cards for:
Total Revenue
Total Customers
Total Orders
Average Order Value (AOV)
Purchase Frequency
Historical CLTV
Created the Customer Retention Heatmap.
Created retention trend/line charts.
Added regional analysis visuals.
Added slicers for interactive filtering.

<!-- Business Recommendations -->
Focus retention campaigns on cohorts showing significant retention decline.
Introduce loyalty programs to encourage repeat purchases.
Target high-CLTV regions with personalized marketing campaigns.
Use promotional offers to improve repeat purchases in low-performing regions.
Monitor cohort retention regularly to identify early signs of customer churn.
Use CLTV and purchase frequency to prioritize valuable customer segments.

<!-- Conclusion -->

This project analyzed e-commerce customer purchasing behavior using cohort and retention analysis. The data was cleaned and explored using Python and Pandas, followed by cohort creation and customer retention analysis. CLTV and regional analysis were performed to understand customer value and geographic performance. The processed datasets were then used to develop an interactive Power BI dashboard. The analysis provides useful insights into customer retention, purchasing behavior, customer value, and regional performance, supporting data-driven marketing and retention decisions.