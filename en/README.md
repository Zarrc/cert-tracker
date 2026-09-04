# 📚 Cert Tracker — AI-Powered Exam Preparation System

> **Let AI automatically organize study materials, summarize notes, and generate practice questions.**  
> Drop a course link into `resources/`, and the AI reads, notes, quizzes, and tracks progress for you.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 📥 **Auto Ingest** | Drop courses/docs/links into `resources/`, AI reads and analyzes |
| 📝 **Smart Notes** | Automatically organized by exam domain into structured notes |
| 🎯 **Auto Quiz** | Generate MC / True-False / Short Answer questions from notes |
| 📊 **Progress Tracking** | Progress bars, question stats, study logs, error journals |
| 🔄 **Extensible** | Add new materials → auto-appends notes and questions |

---

## 🚀 Quick Start

### 1. Add a new exam

Copy `template/exam-name/`, rename it to your exam code:

```
cp -r template/exam-name/ my-exam/
```

Edit `my-exam/index.md` with your exam details.

### 2. Drop materials, let AI process

```bash
# Put course links / PDFs / docs into resources/
# Then tell your AI:
"Process this resource"
```

The AI will automatically:
1. Read the material
2. Summarize key knowledge into `notes/` by domain
3. Generate practice questions into `practice-questions/`
4. Update progress bars

### 3. Practice anytime

Open `practice-questions/` to test yourself, or build a quiz app that reads these files.

---

## 📂 Project Structure

```
en/
├── CLAUDE.md              ← AI behavior config
├── README.md
├── .gitignore
├── template/              ← Copy this to add a new exam
│   └── exam-name/
│       ├── index.md       ← Exam info + domains + progress
│       ├── notes/         ← AI-generated notes (one file per domain)
│       ├── resources/     ← Your raw materials go here
│       └── progress/
│           ├── study-log.md
│           ├── error-log.md
│           └── mock-exam-log.md
├── examples/              ← Real-world examples
│   ├── aws-cloud-practitioner/
│   └── aws-ai-practitioner/
└── practice-questions/    ← AI-generated questions
    └── index.md           ← Stats dashboard
```

---

## 🧠 Workflow

```
You drop resources → AI reads
                        ↓
              Analyzes which domains covered
                        ↓
              Writes notes to notes/
                        ↓
              Generates 3-5 questions to practice-questions/
                        ↓
              Updates progress bars + stats
```

---

## 💡 Best Practices

- **Separate materials by exam**: Each exam has its own `resources/`
- **Separate notes by domain**: One file per domain for focused study
- **Log errors promptly**: AI can analyze your weak spots from the error log
- **Review questions regularly**: Drill before exam day
