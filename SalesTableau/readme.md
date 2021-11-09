# Portfolio Project 2
## Sales_Tableau

### **Shows record of Market** 
![sales of Atliq 1](https://user-images.githubusercontent.com/93612190/140888359-dd88a46c-1487-4e38-aeff-c0ea779fa770.png)

### **Record of Transactions**
![sales of Atliq 2](https://user-images.githubusercontent.com/93612190/140888705-7fdd2cba-e936-4f58-8997-074f53ec56dd.png)


### **Joined Tables usig Inner Join**
![sales of Atliq 3](https://user-images.githubusercontent.com/93612190/140891054-c60e05f8-131b-44df-9e99-5a81bf69b697.png)

## Data Analysis Using SQL

Show all customer records

`SELECT * FROM customers;`

Show total number of customers

`SELECT count(*) FROM customers;`

Show transactions for Chennai market (market code for chennai is Mark001

`SELECT * FROM transactions where market_code='Mark001';`

Show distrinct product codes that were sold in chennai

`SELECT distinct product_code FROM transactions where market_code='Mark001';`

Show transactions where currency is US dollars

`SELECT * from transactions where currency="USD"`

Show transactions in 2020 join by date table

`SELECT transactions.*, date.* FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020;`

Show total revenue in year 2020,

`SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.currency="INR\r" or transactions.currency="USD\r";`

Show total revenue in year 2020, January Month,

`SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and and date.month_name="January" and (transactions.currency="INR\r" or transactions.currency="USD\r");`

Show total revenue in year 2020 in Chennai

`SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date where date.year=2020 and transactions.market_code="Mark001";`


## Data Analysis Using Tableau 19.4

### **Data Model**
![data model tableau](https://user-images.githubusercontent.com/93612190/140980797-367c70bb-5917-436a-a1d2-ce26b1c201cf.png)

### **Top Customers**
![worksheet customer](https://user-images.githubusercontent.com/93612190/140981633-ed4bfde9-9789-4998-8d6e-ac35caac17e4.png)


### **Revenue by Market**
![Revenue by market](https://user-images.githubusercontent.com/93612190/140981778-7e862371-4957-471b-af72-f6a81d1cd899.png)


 ### **Final Dashboard**
![Dashboard tableau](https://user-images.githubusercontent.com/93612190/140981940-d3b580b7-12ba-40b3-923a-34d6c5b4c0bd.png)
 












