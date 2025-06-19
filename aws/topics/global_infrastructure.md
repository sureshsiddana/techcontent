# AWS Global Infrastructure

## Key Concepts
- AWS operates in multiple geographic regions, each with multiple Availability Zones (AZs).
- Edge locations provide low-latency content delivery (CloudFront).
- Global infrastructure ensures high availability, disaster recovery, and compliance.

## Real-World Examples

### Example 1: Multi-Region Deployment
- Deploying applications in multiple regions for disaster recovery and global reach.

### Example 2: Content Delivery
- Use CloudFront edge locations to serve static assets closer to users.

### Example 3: Compliance
- Choose regions to meet data residency and compliance requirements.

## Interview Questions & Answers

**Q1: What is an AWS Region?**
A: A physical location with multiple isolated Availability Zones.

**Q2: Real-time: How do you design for high availability in AWS?**
A: Deploy resources across multiple AZs and regions.

**Q3: What are edge locations?**
A: Data centers for caching content and reducing latency (used by CloudFront).

## References
- [AWS Global Infrastructure](https://aws.amazon.com/about-aws/global-infrastructure/)
- [CloudFront Edge Locations](https://aws.amazon.com/cloudfront/features/)

![AWS Global Map](https://d1.awsstatic.com/global-infrastructure/Global-Infrastructure-Map.6d7b6e7b8e4b4e6b8e4b4e6b8e4b4e6b8e4b4e6b.png)
*Image Source: AWS*
