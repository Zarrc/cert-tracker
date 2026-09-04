# Domain 3: Technology

> Weight 34%

## Compute (EC2)

### EC2 Purchase Options
| Option | Description |
|--------|-------------|
| **On-Demand** | Per-second, no commitment |
| **Reserved (RI)** | 1/3 year commitment, Standard/Convertible/Planned |
| **Spot** | Up to 90% discount, can be reclaimed |
| **Dedicated Host** | Physical server exclusively yours |
| **Savings Plan** | $/hr commitment, covers EC2/Fargate/Lambda |

### Security Group vs NACL
| | Security Group | Network ACL |
|---|---------------|-------------|
| Level | Instance | Subnet |
| Rules | Allow only | Allow + Deny |
| State | Stateful | Stateless |
| Default | Deny inbound, allow outbound | Allow all |

### Other Compute
| Service | Use |
|---------|-----|
| **Lambda** | Serverless functions, per-invocation pricing |
| **ECS** | Docker container orchestration |
| **Fargate** | Serverless containers (no EC2 management) |
| **Lightsail** | Simple VPS (beginner-friendly) |

## Storage (S3)

### S3 Storage Classes
| Class | Use Case |
|-------|----------|
| **S3 Standard** | Frequent access |
| **Intelligent-Tiering** | Unknown access patterns |
| **S3 Standard-IA** | Infrequent but fast retrieval |
| **S3 One Zone-IA** | Recreatable data |
| **S3 Glacier** | Archive (minute retrieval) |
| **Glacier Deep Archive** | Long-term archive (12h retrieval) |

### Snow Family
| Device | Capacity |
|--------|----------|
| **Snowcone** | 8-14 TB |
| **Snowball Edge** | 80 TB + compute |
| **Snowmobile** | 100 PB (shipping container) |

## Databases

| Type | AWS Service |
|------|------------|
| **Relational** | RDS (MySQL/PostgreSQL/Oracle/SQL Server), Aurora |
| **NoSQL** | DynamoDB (Key-Value + Document) |
| **Cache** | ElastiCache (Redis/Memcached) |
| **Data Warehouse** | Redshift |

## Networking

| Service | Use |
|---------|-----|
| **VPC** | Virtual private network |
| **Route 53** | DNS + domain registration |
| **CloudFront** | CDN |
| **Direct Connect** | Dedicated line to AWS |

## Monitoring

| Service | Use |
|---------|-----|
| **CloudWatch** | Metrics, logs, alerts, dashboards |
| **CloudTrail** | Account API audit logs |
| **X-Ray** | Distributed request tracing |

## 🔑 Exam Tips
- S3 storage class selection (access frequency vs cost)
- EC2 purchase options (On-Demand vs RI vs Spot vs Savings Plan)
- Security Group (stateful) vs NACL (stateless)
- CloudWatch (monitoring) vs CloudTrail (audit)
- Horizontal vs vertical scaling
