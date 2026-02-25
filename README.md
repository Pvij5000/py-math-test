# 🧮 Adaptive Math Tutor

> A Python-based interactive learning system exploring adaptive assessment, performance tracking, and the foundational concepts behind reinforcement learning from human feedback (RLHF).

---

## Overview

What started as a simple arithmetic quiz has become a sandbox for exploring how software can **respond to human performance** — adjusting difficulty, tracking progress over time, and building toward predictive models of learner behavior.

The original codebase already implements higher-order functions, modular arithmetic, and stateful game loops — concepts that inform the adaptive architecture in later stages.

This project sits at the intersection of two fields I care deeply about: **cognitive science** (how humans learn and respond to feedback) and **machine learning** (how systems can model and adapt to human behavior). The connection is not accidental — modern AI alignment techniques like RLHF are, at their core, systems that learn from human feedback signals. This project explores that idea from the ground up.

---

## Current Features

- Generates randomized math problems (addition, modulo, floor division) using Python's `random` module
- Higher-order functions pass question types dynamically at runtime
- Stateful game loop tracks questions answered and correct count
- Accepts user input and evaluates correctness in real time
- Computes and displays final accuracy percentage

---

## Roadmap: From Quiz to Adaptive Learning System

### ✅ Stage 1 — Basic Quiz (Complete)
*Concepts: control flow, randomization, user input, conditionals, higher-order functions, modular arithmetic*

Interactive math quiz supporting addition, modulo (`%`), and floor division (`//`). User selects test type, answers 5 questions, receives final accuracy score.

---

### ✅ Stage 2 — Score Tracking & Data Collection (Complete)
*Concepts: data persistence, file I/O, JSON, structured logging, session management*

- Logs every attempt to `results.json` with timestamp, operands, operation, correct answer, user answer, correctness
- Displays session summary and all-time accuracy
- Each result record is a structured observation — the dataset that feeds Stage 5

---

### 📊 Stage 3 — Performance Visualization (Next)
*Concepts: pandas, matplotlib, seaborn, descriptive statistics*

- Load session history into a pandas DataFrame
- Plot accuracy over time
- Visualize error patterns by operation type and number range
- Compute rolling averages and streaks

---

### 🎯 Stage 4 — Adaptive Difficulty
*Concepts: rule-based systems, feedback loops, state machines*

- Dynamically adjust number ranges based on recent accuracy
- Above 80% on a question type → increase difficulty
- Below 50% → reduce difficulty and increase hints
- Rule-based adaptive system — direct conceptual precursor to reinforcement learning

---

### 🤖 Stage 5 — Predictive Modeling
*Concepts: scikit-learn, logistic regression, feature engineering, train/test split*

- Train a classifier on accumulated session data
- Features: question type, number range, recent accuracy, streak length
- Predict whether user will answer correctly
- Evaluate with accuracy, precision, recall

---

### 🧠 Stage 6 — Feedback Loop & RLHF Concepts
*Concepts: reward modeling, human preference data, policy adjustment*

- User rates question difficulty after answering
- Preference signals adjust question generation policy
- Explicit connection to RLHF in large language models
- Documents the parallel between this system and modern AI alignment research

---

## Why This Project Matters

I am a career-transitioning researcher with a background in behavioral neuroscience (published in the *Journal of Neuroscience*), advanced mathematics (real analysis, complex analysis, differential equations, numerical methods, linear algebra), and enterprise data systems. I am building toward graduate research at the intersection of cognitive science and generative AI.

This project is my public laboratory — a place where I work through foundational programming and ML concepts in the open, building on each stage before moving to the next. The topic of adaptive human learning maps directly to my research interests in human-AI interaction, RLHF, and AI alignment.

Every commit in this repo is a data point in my own learning trajectory.

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Jupyter Notebook | Interactive development |
| `random` | Question generation |
| `json` | Data persistence (Stage 2+) |
| `pandas` | Data analysis (Stage 3+) |
| `matplotlib` / `seaborn` | Visualization (Stage 3+) |
| `scikit-learn` | Machine learning (Stage 5+) |

---

## Getting Started
```bash
git clone https://github.com/Pvij5000/py-math-test.git
cd py-math-test
jupyter lab
```

---

## Connect

- GitHub: [@Pvij5000](https://github.com/Pvij5000)
- Email: paris.vij01@gmail.com
- Location: Austin, TX

---

*"Non-significant results require methodological interrogation rather than dismissal."*
*— A principle from behavioral research that applies equally well to debugging neural networks.*

---

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Status-Active%20Development-green)
![Stage](https://img.shields.io/badge/Current%20Stage-2%20Complete-yellow)
