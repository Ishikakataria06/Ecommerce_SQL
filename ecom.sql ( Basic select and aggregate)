create database ecom;
use ecom;
select * from customer;   # 350 rows , which 350 customers record

# female details 
select * from customer where gender = "Female";  # 175 females

# Male details 
select * from customer where gender = "Male";   # 175 male 

# Country : 6 countries data - Los angeles,Chicago,San Francisco,Miami,Houston
select distinct city 
from customer;

# max customer age  - 43
select max(age)
from customer;

# min customer age - 26
select min(age)
from customer;

# customer who have applied discount coupons 
select * from customer where Discount_Applied ="True"; # 175 customers applied the coupon

# out of 175 customer who applied the coupon 117 are females and 58 are males
select * from customer where Discount_Applied = "True" and Gender = "Female";
select * from customer where Discount_Applied = "True" and Gender = "Male";

# customer who are unsatisfied 
# 116 customer are unsatisfied
select * from customer where Satisfaction_Level = "unsatisfied";

# customer who are satisfied 
# 125 customer are satisfied
select * from customer where Satisfaction_Level = "satisfied";

# customer who are neutral 
# 107 customer are neutral
select * from customer where Satisfaction_Level = "Neutral";

# total spend amount - 295883.59
select sum(total_spend)
from customer;

# customer who have spend more than 500 - 267 customer have spend more than 500 
select * from customer where total_spend>500;

# customer who have spend less than 500 - 83 customer spend less than 500
select * from customer where total_spend<500;

# highest number of item purchased - 21
select max(Items_purchased)
from customer;

# lowest number of item purchased - 7
select min(Items_purchased)
from customer;

# Avg of total spend by gold members 
select customer_id,city,Membership_Type,avg(total_spend)
from customer 
where membership_type="Gold"
group by 1,2
order by customer_id desc;

# customer whi have purschase item between 10 and 20
select * 
from customer 
where items_purchased between 10 and 20;

# days since last purchase  - 63 days
select max(days_since_last_purchase)
from customer;

