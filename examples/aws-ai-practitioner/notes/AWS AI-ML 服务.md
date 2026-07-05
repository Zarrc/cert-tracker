# Domain 4: AWS AI/ML 服务

> 权重 28% · 对应资源：freeCodeCamp 15h 课程 (02:02:22 Bedrock · 08:08:46 SageMaker · 10:30:14 Managed ML)

---

## Amazon Bedrock（重点）

全托管 Serverless 服务，通过单一 API 提供多家 Foundation Models。

### 支持的模型
AI21 Labs · Anthropic · Cohere · Meta · Mistral AI · Stability AI · **Amazon Titan**

### Amazon Titan 模型
AWS 自研 FM，Bedrock 独占。

### Bedrock 功能

| 功能 | 说明 |
|------|------|
| **Knowledge Bases** | RAG — 从私有数据检索来 grounding 回答 |
| **Agents** | 多步骤任务规划 + 公司数据/工具 |
| **Guardrails** | 限制不适当/有风险的内容 |
| **PartyRock** | 无代码 GenAI 应用 playground |
| **Model Evaluation** | 比较 FM 的准确率/鲁棒性/毒性 |

### Bedrock 定价
- **On-Demand**：按 Token 付费
- **Provisioned Throughput**：预留容量（微调模型需要）

---

## Amazon SageMaker（全面）

| 组件 | 用途 |
|------|------|
| **Studio** | IDE：Notebook、调试、实验管理 |
| **Feature Store** | ML 特征中央仓库 |
| **Model Registry** | 模型版本管理 |
| **Pipelines** | 工作流编排 |
| **Model Monitor** | 漂移检测 |
| **Ground Truth** | 人工数据标注 |
| **Canvas** | 无代码建模 |
| **JumpStart** | 预训练模型 Hub |
| **Clarify** | 偏差检测 + 可解释性 |
| **Data Wrangler** | 可视化数据准备 |
| **Autopilot** | 自动建模/调优 |
| **A2I (Augmented AI)** | 低置信度预测人工审核 |
| **Managed Spot Training** | 用空闲 EC2 容量降成本 |
| **Profiler** | 资源效率识别 |

---

## AWS 托管 AI 服务速查

### 视觉
| 服务 | 用途 |
|------|------|
| **Rekognition** | 人脸分析、物体检测、内容审核 |
| **Textract** | OCR，从文档提取文字 |

### 语言
| 服务 | 用途 |
|------|------|
| **Comprehend** | NLP — 情感、实体、PII |
| **Translate** | 翻译 |
| **Transcribe** | 语音转文字 |
| **Polly** | 文字转语音 |
| **Lex** | 聊天机器人（Alexa 同技术） |

### 搜索与推荐
| 服务 | 用途 |
|------|------|
| **Kendra** | 智能文档搜索 |
| **Personalize** | 个性化推荐 |
| **Forecast** | 时序预测 |

### 其他
| 服务 | 用途 |
|------|------|
| **Fraud Detector** | 欺诈检测 |
| **Amazon Q** | GenAI 助手（Business/Developer/QuickSight/Connect） |
| **Intelligent Document Processing (IDP)** | Textract + Comprehend + A2I 组合 |

---

## GenAI 应用评估

### 关键指标
- **ROUGE**：摘要任务重叠度
- **BLEU**：翻译 N-gram 准确率
- **GLUE**：多任务 NLU 评估
- **HELM**：广泛语言模型评估
- **MMLU**：多领域知识测试
- **BIG-bench**：创造性/困难 AI 任务

### Hallucination 缓解

| 方法 | 说明 |
|------|------|
| **RAG** | 检索外部数据 grounding 回答 |
| **Fine-Tuning** | 在准确相关数据上训练 |
| **HITL** | 低置信度输出人工审核 |

---

## 考点提示
- 🔑 Bedrock vs SageMaker 的区别（Bedrock = FM 服务，SageMaker = 完整 ML 平台）
- 🔑 场景匹配题最多：给定问题选正确的 AWS 服务
- 🔑 RAG（Retrieval-Augmented Generation）的概念和工作原理
- 🔑 Amazon Titan 是 AWS 自研模型，Bedrock 独占
