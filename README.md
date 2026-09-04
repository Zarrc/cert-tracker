# 📚 Cert Tracker — AI-Powered Exam Preparation System

> **用 AI 自动整理备考资料、归纳笔记、生成练习题。**  
> 丢一个课程链接进 `resources/`，AI 自动读、写笔记、出题、更新进度。

> 🌐 **English edition?** The complete English system (own `CLAUDE.md`/`README.md`) lives in [`en/`](en/) — copy that folder to run an English workflow.

---

## ✨ 功能

| 功能 | 说明 |
|------|------|
| 📥 **自动摄取** | 丢课程/文档/链接到 `resources/`，AI 读取分析 |
| 📝 **智能笔记** | 按 Exam Domain 自动归纳为结构化笔记 |
| 🎯 **自动出题** | 从笔记内容生成选择题/是非题/简答题 |
| 📊 **进度追踪** | 进度条、题数统计、学习日志、错题本 |
| 🔄 **随时扩充** | 加新资料 → 自动追加笔记和题目 |

---

## 🚀 快速开始

### 1. 创建你的第一个考试

复制 `template/exam-name/` 目录，重命名为你的考试名（如 `aws-saa`）：

```
cp -r template/exam-name/ my-exam/
```

然后编辑 `my-exam/index.md`，填入考试信息。

### 2. 丢资料，让 AI 处理

```bash
# 把课程链接/PDF/文档放到 resources/
# 然后对 AI 说：
"处理这个资源"
```

AI 会自动：
1. 读取材料内容
2. 按 Domain 归纳笔记到 `notes/`
3. 生成练习题到 `练习题/`
4. 更新进度条

### 3. 随时自测

打开 `练习题/` 下的题目文件，或未来用练习页面读取。

---

## 📂 项目结构

```
cert-tracker/
├── CLAUDE.md              ← AI 行为配置（告诉 AI 如何工作）
├── README.md              ← 本文件（中文系统在根目录）
├── en/                    ← English edition（完整英文版，含自身 CLAUDE.md/README）
├── .gitignore
├── template/              ← 模板：加新考试时复制此目录
│   └── exam-name/
│       ├── index.md       ← 考试信息 + Domain + 进度
│       ├── notes/         ← AI 写的笔记（按 Domain 分文件）
│       ├── resources/     ← 你放原始资料的地方
│       └── progress/
│           ├── 学习日志.md
│           ├── 错题本.md
│           └── 模拟考记录.md
├── examples/              ← 真实示例
│   ├── aws-cloud-practitioner/
│   └── aws-ai-practitioner/
└── 练习题/                 ← AI 自动生成的题目
    └── index.md           ← 统计仪表盘
```

---

## 🧠 工作流

```
你放资源 → AI 读取
              ↓
        分析覆盖哪些 Domain
              ↓
        按 Domain 写笔记到 notes/
              ↓
        生成 3-5 道题追加到 练习题/
              ↓
        更新进度条 + 统计
```

---

## 💡 最佳实践

- **资料按考试分开**：每个考试独立的 `resources/` 目录
- **笔记按 Domain 分开**：一个 Domain 一个文件，便于聚焦复习
- **错题本及时记录**：做错的题记下来，AI 可以帮你分析薄弱点
- **练习题定期回顾**：考前反复刷，查漏补缺
