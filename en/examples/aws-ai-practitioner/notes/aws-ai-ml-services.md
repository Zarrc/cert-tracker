# Domain 4: AWS AI/ML Services

> Weight 28%

## Amazon Bedrock (Key Service)

Fully managed, serverless — single API for multiple Foundation Models.

### Supported Models
AI21 Labs · Anthropic · Cohere · Meta · Mistral AI · Stability AI · **Amazon Titan**

### Bedrock Features
| Feature | Description |
|---------|-------------|
| **Knowledge Bases** | RAG from private data |
| **Agents** | Multi-step planning + tools |
| **Guardrails** | Restrict inappropriate content |
| **PartyRock** | No-code GenAI playground |
| **Model Evaluation** | Compare FMs on metrics |

## Amazon SageMaker (Full ML Platform)

| Component | Use |
|-----------|-----|
| **Studio** | IDE with notebooks, debugging |
| **Feature Store** | Central ML feature repository |
| **Model Registry** | Version management |
| **Pipelines** | Workflow orchestration |
| **Model Monitor** | Drift detection |
| **Ground Truth** | Human data labeling |
| **Clarify** | Bias detection + explainability |
| **Autopilot** | Automated model building |
| **Canvas** | No-code modeling |
| **JumpStart** | Pre-trained model hub |

## Managed AI Services

### Vision
| Service | Use |
|---------|-----|
| **Rekognition** | Face analysis, object detection |
| **Textract** | OCR from documents |

### Language
| Service | Use |
|---------|-----|
| **Comprehend** | NLP — sentiment, entities, PII |
| **Translate** | Translation |
| **Transcribe** | Speech-to-text |
| **Polly** | Text-to-speech |
| **Lex** | Chatbot (Alexa tech) |

### Search & Recommendations
| Service | Use |
|---------|-----|
| **Kendra** | Intelligent document search |
| **Personalize** | Recommendations |
| **Forecast** | Time-series prediction |

### Hallucination Mitigation
| Method | Description |
|--------|-------------|
| **RAG** | Retrieve external data to ground responses |
| **Fine-Tuning** | Train on accurate domain data |
| **Human-in-the-Loop** | Human review for low-confidence |

## 🔑 Exam Tips
- Bedrock (FM service) vs SageMaker (full ML platform)
- Scenario matching: given a problem → pick right AWS service
- RAG concept and how it reduces hallucination
- Amazon Titan = AWS's own FM, exclusive to Bedrock
