# Domain 2: Data Processing & Feature Engineering

> Weight 18%

## ML Pipeline Overview

```
Collect → Preprocess → Feature Engineering → Train → Deploy → Monitor
```

## Data Collection & Preprocessing

| Step | Description | Tools |
|------|-------------|-------|
| Collection | Store raw data | S3, AWS Data Exchange |
| Cleaning | Dedup, remove PII | Glue, Macie |
| Labeling | Human annotation | SageMaker Ground Truth |
| Split | Train(80%)/Validation(10%)/Test(10%) | Auto |

### AWS Glue Ecosystem
- **DataBrew**: Visual data prep with reusable "recipes"
- **Data Catalog**: Centralized metadata repository
- **Data Quality**: Anomaly detection & rule recommendations

## Feature Engineering

| Operation | Description |
|-----------|-------------|
| **Selection** | Pick most predictive features |
| **Creation** | Derive new features from existing data |
| **Transformation** | Scaling, encoding, dimensionality reduction |

- **SageMaker Feature Store**: Single source of truth for ML features
- **SageMaker Autopilot**: Automated feature engineering + model tuning

## Vector Databases

| AWS Service | Use |
|-------------|-----|
| **OpenSearch** | k-NN vector search |
| **Aurora/RDS PostgreSQL** + pgvector | Embeddings + similarity search |
| **MemoryDB** | Millisecond vector queries |
| **DocumentDB** | MongoDB-compatible vector search |

## 🔑 Exam Tips
- Know the 8-step ML pipeline
- Glue DataBrew "recipe" concept
- Vector databases store embeddings for similarity search (key for RAG)
