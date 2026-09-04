# CLF-C02 Practice Questions

> Organized by domain. Format: `[Type] Question | Options | Answer: X | Domain: XXX`

---

## Domain 1: Cloud Concepts

[MC] What is the primary benefit of the AWS shared responsibility model? | A) AWS is responsible for everything B) Customer is responsible for everything C) AWS handles infrastructure security, customer handles data/OS D) Responsibility is shared equally for all services | Answer: C | Domain: Cloud Concepts
[MC] How many Availability Zones does an AWS Region typically have? | A) 1 B) 2 C) At least 3 D) 5 | Answer: C | Domain: Cloud Concepts
[TF] Hybrid cloud refers to connecting multiple public cloud providers together. | Answer: False | Domain: Cloud Concepts
[MC] Which of the following is NOT one of the 6 pillars of the Well-Architected Framework? | A) Security B) Cost Optimization C) Agility D) Sustainability | Answer: C | Domain: Cloud Concepts
[MC] Which factor is LEAST important when choosing an AWS Region? | A) Compliance B) Latency C) Service availability D) Company logo color | Answer: D | Domain: Cloud Concepts

## Domain 2: Security & Compliance

[MC] Which AWS service records all API calls for audit purposes? | A) CloudWatch B) CloudTrail C) Config D) VPC Flow Logs | Answer: B | Domain: Security & Compliance
[MC] What is the difference between Security Groups and Network ACLs? | A) SGs are stateless, NACLs are stateful B) SGs are stateful, NACLs are stateless C) Both are stateful D) Both are stateless | Answer: B | Domain: Security & Compliance
[TF] IAM Roles are primarily used for individual user accounts. | Answer: False | Domain: Security & Compliance
[MC] Which service detects sensitive data like PII in S3? | A) GuardDuty B) Inspector C) Macie D) Shield | Answer: C | Domain: Security & Compliance
[MC] AWS Shield Advanced protects against what type of attack? | A) SQL injection B) DDoS C) Brute force D) XSS | Answer: B | Domain: Security & Compliance

## Domain 3: Technology

[MC] Which EC2 purchase option offers up to 90% discount but instances can be reclaimed? | A) On-Demand B) Reserved C) Spot D) Dedicated Host | Answer: C | Domain: Technology
[MC] Which S3 storage class is best for long-term archival with 12-hour retrieval? | A) S3 Standard B) S3 Standard-IA C) S3 Glacier D) S3 Glacier Deep Archive | Answer: D | Domain: Technology
[MC] Which AWS service is a NoSQL database? | A) RDS B) Aurora C) DynamoDB D) Redshift | Answer: C | Domain: Technology
[MC] What is the main advantage of AWS Lambda? | A) Supports all languages B) No server management C) Built-in database D) Always free | Answer: B | Domain: Technology
[TF] CloudFront is a content delivery network (CDN) service. | Answer: True | Domain: Technology

## Domain 4: Billing & Pricing

[MC] Is data transfer from AWS to the internet (outbound) charged? | A) Free B) Per GB C) Only for EC2 D) Free for first 10GB | Answer: B | Domain: Billing & Pricing
[MC] Which AWS Support Plan provides a 15-minute response time and dedicated TAM? | A) Basic B) Developer C) Business D) Enterprise | Answer: D | Domain: Billing & Pricing
[TF] Consolidated Billing allows combining usage across accounts for volume discounts. | Answer: True | Domain: Billing & Pricing
[MC] How many Trusted Advisor checks are available in the Basic Support Plan? | A) 0 B) 7 C) All D) 50 | Answer: B | Domain: Billing & Pricing
[SA] Which tool visualizes and forecasts AWS costs? | Answer: Cost Explorer | Domain: Billing & Pricing

---

**Stats**: MC `16` · TF `3` · SA `1` · Total **20**
