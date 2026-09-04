# Domain 2: Security & Compliance

> Weight 30%

## IAM (Identity & Access Management)

### Core Components
| Component | Description |
|-----------|-------------|
| **User** | Real person |
| **Group** | User collection, inherits permissions |
| **Role** | For AWS services or temporary access |
| **Policy** | JSON permission document |

### Three Ways to Access AWS
- **Console** — Web UI (password + MFA)
- **CLI** — Command line (Access Key)
- **SDK** — Code (Access Key)

## Security Services Quick Reference

### Protection
| Service | Use |
|---------|-----|
| **WAF** | Web application firewall (SQL injection, XSS) |
| **Shield** | DDoS protection (Standard free, Advanced paid) |
| **GuardDuty** | Threat detection (intelligent anomaly monitoring) |
| **Inspector** | Vulnerability scanner (EC2, containers) |
| **Macie** | Sensitive data discovery (PII in S3) |
| **Security Hub** | Centralized security state management |

### Encryption
| Service | Use |
|---------|-----|
| **KMS** | Key creation & management |
| **CloudHSM** | Dedicated hardware security module |
| **ACM** | SSL/TLS certificate management |
| **Secrets Manager** | Secret/API token rotation |

### Compliance
| Service | Use |
|---------|-----|
| **Artifact** | Self-service compliance reports (SOC, PCI, ISO) |
| **Config** | Resource configuration audit |
| **CloudTrail** | Account API call logs (audit) |

## Shared Responsibility by Service Type

| | Customer | AWS |
|---|----------|-----|
| **EC2 (IaaS)** | OS, security groups, patches, apps | Physical hardware, network |
| **RDS (PaaS)** | Data, access permissions | OS, patches, backup, failover |
| **S3 (SaaS)** | Data, permission settings | Infrastructure, durability |

## 🔑 Exam Tips
- IAM 4 components (User/Group/Role/Policy)
- CloudTrail (API logs) vs CloudWatch (metrics) vs Config (audit)
- GuardDuty (threats) vs Inspector (vulnerabilities) vs Macie (sensitive data)
- Different services = different customer responsibility scope
