# Cert Tracker — AI Exam Preparation System

> AI behavior configuration. Defines how to automatically process exam materials.

---

## Project Structure

```
en/
├── CLAUDE.md              ← This file
├── template/              ← Exam template
│   └── exam-name/
│       ├── index.md       ← Exam domains & progress
│       ├── notes/         ← AI-generated notes
│       ├── resources/     ← Raw materials
│       └── progress/      ← Study log / error log
├── examples/              ← Complete examples
└── practice-questions/    ← Generated questions
```

---

## Workflows

### 1. Ingest New Material

When you put materials into `resources/` and say "Process this resource":

1. **Read** the material (web page / PDF / document)
2. **Analyze** which exam domains it covers
3. **Summarize** key knowledge into `notes/` files
   - Structured Markdown: concept comparisons, key services, exam tips
4. **Generate questions** based on new knowledge (3-5 questions)
   - `[MC]` Multiple Choice · `[TF]` True/False · `[SA]` Short Answer
   - One line per question, tagged with domain
5. **Update** exam `index.md` progress bar + question stats + log

### 2. Study / Query

When you ask questions about an exam:

1. **Look up** the exam's `notes/` and `practice-questions/`
2. **Synthesize** an answer with source references
3. Optionally generate extra practice questions

### 3. Add a New Exam

Copy `template/exam-name/` → rename → edit `index.md` → start dropping materials

---

## Notes Format

- One file per domain (e.g., `notes/cloud-concepts.md`)
- Each file contains: core concepts, comparison tables, exam tips (`🔑` marker)
- Use `✅` `⚠️` for mastery tracking (AI auto-updates)

## Question Format

```
[MC] Question text | A) OptionA  B) OptionB  C) OptionC  D) OptionD | Answer: X | Domain: XXX
[TF] Statement | Answer: True/False | Domain: XXX
[SA] Short question | Answer: Keyword | Domain: XXX
```

One line per question, easy to append and machine-readable for future quiz apps.

---

## Progress Bar Rules

```
░░░░░░░░░░ 0%   — Not started
██░░░░░░░░ 20%  — Notes created
████░░░░░░ 40%  — All domains covered
██████░░░░ 60%  — Practice questions exist
████████░░ 80%  — Mock exam completed
██████████ 100% — Exam passed
```
