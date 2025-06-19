# SQL Performance Tuning

## Key Concepts
- Performance tuning involves optimizing SQL queries and database design for speed and efficiency.
- Key areas: indexing, query optimization, normalization/denormalization, hardware resources, and database configuration.
- Use EXPLAIN plans to analyze query performance.

## Real-World Examples

### Example 1: Using Indexes
```sql
CREATE INDEX idx_employee_name ON employees(name);
SELECT * FROM employees WHERE name = 'John Doe';
```

### Example 2: Avoiding SELECT *
```sql
-- Bad:
SELECT * FROM orders;
-- Good:
SELECT order_id, order_date, amount FROM orders;
```

### Example 3: Query Refactoring
```sql
-- Inefficient:
SELECT * FROM sales WHERE YEAR(order_date) = 2024;
-- Efficient (if order_date is indexed):
SELECT * FROM sales WHERE order_date >= '2024-01-01' AND order_date < '2025-01-01';
```

### Example 4: Using EXPLAIN
```sql
EXPLAIN SELECT * FROM employees WHERE department_id = 10;
```

## Interview Questions & Answers

**Q1: What are some common causes of slow SQL queries?**
A: Missing indexes, inefficient joins, large result sets, poor query structure, and hardware limitations.

**Q2: How can you identify a slow query?**
A: Use tools like `EXPLAIN`, query profiling, and monitoring slow query logs.

**Q3: Real-time: A report query is taking too long. What steps do you take to troubleshoot?**
A: 1) Analyze the query with EXPLAIN, 2) Check for missing indexes, 3) Refactor the query, 4) Review database configuration, 5) Consider denormalization if appropriate.

**Q4: Real-time: How do you optimize a query that uses multiple joins?**
A: Ensure proper indexes on join columns, avoid unnecessary columns, filter early, and review join order.

**Q5: What is the impact of indexing on write operations?**
A: Indexes speed up reads but can slow down writes (INSERT, UPDATE, DELETE) due to index maintenance overhead.

## References
- [SQL Performance Tuning - Mode](https://mode.com/sql-tutorial/sql-performance-tuning/)
- [SQL Server Docs: Query Tuning](https://docs.microsoft.com/en-us/sql/relational-databases/performance/performance-tuning-sql-queries)
- [PostgreSQL Docs: Performance Tips](https://www.postgresql.org/docs/current/performance-tips.html)
