# Sales Insights Power BI Project
### Data Analysis using SQL
1. Show all customer records

      `SELECT * FROM customers;`

2. Show total number of customers

     `SELECT COUNT(*) FROM customers;`
     
3.  Show the records of market

      `SELECT * FROM markets;`
      
4. Show trasactions from Chennai market ( market code for chennai is Mark001 )

      `SELECT * FROM transactions WHERE market_code='Mark001';`
      
5. Show distinct product codes that were sold in chennai
 
      `SELECT DISTINCT product_code FROM transactions WHERE market_code='Mark001';`
      
6. Show transactions where currency is US dollars

      `SELECT * FROM transactions WHERE currency='USD';`
      
7.  Show total revenue in year 2020 in Chennai
       
        `SELECT SUM(transactions.sales_amount) FROM transactions INNER JOIN date ON transactions.order_date=date.date WHERE date.year=2020
         and transactions.market_code="Mark001";`
         

## Power BI dashboard







