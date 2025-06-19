# SQL Interview Questions

## Key Concepts
- SQL interviews test knowledge of database concepts, query writing, optimization, and real-world problem solving.
- Questions range from basic syntax to advanced performance and security topics.

## Real-World Examples & Questions

### Example 1: Write a query to find the second highest salary from an employee table.
```sql
SELECT MAX(salary) AS second_highest_salary
FROM employees
WHERE salary < (SELECT MAX(salary) FROM employees);
```

### Example 2: Find duplicate records in a table.
```sql
SELECT column1, COUNT(*)
FROM table_name
GROUP BY column1
HAVING COUNT(*) > 1;
```

### Example 3: Retrieve departments with more than 5 employees.
```sql
SELECT department_id, COUNT(*) AS num_employees
FROM employees
GROUP BY department_id
HAVING COUNT(*) > 5;
```

### Example 4: Real-time: How would you design a database for an e-commerce platform?
A: Identify entities (users, products, orders), define relationships, normalize tables, ensure indexing, and plan for scalability and security.

### Example 5: Real-time: How do you troubleshoot a slow-running query in production?
A: 1) Analyze the query plan, 2) Check for missing indexes, 3) Refactor the query, 4) Monitor resource usage, 5) Collaborate with DBAs.

## Interview Q&A with Explanations

**Q1: What is normalization? Why is it important?**
A: Normalization organizes data to reduce redundancy and improve integrity. It ensures efficient storage and consistency.

**Q2: Explain the difference between INNER JOIN and LEFT JOIN.**
A: INNER JOIN returns only matching rows; LEFT JOIN returns all rows from the left table and matching rows from the right, with NULLs for non-matches.

**Q3: What is a transaction?**
A: A transaction is a sequence of operations performed as a single logical unit, ensuring ACID properties (Atomicity, Consistency, Isolation, Durability).

**Q4: Real-time: How would you implement audit logging in SQL?**
A: Use triggers or built-in auditing features to log changes to a separate audit table.

**Q5: Real-time: How do you handle schema changes in a live production database?**
A: Plan changes, test in staging, use migrations, communicate with stakeholders, and monitor after deployment.

## References
- [SQL Interview Questions - LeetCode](https://leetcode.com/problemset/database/)
- [SQL Interview Questions - GeeksforGeeks](https://www.geeksforgeeks.org/sql-interview-questions/)
- [SQL Server Docs: Interview Preparation](https://docs.microsoft.com/en-us/sql/)
