# AWS Lambda

## Key Concepts
- **Serverless Compute:** Run code without provisioning or managing servers.
- **Event-Driven:** Trigger functions in response to events (S3, API Gateway, DynamoDB, etc.).
- **Stateless Functions:** Each invocation is independent.
- **Resource Allocation:** Configure memory, timeout, and environment variables.
- **Concurrency:** Supports scaling automatically with demand.
- **Integrations:** Works with many AWS services and custom events.

## Real-World Example
- **Image Processing:** Automatically resize images uploaded to S3.
- **API Backend:** Build RESTful APIs using Lambda and API Gateway.

## Interview Q&A
**Q: What is AWS Lambda?**
A: Lambda is a serverless compute service that runs code in response to events and automatically manages the compute resources.

**Q: How is Lambda billed?**
A: You pay only for the compute time you consume (number of requests and duration).

**Q: How do you secure Lambda functions?**
A: Use IAM roles, environment variable encryption, and VPC integration for private resources.

## References
- [AWS Lambda Documentation](https://docs.aws.amazon.com/lambda/index.html)
- [Serverless Architectures](https://aws.amazon.com/serverless/)

## Relevant Image
![AWS Lambda Overview](https://d1.awsstatic.com/diagrams/product-page-diagrams/AWS-Lambda@2x.7d7e6b7e2b2e2e7e2e7e2e7e2e7e2e7e.png)
