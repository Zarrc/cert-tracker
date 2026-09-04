# Domain 1: AI/ML Fundamentals

> Weight 20%

## AI/ML Hierarchy

```
General AI → Machine Learning → Deep Learning → Generative AI → LLMs
```

| Level | Description | Examples |
|-------|-------------|----------|
| **General AI** | Systems performing intellectual tasks across domains | Expert systems |
| **Machine Learning** | Learning from data without explicit programming | Linear regression, SVM |
| **Deep Learning** | Multi-layer neural networks for unstructured data | CNN (images), RNN (sequence) |
| **Generative AI** | Creating new content from learned data | ChatGPT, DALL·E |
| **LLMs** | GenAI trained on massive text corpora | GPT-4, BERT, Claude |

## Prompt Engineering
- **Zero-Shot**: No examples given
- **One-Shot**: One example
- **Few-Shot**: Multiple examples
- **Chain-of-Thought (CoT)**: Step-by-step reasoning
- **Prompt Tuning**: Optimizing prompts for specific tasks

## Key Terms
- **Token**: Basic text unit (word/subword/character)
- **Context Window**: Max tokens an LLM can process at once
- **Embeddings**: Numerical vector representations capturing semantics
- **Hallucination**: Model generating plausible but incorrect content
- **Latent Space**: Encoded knowledge/patterns inside LLMs

### Hallucination Mitigations
- **RAG**: Retrieval-Augmented Generation (external grounding)
- **Fine-Tuning**: Training on accurate data
- **HITL**: Human-in-the-loop review

## Inference Parameters (Bedrock)

| Parameter | Effect |
|-----------|--------|
| **Temperature** | Randomness — higher = more creative |
| **Top-K** | Limit to K most probable tokens |
| **Top-P** | Cumulative probability threshold |

## Evaluation Metrics

| Metric | Use |
|--------|-----|
| **ROUGE** | Summarization quality |
| **BLEU** | Translation accuracy (N-gram) |
| **Perplexity** | Prediction quality (lower = better) |
| **Precision/Recall/F1** | Classification |

## 🔑 Exam Tips
- Distinguish AI/ML/DL/GenAI/LLM hierarchy levels
- Know inference parameter effects (Temperature vs Top-K vs Top-P)
- Understand hallucination and its mitigations (RAG, Fine-Tuning, HITL)
