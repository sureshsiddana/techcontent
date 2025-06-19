# Constraints in SQL

Constraints are rules enforced on data columns to ensure data integrity.

## Key Concepts
- Primary Key, Foreign Key
- Unique, Not Null, Check, Default
- Adding and Dropping Constraints

## Real-world Project Example
Enforcing unique email addresses for users:
```sql
ALTER TABLE Users ADD CONSTRAINT UQ_Email UNIQUE (Email);
```

## More Examples
- Foreign key constraint:
```sql
ALTER TABLE Orders ADD CONSTRAINT FK_Customer FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID);
```
- Check constraint:
```sql
ALTER TABLE Employees ADD CONSTRAINT CK_Salary CHECK (Salary > 0);
```

## Interview Questions & Answers
**Q1: What is a primary key?**
A: A column or set of columns that uniquely identifies each row in a table.

**Q2: What is a foreign key?**
A: A column that creates a relationship between two tables.

**Q3: What is the purpose of a check constraint?**
A: To enforce domain integrity by limiting the values that can be placed in a column.

**Q4: Can a table have multiple unique constraints?**
A: Yes, a table can have multiple unique constraints on different columns.

## Detailed Explanation
Constraints are essential for maintaining data quality and enforcing business rules at the database level.

## References
- [SQL Constraints - W3Schools](https://www.w3schools.com/sql/sql_constraints.asp)
- [Constraints - SQL Server Docs](https://learn.microsoft.com/en-us/sql/relational-databases/tables/table-constraints)
