# Domain 3: Model Training & Deployment

> Weight 26%

## Training Hyperparameters

| Parameter | Description |
|-----------|-------------|
| **Epoch** | Full pass through the dataset |
| **Batch Size** | Samples per parameter update |
| **Learning Rate** | Training speed control |

## Common Training Issues

| Issue | Symptom | Solution |
|-------|---------|----------|
| **Overfitting** | Good on train, bad on test | More diverse data, regularization |
| **Underfitting** | Bad on both train and test | More epochs, complex model |
| **Bias/Fairness** | Model has prejudice | Diverse representative data |

## Fine-Tuning Approaches

| Method | Description | Risk |
|--------|-------------|------|
| **Fine-Tuning** | Adjust pre-trained weights with labeled data | Catastrophic Forgetting |
| **Domain Adaptation** | Tailor to specific domain (legal/medical) | — |
| **Transfer Learning** | Transfer general features to new problems | — |

## Deployment Options

### SageMaker Inference
| Mode | Best For |
|------|----------|
| **Real-Time** | Low latency, sustained traffic, auto-scaling |
| **Batch Transform** | Large async data batches |
| **Asynchronous** | Long-running, large payloads |
| **Serverless** | Intermittent traffic, auto scaling |

### Bedrock
| Mode | Use Case |
|------|----------|
| **On-Demand** | Pay per token, low/sporadic usage |
| **Provisioned Throughput** | Reserved capacity for fine-tuned models |
| **Agents** | Multi-step workflows + tools |

## Monitoring

| Type | Description |
|------|-------------|
| **Data Drift** | Input distribution changes |
| **Concept Drift** | Input-output relationship changes |
| **Tool** | SageMaker Model Monitor + CloudWatch |

## 🔑 Exam Tips
- Overfitting vs Underfitting and solutions
- SageMaker 4 inference modes
- Fine-Tuning vs RAG (when to use which)
- Data Drift vs Concept Drift distinction
