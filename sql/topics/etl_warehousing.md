# ETL and Data Warehousing in SQL

## Key Concepts
- ETL stands for Extract, Transform, Load: the process of moving and transforming data from source to destination.
- Data warehousing involves storing large volumes of data for analysis and reporting.
- SQL is used for data extraction, transformation, loading, and querying in data warehouses.

## Real-World Examples

### Example 1: Extracting Data
```sql
SELECT * FROM sales WHERE sale_date >= '2024-01-01';
```

### Example 2: Transforming Data
```sql
SELECT customer_id, UPPER(name) AS name_upper, amount * 1.1 AS adjusted_amount
FROM sales;
```

### Example 3: Loading Data
```sql
INSERT INTO warehouse.sales_summary (customer_id, total_amount)
SELECT customer_id, SUM(amount) FROM sales GROUP BY customer_id;
```

### Example 4: Star Schema Example
- Fact table: `sales`
- Dimension tables: `customers`, `products`, `time`

```sql
SELECT c.name, p.product_name, t.year, SUM(s.amount) AS total_sales
FROM sales s
JOIN customers c ON s.customer_id = c.id
JOIN products p ON s.product_id = p.id
JOIN time t ON s.time_id = t.id
GROUP BY c.name, p.product_name, t.year;
```

## Interview Questions & Answers

**Q1: What is ETL and why is it important?**
A: ETL (Extract, Transform, Load) is the process of moving and transforming data for analysis. It's crucial for integrating data from multiple sources into a data warehouse.

**Q2: What is a star schema?**
A: A star schema is a data warehouse design with a central fact table connected to dimension tables, optimizing query performance and simplicity.

**Q3: Real-time: How would you handle slowly changing dimensions in a data warehouse?**
A: Use techniques like Type 1 (overwrite), Type 2 (add new row with versioning), or Type 3 (add new column for previous value) to manage changes in dimension data.

**Q4: Real-time: How do you optimize ETL processes for large datasets?**
A: Use bulk operations, parallel processing, incremental loads, and proper indexing. Monitor and tune performance regularly.

**Q5: What SQL features are commonly used in ETL?**
A: Joins, aggregations, window functions, CTEs, and bulk insert operations.

## References
- [ETL Concepts - W3Schools](https://www.w3schools.com/whatis/whatis_etl.asp)
- [Data Warehousing - Mode](https://mode.com/sql-tutorial/sql-data-warehousing/)
- [SQL Server Docs: Data Warehousing](https://docs.microsoft.com/en-us/sql/relational-databases/data-warehousing/)
