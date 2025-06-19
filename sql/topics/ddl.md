# Data Definition Language (DDL)

DDL statements are used to define and modify database structures.

## Key Concepts
- CREATE, ALTER, DROP, and TRUNCATE
- Creating and Modifying Tables
- Adding Constraints

## Real-world Project Example
Creating a new table for storing employee data:
```sql
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    Name VARCHAR(100),
    Department VARCHAR(50)
);
```

## Interview Questions & Answers
**Q1: What is DDL?**
A: Data Definition Language, used to define and modify database schema.

**Q2: What is the difference between DROP and TRUNCATE?**
A: DROP removes the table and its data, TRUNCATE removes only the data but keeps the table structure.

**Q3: How do you add a column to an existing table?**
A: Use ALTER TABLE ... ADD COLUMN.

## References
- [SQL DDL - W3Schools](https://www.w3schools.com/sql/sql_ref_ddl.asp)
- [SQL CREATE TABLE - SQL Server Docs](https://learn.microsoft.com/en-us/sql/t-sql/statements/create-table-transact-sql)
