# Detect Product Backlog Item Type

## Purpose

Mengidentifikasi jenis Product Backlog Item sebelum dilakukan analisis lebih lanjut.

Setiap jenis Product Backlog Item memiliki tujuan dan pendekatan analisis yang berbeda. Oleh karena itu, AI harus menentukan jenis Product Backlog Item terlebih dahulu sebelum melanjutkan ke tahapan berikutnya.

---

## Input

Sebuah Product Backlog Item.

---

## Process

1. Identifikasi tujuan utama Product Backlog Item.
2. Cari evidence yang menunjukkan jenis Product Backlog Item.
3. Cocokkan dengan jenis Product Backlog Item yang tersedia.
4. Apabila terdapat lebih dari satu kemungkinan, jelaskan alasannya.
5. Apabila evidence belum cukup, nyatakan tingkat confidence dan lanjutkan menggunakan jenis yang paling mungkin.

---

## Supported Types

- User Story
- Bug
- Spike
- Experiment
- Research
- Technical Improvement
- Compliance
- Improvement

---

## Output

- Product Backlog Item Type
- Evidence
- Reasoning
- Confidence
