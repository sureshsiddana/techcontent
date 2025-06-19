# Window Functions in SQL

## Key Concepts
- Window functions perform calculations across a set of table rows related to the current row.
- Unlike aggregate functions, window functions do not collapse rows.
- Common window functions: `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, `NTILE()`, `LEAD()`, `LAG()`, `SUM() OVER`, `AVG() OVER`.
- Syntax: `function_name() OVER (PARTITION BY ... ORDER BY ...)`

## Real-World Examples

### Example 1: Ranking Employees by Salary
```sql
SELECT employee_id, department_id, salary,
       RANK() OVER (PARTITION BY department_id ORDER BY salary DESC) AS dept_salary_rank
FROM employees;
```

### Example 2: Calculating Running Total
```sql
SELECT order_id, order_date, amount,
       SUM(amount) OVER (ORDER BY order_date) AS running_total
FROM orders;
```

### Example 3: Comparing Current Row to Previous Row
```sql
SELECT order_id, order_date, amount,
       LAG(amount, 1) OVER (ORDER BY order_date) AS prev_amount
FROM orders;
```

### Example 4: Percentile Distribution
```sql
SELECT student_id, score,
       NTILE(4) OVER (ORDER BY score DESC) AS quartile
FROM exam_results;
```

## Interview Questions & Answers

**Q1: What is the difference between window functions and aggregate functions?**
A: Aggregate functions return a single value for a group of rows, collapsing them into one. Window functions perform calculations across a set of rows related to the current row, but do not collapse the result set.

**Q2: How would you calculate a running total in SQL?**
A: Use `SUM(column) OVER (ORDER BY ...)` to calculate a running total. Example:
```sql
SELECT order_id, amount, SUM(amount) OVER (ORDER BY order_id) AS running_total FROM orders;
```

**Q3: Explain the use of LAG and LEAD functions.**
A: `LAG` returns data from a previous row, while `LEAD` returns data from a following row, both based on the specified order. Useful for comparing current row values to previous or next rows.

**Q4: Real-time: You need to find the top 3 sales per region, but also show all sales. How would you do this?**
A: Use `RANK()` or `ROW_NUMBER()` window function partitioned by region and filter in an outer query:
```sql
SELECT * FROM (
  SELECT sale_id, region, amount,
         ROW_NUMBER() OVER (PARTITION BY region ORDER BY amount DESC) AS rn
  FROM sales
) t WHERE rn <= 3;
```

**Q5: Real-time: How can you compare each month's sales to the previous month's sales in a single query?**
A: Use `LAG()` to access the previous month's sales:
```sql
SELECT month, sales,
       LAG(sales, 1) OVER (ORDER BY month) AS prev_month_sales,
       sales - LAG(sales, 1) OVER (ORDER BY month) AS sales_diff
FROM monthly_sales;
```

## References
- [SQL Window Functions - Mode](https://mode.com/sql-tutorial/sql-window-functions/)
- [PostgreSQL Docs: Window Functions](https://www.postgresql.org/docs/current/tutorial-window.html)
- [SQL Server Docs: Window Functions](https://docs.microsoft.com/en-us/sql/t-sql/queries/select-over-clause-transact-sql)
