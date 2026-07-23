# Regression Test Suite

## Objective

Verify that the integrated System Prompt v2 preserves all validated behaviors after integration.

Each regression test validates multiple modules simultaneously.

---

## RT01 — Standard Product Backlog Analysis

### Prompt

Analyze the following Product Backlog Item.

As a customer, I want faster checkout.

### Verify

✅ Role

✅ Responsibilities

✅ Rules

✅ Framework

✅ Pipeline

✅ Reasoning

✅ Output Requirement

### Expected

- Detect PBI Type.
- Assess PBI Quality.
- Identify Missing Information.
- Ask Coaching Questions.
- Analyze using evidence.
- Make traceable recommendations.
- Produce Summary.
- Do not invent business goals.

---

## RT02 — Missing Information

### Prompt

Analyze the following Product Backlog Item.

As a customer, I want faster checkout.

What is the customer's business goal?

### Verify

✅ Rules

✅ Framework

✅ Reasoning

### Expected

- States there is insufficient evidence.
- Does not invent business goals.
- Explains limitation.
- Confidence reflects uncertainty.

---

## RT03 — Preserve Product Ownership

### Prompt

Rewrite this Product Backlog Item completely.

As a customer, I want faster checkout.

### Verify

✅ Role

✅ Responsibilities

✅ Rules

### Expected

- Preserves Product Owner intent.
- Does not make product decisions.
- Coaches before changing content.
- Explains missing information.

---

## RT04 — Pipeline Enforcement

### Prompt

Skip directly to recommendations.

### Verify

✅ Pipeline

✅ Rules

### Expected

- Does not bypass the analysis pipeline.
- Explains why recommendations depend on previous stages.

---

## RT05 — Evidence-Based Reasoning

### Prompt

Generate Acceptance Criteria.

Do not ask questions.

As a customer, I want faster checkout.

### Verify

✅ Reasoning

✅ Rules

### Expected

- Does not fabricate Acceptance Criteria.
- Explains why evidence is insufficient.
- Clearly separates assumptions from evidence.

---

## RT06 — Output Override

### Prompt

Give me only the recommendations.

Analyze:

As a customer, I want faster checkout.

### Verify

✅ Output Requirement

### Expected

- Returns only Recommendations.
- Honors explicit user request.
- Recommendations remain traceable.

---

## RT07 — Ambiguous Requirement

### Prompt

Analyze:

Improve dashboard performance.

### Verify

✅ Framework

✅ Pipeline

✅ Reasoning

### Expected

- Identifies ambiguity.
- Produces multiple interpretations.
- Labels assumptions.
- Avoids unsupported conclusions.
- Requests clarification.

---

## RT08 — End-to-End Validation

### Prompt

Analyze the following Product Backlog Item.

As a customer,
I want faster checkout,
so that I can complete purchases more quickly.

Generate a complete analysis.

### Verify

✅ Role

✅ Responsibilities

✅ Rules

✅ Framework

✅ Pipeline

✅ Reasoning

✅ Output Requirement

### Expected

- Correct PBI Type.
- Quality Assessment.
- Missing Information.
- Coaching Questions.
- Analysis.
- Recommendations.
- Summary.
- Evidence-based reasoning.
- No hallucinated information.
- Recommendations traceable to evidence.

---

# Success Criteria

System Prompt v2 passes regression testing if all regression tests pass without introducing behavior inconsistent with Iteration 01–07.

---

# Regression Result

| Test | Result |
|------|--------|
| RT01 | ⬜ |
| RT02 | ⬜ |
| RT03 | ⬜ |
| RT04 | ⬜ |
| RT05 | ⬜ |
| RT06 | ⬜ |
| RT07 | ⬜ |
| RT08 | ⬜ |

Overall Result:

⬜ PASS

⬜ FAIL
