# CLF-C02 练习题

> 按 Domain 分组，一行一道题。
> 格式：`[题型] 题目 | 选项 | 答案: X | Domain: XXX`

---

## Domain 1: 云概念

[MC] AWS Global Infrastructure 中，Region 和 Availability Zone 的关系是什么？ | A) 每个 Region 只有一个 AZ B) 每个 Region 至少 3 个 AZ C) AZ 包含多个 Region D) 每个 AZ 只有一个数据中心 | 答案: B | Domain: 云概念
[MC] 责任共担模型中，哪个是客户的责任？ | A) 物理服务器安全 B) 数据中心电力 C) EC2 实例的操作系统补丁 D) AWS 网络基础设施 | 答案: C | Domain: 云概念
[TF] 混合云是指将多个公有云提供商连接在一起的架构。 | 答案: False（混合云是公有云+本地设施） | Domain: 云概念
[MC] Well-Architected Framework 的 6 个支柱不包括以下哪个？ | A) 安全性 B) 成本优化 C) 敏捷性 D) 可持续性 | 答案: C | Domain: 云概念
[MC] 以下哪个是云计算的六大优势之一？ | A) 需要长期合约 B) 前期巨额投资 C) 不再猜测容量 D) 固定地理位置 | 答案: C | Domain: 云概念

## Domain 2: 安全与合规

[MC] IAM 中，以下哪个组件用于给 AWS 服务分配权限？ | A) User B) Group C) Role D) MFA | 答案: C | Domain: 安全与合规
[MC] 以下哪个服务用于记录 AWS 账户的所有 API 调用？ | A) CloudWatch B) CloudTrail C) Config D) VPC Flow Logs | 答案: B | Domain: 安全与合规
[TF] Security Group 是无状态的，Network ACL 是有状态的。 | 答案: False（SG 有状态，NACL 无状态） | Domain: 安全与合规
[MC] GuardDuty、Inspector、Macie 三者的区别是？ | A) 都一样 B) GuardDuty 是威胁检测，Inspector 是漏洞扫描，Macie 是敏感数据发现 C) GuardDuty 是防火墙 D) Inspector 只检查 S3 | 答案: B | Domain: 安全与合规
[MC] 以下哪个是 MFA 设备？ | A) YubiKey B) EC2 C) S3 D) Lambda | 答案: A | Domain: 安全与合规
[MC] AWS Shield Advanced 主要防护什么类型的攻击？ | A) SQL 注入 B) DDoS C) 暴力破解 D) XSS | 答案: B | Domain: 安全与合规

## Domain 3: 技术

[MC] EC2 的哪种购买选项最高可有 90% 折扣，但实例可能随时被回收？ | A) 按需 B) 预留实例 C) Spot Instance D) Dedicated Host | 答案: C | Domain: 技术
[MC] S3 Standard-IA 适合什么场景？ | A) 频繁访问的数据 B) 不经常访问但需要快速恢复的数据 C) 长期归档 D) 访问模式不确定 | 答案: B | Domain: 技术
[TF] CloudFront 是 AWS 的内容分发网络（CDN）服务。 | 答案: True | Domain: 技术
[MC] 以下哪个是 NoSQL 数据库服务？ | A) RDS B) Aurora C) DynamoDB D) Redshift | 答案: C | Domain: 技术
[MC] Auto Scaling Group 的主要功能是什么？ | A) 分发流量 B) 根据负载自动增减实例 C) DNS 解析 D) 数据备份 | 答案: B | Domain: 技术
[MC] Lambda 的最大优势是什么？ | A) 支持所有语言 B) 无需管理服务器 C) 内置数据库 D) 免费使用 | 答案: B | Domain: 技术
[SA] EBS 和 EFS 的区别中，EBS 是块存储只能附加到一个 EC2（同 AZ），EFS 是什么类型的存储？ | 答案: 文件存储（NFS，可多个 EC2 共享） | Domain: 技术
[MC] 同 Region 内不同 AZ 之间的数据传输是否收费？ | A) 免费（私有 IP） B) 按 GB 收费 C) 按分钟收费 D) 不收费但有流量限制 | 答案: A | Domain: 技术

## Domain 4: 计费与定价

[MC] 数据从 AWS 传到互联网（出站）是否收费？ | A) 免费 B) 按 GB 收费 C) 仅 EC2 收费 D) 前 10GB 免费 | 答案: B | Domain: 计费
[MC] AWS Cost Explorer 的主要功能是什么？ | A) 设置预算 B) 可视化分析和预测成本 C) 架构设计 D) 安全审计 | 答案: B | Domain: 计费
[TF] Consolidated Billing 可以合并多个 AWS 账号的用量来获得更大折扣。 | 答案: True | Domain: 计费
[MC] AWS Support 计划中，哪个提供 15 分钟响应时间和专属 TAM？ | A) Basic B) Developer C) Business D) Enterprise | 答案: D | Domain: 计费
[MC] Trusted Advisor 在 Basic 计划中可以检查多少项？ | A) 0 B) 7 C) 全部 D) 50 | 答案: B | Domain: 计费

---

**统计**: 选择题 `16` · 是非题 `3` · 简答题 `1` · 总计 `20`
