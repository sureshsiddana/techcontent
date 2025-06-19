# Transactions in SQL

A transaction is a sequence of operations performed as a single logical unit of work.

## Key Concepts
- ACID Properties (Atomicity, Consistency, Isolation, Durability)
- BEGIN, COMMIT, ROLLBACK
- Savepoints
- Isolation Levels

## Real-world Project Example
Transferring money between two accounts:
```sql
BEGIN TRANSACTION;
UPDATE Accounts SET Balance = Balance - 100 WHERE AccountID = 1;
UPDATE Accounts SET Balance = Balance + 100 WHERE AccountID = 2;
COMMIT;
```

## More Examples
- Rolling back a transaction on error:
```sql
BEGIN TRANSACTION;
UPDATE Products SET Stock = Stock - 10 WHERE ProductID = 5;
IF @@ERROR <> 0
    ROLLBACK;
ELSE
    COMMIT;
```
- Using savepoints:
```sql
SAVEPOINT before_update;
UPDATE Employees SET Salary = Salary * 1.1;
ROLLBACK TO before_update;
```

## Interview Questions & Answers
**Q1: What is a transaction in SQL?**
A: A group of operations executed as a single unit, ensuring data integrity.

**Q2: What are the ACID properties?**
A: Atomicity, Consistency, Isolation, Durability—guarantee reliable processing of database transactions.

**Q3: How do you handle errors in transactions?**
A: Use ROLLBACK to undo changes if an error occurs.

**Q4: What is an isolation level?**
A: It defines how/when changes made by one operation become visible to others.

## Detailed Explanation
Transactions ensure that either all operations succeed or none do, protecting data integrity. Isolation levels control concurrency and consistency.

## References
- [SQL Transactions - W3Schools](https://www.w3schools.com/sql/sql_transactions.asp)
- [Transactions - SQL Server Docs](https://learn.microsoft.com/en-us/sql/t-sql/language-elements/transactions-transact-sql)
