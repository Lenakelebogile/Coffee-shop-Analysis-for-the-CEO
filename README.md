# Coffee-shop-Analysis-for-the-CEO
This repository contains a detailed  analysis for coffee shop with different location,the goal of this is to get a clear understanding  of the revenue trends,sales trends across  products and the time intervals ,what time of the day does the store seems to have high sales it also looks at the customer behaviour and identifiyes strategies on how to grow the business

SUMMARY OF FINDINGS 

Revenue increase from month to month
The three stores contributed nearly the same revenue
Sales by time of the day (highest to lowest)
Morning 
Afternoon
Evening 
Product contribution  coffeee and tea contributed the most revenue the most revenue while others products contributed less
Most of thier revenue is done mostly on the morning and the afternoon 
The sales drops during mid-day  hours releveled gaps in lunch offering 
our stores had signaificanlty   higher morning revenue-potential for breakfast promotions 
Percentage of the profit is ranging from 50% to 85%

RECOMMENDATIONS

Boosts inventory for the top selling items to meet demands and increase revenue during peak hours
Optimise stock levels  and products placement 
To introduce targeted promotions in order fro incentives
Marketing campaigns during slow time slots
Stock more of the best-selling items
Promote underperforming products
PERIOD
This anlysis was done in 4 weeks Looking at the Morning  Afternoon Evening periods
 
PROBLEM STATEMENT
Bright Coffee Shop is a retail coffee business currently undergoing a leadership transition with the appointment of a new CEO. To support the CEO’s strategic goal of increasing revenue and improving product performance, there is a need to extract actionable insights from historical transactional data collected at the store level.
The core challenge is to analyze this sales data to identify:
Which products contribute the most to revenue
When during the day the store experiences the highest and lowest sales
Trends in customer purchasing behavior over time
Underperforming product categories that may need adjustment
The analysis must not only answer these questions but also guide the CEO with data-driven recommendations on sales optimization, inventory planning, and marketing strategies.

The Aim of the project
You have been provided with a dataset titled “Bright Coffee Shop Sales”, which captures daily transactional information from a coffee shop. The business has recently appointed a new CEO whose mission is to grow the company’s revenue and improve product performance. Your role, as a Junior Data Analyst, is to extract actionable insights from historical data and prepare a presentation to assist the CEO in decision-making.

METHODS USED

Microsoft SQL Server
Databricks
DBeaver
SQL Developer
Google BigQuery
MySQL Workbench

TOOLS ALLOWED

Coding Platforms:
Microsoft SQL Server
batabricks
DBeaver
SQL Developer
Google BigQuery
MySQL Workbench
Data Visualization:
Microsoft Excel
Power BI
Tableau
Google Sheets
Presentation & Reporting:
Microsoft PowerPoint
Canva
Miro
Figma

OBJECTIVES OF THIS ANALYSIS

Use your analytics, SQL, and data visualization skills to help Bright Coffee Shop understand:
Which products generate the most revenue
What time of day the store performs best
Sales trends across products and time intervals
Recommendations for improving sales performance

PROJECT STRUCTURE

DATA Raw and aggrigated dat 
SQL Code snowflake scripts
Documents:Case study,Miro footprint and Methodology
PIVOT TABLE
PRESENTATION Is in the presentation mode

2. List the Key Insights that the team should deliver, such as:
   
Sales by product category and time intervals
High-performing and low-performing products
Total revenue calculations

4. Outline the calculations to be performed:
   
Total Amount = unit_price * transaction_qty
Grouping by 30-minute time intervals
Total units sold by product type or detail
You can add on the above, this is just to give you an idea of what is expected from the Miro planning.

Task 2: Data Processing in Snowflake

1. Convert the provided Excel data to CSV.
2.Load the CSV into Snowflake
3. Perform data transformations:
Create a new column: transaction_time_bucket to group transactions into 30-minute intervals (Or it can be 1 hour intervals)
Cast unit_price properly (some entries use commas, e.g., '3,1' should be converted to 3.1)
Compute total_amount = unit_price * transaction_qty
Use SQL to group by product types, time buckets, etc.
You can add on the above, this is just to give you an idea of what is expected from the Data Processing.

Task 3: Data Analysis in Excel

After processing the data in Snowflake: 1. Export the processed table to Microsoft Excel or your visualization tool 2. Create dashboards or pivot tables showing:
al revenue per product type
Peak time intervals for sales
Quantity of items sold by product category
Best-selling product types or details
Use charts and graphs to make the story visually appealing

Task 4: Presentation to the CEO

Prepare a Presentation to deliver insights to the CEO. Include:
1. Overview of your approach – Create a separate document for your Methodology
2.   Key insights from your analysis (backed by visuals) – Create a separate document for your Presentation
   

5. Next Steps:
Automate daily sales reporting
Track sales performance across multiple locations in the future
Implement loyalty programs based on peak customer time slots


