# Domain 4: Billing & Pricing

> Weight 12%

## AWS Pricing Model

### Compute Pricing
- **EC2**: Per-second (instance type + region + purchase option)
- **Lambda**: Per invocation + execution time

### Storage Pricing
- **S3**: Per GB/month + requests + data transfer
- **EBS**: Per provisioned GB/month

### Data Transfer
- **Inbound** (to AWS): Free
- **Outbound** (from AWS): Per GB
- **Same region** (private IP): Free

## AWS Organizations

| Feature | Description |
|---------|-------------|
| **Consolidated Billing** | Single bill for all accounts |
| **SCP** | Organization-level permission boundaries |
| **OU** | Organizational units (hierarchical) |

## Billing Tools

| Tool | Use |
|------|-----|
| **Cost Explorer** | Visualize & forecast costs |
| **Budgets** | Set budgets & alerts |
| **Pricing Calculator** | Estimate service costs |
| **Cost & Usage Report** | Detailed cost/usage data |

## Support Plans

| Plan | Price | Key Feature |
|------|-------|-------------|
| **Basic** | Free | Docs + health dashboard |
| **Developer** | Usage-based | Business-hours email |
| **Business** | Usage-based | 1h response + architecture guidance |
| **Enterprise** | Fixed | 15min response + dedicated TAM |

## Trusted Advisor Categories

| Category | Checks |
|----------|--------|
| **Cost Optimization** | Idle instances, RI optimization |
| **Performance** | EC2 config, EBS throughput |
| **Security** | S3 public access, security group rules |
| **Fault Tolerance** | Multi-AZ, RDS backup |
| **Service Limits** | Usage limits |

> Basic plan: 7 core checks only. Business/Enterprise: full access.

## 🔑 Exam Tips
- Inbound to AWS free, outbound charged
- Cost Explorer (analysis) vs Budgets (alerts)
- Support Plan response times & TAM
- Trusted Advisor 5 categories
- Organizations + Consolidated Billing benefits
