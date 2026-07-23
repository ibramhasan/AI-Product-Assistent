# AI Product Assistant Architecture

## Overview

AI Product Assistant dirancang menggunakan pendekatan modular.

Setiap komponen memiliki tanggung jawab yang jelas sehingga proses berpikir AI dapat dipahami, diuji, dan dikembangkan secara bertahap.

Repository ini memisahkan antara:

- tujuan sistem,
- pengetahuan,
- proses berpikir,
- evaluasi,
- dan evolusi sistem.

Pendekatan ini membuat AI lebih mudah dipelihara dibandingkan menyimpan seluruh logika di dalam satu System Prompt.

---

# Architecture

Repository terdiri dari lima layer.

Strategy Layer

↓

Knowledge Layer

↓

Execution Layer

↓

Orchestration Layer

↓

Validation Layer

---

# Strategy Layer

Menjelaskan mengapa AI dibangun dan masalah apa yang ingin diselesaikan.

Folder dan dokumen:

- Vision.md
- Problem-statement.md
- Mvp.md
- AI-Decision-framework.md

---

# Knowledge Layer

Menyediakan prinsip dan pengetahuan yang digunakan AI ketika mengambil keputusan.

Folder:

Framework/

Knowledge-base/

Framework berisi prinsip Product Management, Agile, Coaching, dan Evidence-Based Reasoning.

Knowledge Base berisi referensi yang dapat digunakan AI selama proses analisis.

---

# Execution Layer

Mendefinisikan bagaimana AI memproses Product Backlog Item.

Folder:

Pipeline/

Reasoning/

Pipeline menjelaskan tahapan kerja AI.

Reasoning mendefinisikan aturan inferensi, decision tree, decision rule, dan output specification.

---

# Orchestration Layer

Menghubungkan seluruh komponen repository menjadi satu System Prompt.

System Prompt tidak menyimpan business logic.

System Prompt hanya mengorkestrasi:

- Framework
- Pipeline
- Reasoning
- Knowledge Base

---

# Validation Layer

Memastikan kualitas AI tetap terjaga.

Folder:

Evaluation/

Experiments/

Test-case/

Workflow/

Evaluation digunakan untuk mengukur kualitas output.

Experiments digunakan untuk mencatat eksperimen.

Test Cases digunakan sebagai dataset pengujian.

Workflow menyimpan evolusi System Prompt.

---

# Repository Flow

Strategy

↓

Knowledge

↓

Execution

↓

System Prompt

↓

AI Output

↓

Evaluation

↓

Experiments

↓

Repository Improvement

---

# Design Principles

Repository mengikuti prinsip berikut.

- Separation of Concerns
- Modular Architecture
- Evidence-Based Reasoning
- Coaching Before Conclusion
- Continuous Evaluation
- Experiment-Driven Improvement

---

# Guiding Principle

Prompt bukan pusat sistem.

Prompt hanya menjadi orchestrator.

Pengetahuan berada pada Framework.

Proses berada pada Pipeline.

Aturan inferensi berada pada Reasoning.

Kualitas dijaga melalui Evaluation.

Perubahan dilakukan melalui Experiments.
