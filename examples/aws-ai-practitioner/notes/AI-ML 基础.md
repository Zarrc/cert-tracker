# Domain 1: AI/ML 基础

> 权重 20% · 对应资源：freeCodeCamp 15h 课程 (00:17:48)

---

## AI/ML 层级结构

```
General AI → Machine Learning → Deep Learning → Generative AI → LLMs
```

| 层级 | 说明 | 例子 |
|------|------|------|
| **通用 AI** | 跨领域执行智能任务的系统 | 专家系统、规则引擎 |
| **机器学习** | 从数据中学习，无需显式编程 | 线性回归、决策树、SVM |
| **深度学习** | 多层神经网络，适合非结构化数据 | CNN（图像）、RNN（序列） |
| **生成式 AI** | 从学习数据中创造新内容 | ChatGPT、DALL·E |
| **大语言模型** | 海量文本训练的生成式 AI | GPT-4、BERT、Claude |

## 关键概念

### 提示工程
- **Zero-Shot**：不给示例
- **One-Shot**：给 1 个示例
- **Few-Shot**：给多个示例
- **Chain-of-Thought (CoT)**：引导逐步推理
- **Prompt Tuning**：调优提示以适应特定任务

### 核心术语
- **Token**：LLM 处理的基本文本单元（词/子词/字符）
- **Context Window**：LLM 一次能处理的最大 Token 数，超出会截断
- **Embeddings**：Token 的数值向量表示，捕获语义含义
- **Latent Space**：LLM 内部编码的知识/模式
- **Hallucination**：模型生成看似合理但错误的内容

### 推理参数（Bedrock）
| 参数 | 作用 | 取值影响 |
|------|------|---------|
| **Temperature** | 控制随机性 | 高 = 创造性/多样化 |
| **Top K** | 限制为 K 个最可能 Token | 越小越确定 |
| **Top P** | 累积概率阈值 | 比 Top K 更自适应灵活 |

### 搜索方式
- **Keyword Search**：精确匹配关键词
- **Semantic Search**：用 Embeddings 理解语义

## 学习类型对比

| 类型 | 数据 | 例子 |
|------|------|------|
| **监督学习** | 有标签 | 分类、回归 |
| **无监督学习** | 无标签 | 聚类、降维 |
| **强化学习** | 试错 + 奖励 | DeepRacer |

## 生成式 AI 模型类型

| 类型 | 应用 |
|------|------|
| **GANs** | 图像生成（StyleGAN、CycleGAN） |
| **VAEs** | 图像去噪、异常检测 |
| **Transformers** | 文本生成、翻译（GPT、BERT、T5） |
| **Diffusion Models** | 图像生成（Stable Diffusion、DALL·E 2） |
| **Flow-Based** | 高质量图像生成 |

## 评估指标

| 指标 | 用途 |
|------|------|
| **ROUGE** | 文本摘要质量 |
| **BLEU** | 翻译准确度（N-gram） |
| **Perplexity** | 语言模型预测质量（越低越好） |
| **Precision/Recall/F1** | 分类任务 |
| **MSE/RMSE** | 回归任务误差 |

## 考点提示
- 🔑 能够区分 AI/ML/DL/GenAI/LLM 的层级关系
- 🔑 知道各种推理参数的用途（Temperature vs Top-K vs Top-P）
- 🔑 理解 Hallucination 及其缓解方法（RAG、Fine-Tuning、HITL）
