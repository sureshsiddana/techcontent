# Data Query Language (DQL)

DQL is used to query information from the database.

## Key Concepts
- SELECT Statement
- Filtering, Sorting, and Limiting Results
- Aggregate Functions (COUNT, SUM, AVG, MIN, MAX)
- GROUP BY and HAVING

## Real-world Project Example
Finding the total sales for each product:
```sql
SELECT ProductID, SUM(Sales) AS TotalSales
FROM Orders
GROUP BY ProductID;
```

## Interview Questions & Answers
**Q1: What is DQL?**
A: Data Query Language, primarily the SELECT statement for querying data.

**Q2: How do you group results in SQL?**
A: Use GROUP BY to aggregate data by one or more columns.

**Q3: What is the difference between WHERE and HAVING?**
A: WHERE filters rows before grouping, HAVING filters groups after aggregation.

## References
- [SQL SELECT - W3Schools](https://www.w3schools.com/sql/sql_select.asp)
- [SQL GROUP BY - SQL Server Docs](https://learn.microsoft.com/en-us/sql/t-sql/queries/select-group-by-transact-sql)
