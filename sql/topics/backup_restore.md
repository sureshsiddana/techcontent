# SQL Backup and Restore

## Key Concepts
- Backup and restore are essential for data protection and disaster recovery.
- Types of backups: full, differential, incremental, and transaction log backups.
- Restore operations recover data from backups.

## Real-World Examples

### Example 1: Full Database Backup
```sql
-- SQL Server
BACKUP DATABASE mydb TO DISK = 'C:\backup\mydb_full.bak';
```

### Example 2: Restoring a Database
```sql
-- SQL Server
RESTORE DATABASE mydb FROM DISK = 'C:\backup\mydb_full.bak';
```

### Example 3: MySQL Backup and Restore
```bash
# Backup
mysqldump -u root -p mydb > mydb_backup.sql
# Restore
mysql -u root -p mydb < mydb_backup.sql
```

### Example 4: PostgreSQL Backup and Restore
```bash
# Backup
pg_dump mydb > mydb_backup.sql
# Restore
psql mydb < mydb_backup.sql
```

## Interview Questions & Answers

**Q1: What are the different types of backups in SQL?**
A: Full, differential, incremental, and transaction log backups.

**Q2: How do you restore a database to a specific point in time?**
A: Use transaction log backups and specify the recovery point during the restore process.

**Q3: Real-time: A production database is corrupted. What steps do you take to restore service?**
A: 1) Assess the extent of corruption, 2) Restore the latest full backup, 3) Apply differential/incremental and transaction log backups, 4) Validate data integrity, 5) Communicate with stakeholders.

**Q4: Real-time: How do you automate regular backups?**
A: Use database maintenance plans, scheduled jobs, or scripts to automate backups and monitor their success.

**Q5: How do you verify the integrity of a backup?**
A: Use database tools to test restore operations and validate backup files.

## References
- [SQL Backup and Restore - W3Schools](https://www.w3schools.com/sql/sql_backup.asp)
- [SQL Server Docs: Backup and Restore](https://docs.microsoft.com/en-us/sql/relational-databases/backup-restore/)
- [PostgreSQL Docs: Backup and Restore](https://www.postgresql.org/docs/current/backup.html)
