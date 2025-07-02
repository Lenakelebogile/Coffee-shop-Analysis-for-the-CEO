--I was counting the number of rows in my  excel sheet
select count(TRANSACTION_ID) AS number_of_sales
from transactions.coffee_shop.bright;

--I was counting the number Of units sold 
select SUM(transaction_qty) AS number_of_units_sold
from transactions.coffee_shop.bright;

--Calculating the Revenue per transaction
select transaction_qty* unit_price AS revenue_per_transaction
from transactions.coffee_shop.bright;


--Calculating the total revenue
select sum (transaction_qty* unit_price) AS total_revenue
from transactions.coffee_shop.bright;
--grouping by product category AND order by
select sum (transaction_qty* unit_price) AS total_revenue,
           product_category
from transactions.coffee_shop.bright
GROUP BY PRODUCT_CATEGORY
order by total_revenue DESC

--calculating minimum tranction time
--get the earliest time in which the time opens
select min(transaction_time)
from transactions.coffee_shop.bright

--calculating minimum tranction time
--to get the time in which the shop closes
select max(transaction_time)
from transactions.coffee_shop.bright

--Final query for analysis
select
sum (transaction_qty*unit_price) AS total_revenue,
SUM (transaction_qty) AS number_of_units_sold,
count(TRANSACTION_ID) AS number_of_sales,

TO_CHAR(TRANSACTION_DATE,'YYYYMM') AS month_id,
monthname(transaction_date)as month_name,
dayname(transaction_date) as day_name,

case

when transaction_time between '06:00:00' and '11:59:59' then 'morning'
when transaction_time between '12:00:00' and '15:59:59' then 'afternoon'
when transaction_time between '16:00:00' and '20:00:00' then 'evening'
ELSE'night'
end as time_bucket,

case

WHEN SUM (TRANSACTION_QTY*UNIT_PRICE)BETWEEN 0 AND 20 THEN 'LOW'
WHEN SUM (TRANSACTION_QTY*UNIT_PRICE)BETWEEN 21 AND 40 THEN 'MED'
WHEN SUM (TRANSACTION_QTY*UNIT_PRICE)BETWEEN 41 AND 60 THEN 'HIGH'
ELSE'Very high'
end as spend_bends,

        PRODUCT_CATEGORY,
        product_type,
        product_detail,
        store_location
from transactions.coffee_shop.bright
group by time_bucket,
         PRODUCT_CATEGORY,
         product_type,
         product_detail,
         store_location,
         month_id,
         month_name,
         day_name;
         
