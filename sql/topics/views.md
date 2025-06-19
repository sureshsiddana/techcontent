# Views in SQL

A view is a virtual table based on the result of a SQL query.

## Key Concepts
- Creating and Using Views
- Updatable vs. Non-Updatable Views
- Security and Abstraction

## Real-world Project Example
Creating a view to show active customers:
```sql
CREATE VIEW ActiveCustomers AS
SELECT * FROM Customers WHERE Status = 'Active';
```

## More Examples
- View joining multiple tables:
```sql
CREATE VIEW CustomerOrders AS
SELECT c.Name, o.OrderID, o.Total
FROM Customers c
JOIN Orders o ON c.CustomerID = o.CustomerID;
```
- Using a view for reporting:
```sql
SELECT * FROM CustomerOrders WHERE Total > 1000;
```

## Interview Questions & Answers
**Q1: What is a view in SQL?**
A: A virtual table based on a SELECT query, used for abstraction and security.

**Q2: Can you update data through a view?**
A: Yes, if the view is updatable and not based on joins or aggregations.

**Q3: What are the benefits of using views?**
A: Simplifies complex queries, enhances security, and provides a consistent interface.

**Q4: How do you refresh a view?**
A: In most databases, views are updated automatically; materialized views require manual refresh.

## Detailed Explanation
Views help encapsulate complex queries and restrict access to sensitive data. They do not store data themselves but present data dynamically from underlying tables.

## References
- [SQL Views - W3Schools](https://www.w3schools.com/sql/sql_view.asp)
- [Views - SQL Server Docs](https://learn.microsoft.com/en-us/sql/relational-databases/views/views)
