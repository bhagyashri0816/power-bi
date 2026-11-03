# CREDIT CARD WEEKLY STATUS REPORT 
To develop a comprehensive credit card weekly dashboard that provides real-time insights into key performance metrics and trends, enabling stakeholders to monitor and analyse credit card operations effectively.

## Content in this Project:  
1. Project objective 
2. Data from CSV 
3. Data processing & DAX 
4. Dashboard & insights 
5. Export & share project 

## Git Hub Link
https://github.com/bhagyashri0816/power-bi 
<br>
or
<br>
Google Drive: Click Here

# DAX Queries

AgeGroup = SWITCH( 
<br>
TRUE(), 
<br>
'public cust_detail'[customer_age] < 30, "20-30", 
<br>
'public cust_detail'[customer_age] >= 30 && 'public cust_detail'[customer_age] < 40, "30-40", 
<br>
'public cust_detail'[customer_age] >= 40 && 'public cust_detail'[customer_age] < 50, "40-50", 
<br>
'public cust_detail'[customer_age] >= 50 && 'public cust_detail'[customer_age] < 60, "50-60",  
<br>
'public cust_detail'[customer_age] >= 60, "60+", 
<br>
"unknown"
<br>

) 
<br>
IncomeGroup = SWITCH(
<br>
TRUE(), 
<br>
'public cust_detail'[income] < 35000, "Low", 
<br>
'public cust_detail'[income] >= 35000 && 'public cust_detail'[income] <70000, 
<br>
"Med", 
<br>
'public cust_detail'[income] >= 70000, "High", 
<br>
"unknown" 
<br>
)
<br>

week_num2 = WEEKNUM('public cc_detail'[week_start_date]) 
<br>
Revenue = 'public cc_detail'[annual_fees] + 'public cc_detail'[total_trans_amt] + 'public cc_detail'[interest_earned]
<br>


## Project Insights- Week 53 (31st Dec) 

# WoW change:  

• Revenue increased by 28.8%, 
<br>
• Total Transaction Amt & Count increased by xx% & xx% 
<br>
• Customer count increased by xx% Overview YTD:
<br>
• Overall revenue is 57M 
<br>
• Total interest is 8M 
<br>
• Total transaction amount is 46M 
<br>
• Male customers are contributing more in revenue 31M, female 
<br>
26M 
<br>
• Blue & Silver credit card are contributing to 93% of overall 
<br>
transactions 
<br>
• TX, NY & CA is contributing to 68% 
<br>
• Overall Activation rate is 57.5%
<br>
Note:  
<br>
You can add more insights 
<br>
• Overall Delinquent rate is 6.06%
<br>

## Add to resume

Credit card financial dashboard using Power BI: 
<br>
• Developed an interactive dashboard using transaction and 
<br>
customer data from a SQL database, to provide real-time insights.  
<br>
• Streamlined data processing & analysis to monitor 
<br>
key performance metrics and trends. 
<br>
• Shared actionable insights with stakeholders based 
<br>
on dashboard findings to support decision-making 
<br>
processes.


