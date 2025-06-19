# AWS RDS (Relational Database Service)

## Key Concepts
- **Managed Database:** RDS automates database setup, patching, backups, and scaling.
- **Supported Engines:** MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, and Amazon Aurora.
- **High Availability:** Multi-AZ deployments for failover and durability.
- **Read Replicas:** Improve performance and scalability for read-heavy workloads.
- **Security:** Encryption at rest/in transit, VPC isolation, IAM authentication.
- **Backups & Snapshots:** Automated backups and manual snapshots for disaster recovery.

## Real-World Example
- **Web Application Backend:** Use RDS for transactional data storage in scalable web apps.
- **Analytics:** Offload reporting to read replicas to reduce load on primary DB.

## Interview Q&A
**Q: What is AWS RDS?**
A: RDS is a managed relational database service that simplifies database administration tasks.

**Q: How does RDS provide high availability?**
A: Through Multi-AZ deployments, automated failover, and backups.

**Q: How can you secure an RDS instance?**
A: Use VPC, security groups, encryption, and IAM authentication.

## References
- [AWS RDS Documentation](https://docs.aws.amazon.com/rds/index.html)
- [RDS Best Practices](https://aws.amazon.com/rds/details/)

## Relevant Image
![AWS RDS Overview](https://d1.awsstatic.com/diagrams/product-page-diagrams/Amazon-RDS@2x.7d7e6b7e2b2e2e7e2e7e2e7e2e7e2e7e.png)
