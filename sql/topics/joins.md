# Joins in SQL

Joins are used to combine rows from two or more tables based on related columns.

## Key Concepts
- INNER JOIN
- LEFT (OUTER) JOIN
- RIGHT (OUTER) JOIN
- FULL (OUTER) JOIN
- CROSS JOIN

## Real-world Project Example
Getting a list of customers and their orders:
```sql
SELECT Customers.Name, Orders.OrderID
FROM Customers
INNER JOIN Orders ON Customers.CustomerID = Orders.CustomerID;
```

## Interview Questions & Answers
**Q1: What is an INNER JOIN?**
A: Returns rows when there is a match in both tables.

**Q2: What is the difference between LEFT JOIN and RIGHT JOIN?**
A: LEFT JOIN returns all rows from the left table and matched rows from the right; RIGHT JOIN does the opposite.

**Q3: When would you use a FULL OUTER JOIN?**
A: To return all rows when there is a match in one of the tables.

## References
- [SQL Joins - W3Schools](https://www.w3schools.com/sql/sql_join.asp)
- [SQL JOIN - SQL Server Docs](https://learn.microsoft.com/en-us/sql/t-sql/queries/select-joins-transact-sql)
