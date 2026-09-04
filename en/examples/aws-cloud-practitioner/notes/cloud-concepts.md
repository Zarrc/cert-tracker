# Domain 1: Cloud Concepts

> Weight 24%

## What is Cloud Computing?

On-demand IT resources, pay-as-you-go pricing.

### Deployment Models
- **Cloud (Public)** — fully on cloud
- **Hybrid** — cloud + on-premises connected
- **On-Premises (Private Cloud)** — self-managed

### Six Advantages (AWS)
1. Variable → fixed expense
2. Economies of scale
3. No capacity guessing
4. Speed & agility
5. No data center costs
6. Global deployment

## AWS Global Infrastructure

| Component | Description |
|-----------|-------------|
| **Region** | Geographic area, ≥3 AZs each |
| **AZ** | 1+ data centers, high bandwidth low latency |
| **Edge Location** | CloudFront cache, 400+ globally |
| **Local Zone** | Compute/storage close to metro users |
| **Wavelength** | AWS embedded in 5G networks |

### Region Selection Factors
- **Compliance** — data sovereignty
- **Latency** — proximity to users
- **Cost** — varies by region
- **Service availability** — new services roll out gradually

## Shared Responsibility Model

```
Customer ("security IN the cloud"):
  - Customer data
  - Platform, apps, IAM
  - OS, network, firewall config
  - Client-side encryption

AWS ("security OF the cloud"):
  - Physical security
  - Hardware, network, infrastructure
  - Managed services (S3, RDS, Lambda)
```

## Well-Architected Framework (6 Pillars)

| Pillar | Focus |
|--------|-------|
| Operational Excellence | Run & monitor, improve processes |
| Security | Protect data & systems |
| Reliability | Recover from failure, scale |
| Performance Efficiency | Efficient resource use |
| Cost Optimization | Avoid unnecessary cost |
| Sustainability | Minimize environmental impact |

## 🔑 Exam Tips
- Distinguish public/hybrid/on-premises
- Know what customer vs AWS is responsible for (shared responsibility)
- Region vs AZ vs Edge Location differences
- Well-Architected 6 pillars
