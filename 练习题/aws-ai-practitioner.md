# AIF-C01 练习题

> 按 Domain 分组，一行一道题。
> 格式：`[题型] 题目 | 选项 | 答案: X | Domain: XXX`

---

## Domain 1: AI/ML 基础

[MC] 以下哪种方式是通过在提示中加入例子来增强模型表现？ | A) Fine-Tuning B) In-Context Learning C) Reinforcement Learning D) Transfer Learning | 答案: B | Domain: AI/ML 基础
[MC] 推理参数中，控制模型输出随机性的是哪个？ | A) Top-K B) Top-P C) Temperature D) Batch Size | 答案: C | Domain: AI/ML 基础
[TF] Chain-of-Thought prompting 是通过引导模型逐步推理来提高准确性。 | 答案: True | Domain: AI/ML 基础
[MC] 以下哪个是深度学习区别于传统机器学习的主要特征？ | A) 需要手工特征工程 B) 自动学习特征表示 C) 只能处理结构化数据 D) 训练成本更低 | 答案: B | Domain: AI/ML 基础
[SA] 什么指标用于衡量语言模型预测下一个 Token 的质量？（越低越好） | 答案: Perplexity | Domain: AI/ML 基础
[MC] 以下哪个是生成式 AI 的典型例子？ | A) 线性回归 B) 决策树 C) ChatGPT D) K-Means 聚类 | 答案: C | Domain: AI/ML 基础
[TF] Zero-Shot prompting 是指在提示中提供多个示例来引导模型。 | 答案: False (Zero-Shot 不给示例，Few-Shot 给多个) | Domain: AI/ML 基础
[MC] Hallucination 在 LLM 中指的是什么？ | A) 模型训练时产生错误 B) 模型生成看似合理但错误的内容 C) 模型拒绝回答问题 D) 模型输出过于冗长 | 答案: B | Domain: AI/ML 基础

## Domain 2: 数据处理与特征工程

[MC] 在 ML 数据预处理中，常用的训练/验证/测试数据分割比例是？ | A) 60/20/20 B) 70/15/15 C) 80/10/10 D) 90/5/5 | 答案: C | Domain: 数据处理
[MC] AWS 的哪个服务用于可视化数据准备，并支持可复用的转换"配方"？ | A) SageMaker Clarify B) Glue DataBrew C) Athena D) QuickSight | 答案: B | Domain: 数据处理
[TF] SageMaker Feature Store 是用于存储 ML 特征的中央仓库。 | 答案: True | Domain: 数据处理
[MC] 以下哪个 AWS 服务适合存储 Embeddings 并做向量相似搜索？ | A) S3 Standard B) Amazon OpenSearch C) CloudFront D) Route 53 | 答案: B | Domain: 数据处理
[SA] ETL 全称是什么？ | 答案: Extract, Transform, Load | Domain: 数据处理
[MC] SageMaker Ground Truth 的主要用途是什么？ | A) 模型训练 B) 人工数据标注 C) 模型部署 D) 成本监控 | 答案: B | Domain: 数据处理

## Domain 3: 模型训练与部署

[MC] 模型在训练集上表现很好但在测试集上表现差，这是什么问题？ | A) Underfitting B) Overfitting C) Data Drift D) Concept Drift | 答案: B | Domain: 模型训练
[MC] SageMaker 的哪种推理方式最适合断续流量、自动伸缩的场景？ | A) Real-Time B) Batch Transform C) Serverless D) Provisioned Throughput | 答案: C | Domain: 模型训练
[TF] Fine-Tuning 的一个风险是灾难性遗忘（Catastrophic Forgetting）。 | 答案: True | Domain: 模型训练
[MC] 以下哪个是 Bedrock 的部署选项？ | A) Batch Transform B) On-Demand C) Serverless D) Real-Time | 答案: B | Domain: 模型训练
[MC] Data Drift 和 Concept Drift 的区别是什么？ | A) Data Drift 是标签改变，Concept Drift 是数据改变 B) Data Drift 是输入分布改变，Concept Drift 是输入输出关系改变 C) 两者一样 D) Data Drift 只在训练时发生 | 答案: B | Domain: 模型训练
[SA] 哪个 AWS 工具用于 ML 工作流编排？ | 答案: SageMaker Pipelines | Domain: 模型训练

## Domain 4: AWS AI/ML 服务

[MC] Amazon Bedrock 是什么类型的服务？ | A) 关系型数据库 B) 全托管的 Foundation Models 服务 C) 容器编排服务 D) 内容分发网络 | 答案: B | Domain: AWS AI/ML 服务
[MC] Amazon Titan 是什么？ | A) AWS 的 GPU 芯片 B) AWS 自研的基础模型 C) 一种 NoSQL 数据库 D) 安全审计工具 | 答案: B | Domain: AWS AI/ML 服务
[TF] Bedrock Knowledge Bases 通过 RAG 方式从私有数据检索来增强回答。 | 答案: True | Domain: AWS AI/ML 服务
[MC] 以下哪个 AWS 服务是用于人脸分析和内容审核的？ | A) Textract B) Rekognition C) Comprehend D) Polly | 答案: B | Domain: AWS AI/ML 服务
[MC] SageMaker 和 Bedrock 的主要区别是什么？ | A) Bedrock 更贵 B) SageMaker 是完整 ML 平台，Bedrock 专注 FM 服务 C) 两者完全一样 D) SageMaker 不能训练模型 | 答案: B | Domain: AWS AI/ML 服务
[MC] Amazon Lex 是什么服务？ | A) 翻译服务 B) 聊天机器人服务 C) 语音转文字 D) 文字转语音 | 答案: B | Domain: AWS AI/ML 服务
[SA] RAG 的全称是什么？ | 答案: Retrieval-Augmented Generation | Domain: AWS AI/ML 服务

## Domain 5: AI/ML 治理与安全

[MC] SageMaker Clarify 的主要用途是什么？ | A) 数据标注 B) 模型偏差检测和可解释性 C) 模型部署 D) 成本优化 | 答案: B | Domain: 治理与安全
[TF] Responsible AI 的六大原则包括公平性、可解释性、隐私、鲁棒性、透明度和问责制。 | 答案: True | Domain: 治理与安全
[MC] 哪个 AWS 服务可用于自助获取 SOC、PCI 合规报告？ | A) Artifact B) GuardDuty C) Macie D) Inspector | 答案: A | Domain: 治理与安全
[MC] AI/ML 安全中，哪个网络最佳实践用于隔离 SageMaker？ | A) Internet Gateway B) PrivateLink/VPC Endpoints C) NAT Gateway D) Direct Connect | 答案: B | Domain: 治理与安全

---

**统计**: 选择题 `17` · 是非题 `5` · 简答题 `4` · 总计 `26`
