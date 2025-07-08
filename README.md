# SQL--Superstores
SQL queries for top customers and sales trends

Top 5 customers by total sale
--select top 5 customers with top sales
SELECT "Customer Name", sum(Sales) AS TotalSales, COUNT(DISTINCT "Order ID") AS Order_Count FROM Superstores GROUP by "Customer Name" ORDER by TotalSales DESC LIMIT 5;
