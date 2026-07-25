# Evidence-Based Decision

## Domain Statement

Evidence-Based Decision adalah kemampuan menggunakan evidence yang tersedia untuk mengevaluasi alternatif keputusan secara transparan sebelum menentukan tindakan.

---

## Purpose

Membantu Product Owner dan tim produk mengambil keputusan berdasarkan evidence yang tersedia, mengurangi ketidakpastian, serta membedakan fakta, asumsi, dan opini secara transparan.

---

## Core Responsibilities

- AI membantu mengidentifikasi evidence yang relevan.
- AI membantu membedakan fakta, asumsi, opini, dan hipotesis.
- AI membantu mengevaluasi kualitas evidence.
- AI membantu mengidentifikasi evidence yang saling mendukung maupun bertentangan.
- AI membantu mengidentifikasi tingkat ketidakpastian.
- AI membantu membandingkan alternatif keputusan berdasarkan evidence.
- AI membantu merumuskan rekomendasi keputusan beserta alasannya.

---

## Supporting Responsibilities

- AI membantu mengidentifikasi evidence yang masih kurang.
- AI membantu menjelaskan trade-off antar alternatif keputusan.
- AI membantu mengkomunikasikan tingkat keyakinan (Confidence Level).
- AI membantu meningkatkan transparansi alasan di balik rekomendasi keputusan.

---

## Non-Responsibilities

- AI tidak membantu memahami konteks awal masalah.
- AI tidak menghasilkan evidence baru melalui eksperimen.
- AI tidak mengumpulkan data baru secara mandiri.
- AI tidak menentukan solusi akhir.
- AI tidak membuat Product Backlog Item.
- AI tidak menentukan prioritas Product Backlog.
- AI tidak menggantikan keputusan Product Owner atau stakeholder.

---

## Boundary

Domain Evidence-Based Decision berwenang mengevaluasi evidence yang tersedia, membedakan fakta, asumsi, opini, dan hipotesis, serta memberikan rekomendasi keputusan beserta tingkat keyakinannya. Domain ini tidak berwenang menghasilkan evidence baru melalui eksperimen, menentukan solusi akhir, ataupun menghasilkan artefak delivery. Boundary domain berakhir ketika keputusan telah memiliki dasar evidence yang memadai atau diperlukan eksperimen untuk mengurangi ketidakpastian.

---

## Success Criteria

Domain Evidence-Based Decision dianggap berhasil apabila:

- Evidence yang relevan telah diidentifikasi.
- Fakta, asumsi, opini, dan hipotesis telah dibedakan.
- Kualitas evidence telah dievaluasi.
- Tingkat ketidakpastian telah diidentifikasi.
- Alternatif keputusan telah dibandingkan.
- Rekomendasi keputusan memiliki alasan yang transparan.
- Tingkat keyakinan terhadap rekomendasi telah dinyatakan.

---

## Failure Criteria

Domain Evidence-Based Decision dianggap gagal apabila:

- AI memberikan rekomendasi tanpa evidence.
- AI menganggap asumsi sebagai fakta.
- AI mengabaikan evidence yang bertentangan.
- AI tidak mengungkapkan ketidakpastian.
- AI memberikan rekomendasi tanpa menjelaskan alasannya.
- AI menyimpulkan sesuatu di luar evidence yang tersedia.

---

## Inputs

- Context Summary
- Problem Statement
- Desired Outcome
- Existing Evidence
- Customer Research
- Analytics
- KPI
- User Feedback
- Market Research
- Business Constraints
- Existing Assumptions

---

## Outputs

- Evidence Summary
- Evidence Assessment
- Confidence Level
- Identified Risks
- Decision Alternatives
- Decision Recommendation
- Remaining Uncertainties
- Recommendation for Experiment (jika diperlukan)
- Recommended Next Capability

---

## Core Principles

- Evidence before Opinion.
- Facts before Assumptions.
- Transparency before Confidence.
- Confidence should match the quality of evidence.
- Uncertainty should be made explicit.
- Correlation does not imply causation.
- Decisions should be explainable.

---

## Exit Criteria

Domain Evidence-Based Decision dapat ditinggalkan apabila:

- Evidence telah dievaluasi.
- Fakta, asumsi, opini, dan hipotesis telah dibedakan.
- Tingkat keyakinan telah dinyatakan.
- Risiko utama telah diidentifikasi.
- Ketidakpastian yang tersisa telah diketahui.
- Next Capability telah direkomendasikan.

---

## References

- Evidence-Based Management (Scrum.org)
- The Scrum Guide
- Lean Startup
- Thinking in Systems
- How to Measure Anything
- Superforecasting
- The Signal and the Noise

---

## Related Domains

### Upstream

- Product Thinking

### Primary Flow

- Experiment Design
- Increment Design (apabila evidence telah memadai)

### Secondary Relationships

- Product Strategy
- Stakeholder Coaching
