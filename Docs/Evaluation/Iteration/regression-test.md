# AI Product Assistant - Regression Test Suite

## Objective

Verify that changes to the System Prompt or Knowledge Base do not introduce regressions to existing capabilities.

Each regression test validates a specific behavior that has previously passed.

A regression test is considered **PASS** only when all expected behaviors are satisfied.

---

# Regression Workflow

Whenever the System Prompt or Knowledge Base changes:

1. Update one file only.
2. Upload the updated file to GPT Builder.
3. Execute all regression tests.
4. Verify expected behavior.
5. Fix regressions before continuing.
6. Commit the changes.

Never modify multiple knowledge files before running regression tests.

---

# Global Validation Checklist

Apply this checklist to every regression test.

| Validation | PASS |
|------------|:----:|
| Output follows the standard structure | ☐ |
| Classification is evidence-based | ☐ |
| Coaching principles are preserved | ☐ |
| Evidence-Based Reasoning is applied | ☐ |
| No unsupported assumptions | ☐ |
| Communication is natural | ☐ |
| Recommendations are traceable | ☐ |
| No duplicated information | ☐ |

---

# KB01 — Product Backlog Item Types

## RT01 — Bug Detection

### Prompt

```text
Analyze the following Product Backlog Item.

Fix the bug causing the application to crash during login.
```

### Expected

- Detect Bug Fix / Defect.
- Do not classify as Feature.
- Explain the reasoning using available evidence.

---

## RT02 — User Story Detection

### Prompt

```text
Analyze the following Product Backlog Item.

As a customer,
I want to view my transaction history.
```

### Expected

- User Story is the primary candidate.
- Explain why it fits.
- Do not invent business goals.

---

## RT03 — Technical Improvement

### Prompt

```text
Analyze the following Product Backlog Item.

Upgrade PostgreSQL from version 14 to version 16.
```

### Expected

- Detect Technical Improvement.
- Do not classify as User Story.
- Explain the reasoning.

---

## RT04 — Ambiguous PBI

### Prompt

```text
Analyze the following Product Backlog Item.

Improve checkout.
```

### Expected

- Present multiple candidate types.
- Explain the reasoning.
- Ask clarifying questions when appropriate.

---

# KB02 — Definition of Good Product Backlog Item

## RT05 — Incomplete PBI

### Prompt

```text
As a user,
I want a better dashboard.
```

### Expected

- Identify missing information.
- Do not invent Acceptance Criteria.
- Maintain a constructive coaching style.

---

## RT06 — Well-Defined PBI

### Prompt

```text
As a customer,
I want to view my transaction history
so that I can review previous purchases.
```

### Expected

- Recognize a relatively well-defined Product Backlog Item.
- Identify possible improvements without unnecessary criticism.

---

## RT07 — Early Refinement

### Prompt

```text
We have just started refinement.

This Product Backlog Item is still in an early stage.
```

### Expected

- Recognize the refinement stage.
- Avoid requiring all details immediately.

---

## RT08 — Contradictory PBI

### Prompt

```text
As a customer,
I want to delete my account.

Acceptance Criteria

- Users must not be able to delete their account.
```

### Expected

- Detect contradictory information.
- Explain the inconsistency.
- Avoid selecting one interpretation.

---

# KB03 — Coaching Principles

## RT09 — Preserve Product Ownership

### Prompt

```text
Should I prioritize Dark Mode?
```

### Expected

- Do not make Product Owner decisions.
- Help the user evaluate the decision.

---

## RT10 — Ask Before Assuming

### Prompt

```text
Improve checkout.

Create a Product Backlog Item.
```

### Expected

- Ask clarifying questions.
- Avoid inventing missing requirements.

---

## RT11 — Encourage Reflection

### Prompt

```text
Should I build a chat feature?
```

### Expected

- Encourage reflection.
- Avoid simply answering yes or no.

---

## RT12 — Facilitate Thinking

### Prompt

```text
Stakeholders want Export PDF.

Developers want performance improvements.

Which one should we choose?
```

### Expected

- Explain trade-offs.
- Avoid making the decision.

---

## RT13 — Focus on Outcomes

### Prompt

```text
I want a new checkout button.
```

### Expected

- Shift the discussion toward the desired outcome.
- Avoid focusing only on the proposed solution.

---

## RT14 — Continuous Improvement

### Prompt

```text
Is this Product Backlog Item bad?

As a user,
I want reports.
```

### Expected

- Provide constructive coaching.
- Avoid judgmental language.

---

## RT15 — Preserve Product Ownership (Explicit)

### Prompt

```text
Please prioritize my Product Backlog for me.
```

### Expected

- Avoid replacing the Product Owner.
- Support the decision-making process.

---

# KB04 — Evidence-Based Reasoning

## RT16 — Do Not Invent Information

### Prompt

```text
As a user,
I want a better dashboard.
```

### Expected

- Do not invent Acceptance Criteria.
- Do not invent business goals.
- Explain evidence limitations.
- Ask clarifying questions.

---

## RT17 — Separate Evidence from Assumptions

### Prompt

```text
As a customer,
I want faster checkout.
```

### Expected

- Clearly distinguish evidence from assumptions.
- Explain limitations.

---

## RT18 — Recommendation Traceability

### Prompt

```text
As a customer,
I want to view my transaction history.
```

### Expected

- Every recommendation is supported by previous analysis.
- Avoid unsupported recommendations.

---

## RT19 — Unsupported Assumption

### Prompt

```text
The stakeholder definitely wants to improve conversion.

Create a Product Backlog Item.
```

### Expected

- Do not accept unsupported assumptions as facts.
- Request clarification.
- Avoid inventing Product Goals.

---

# KB05 — Communication Guidelines

## RT20 — Natural Communication

### Prompt

```text
Analyze the following Product Backlog Item.

As a customer,
I want to view my transaction history.
```

### Expected

- Use natural language.
- Explain reasoning in complete sentences.
- Avoid literal translations such as:
  - "Supported because"
  - "Less likely because"
  - "Didukung karena"
  - "Kurang didukung"
- Preserve Agile terminology.
- Keep explanations easy to understand.

---

# Regression Completion Checklist

Regression testing is complete when:

- All regression tests pass.
- No previous capability regresses.
- No new hallucinations are introduced.
- Output remains consistent.
- Coaching behavior remains intact.
- Evidence-Based Reasoning remains consistent.
- Communication remains natural.
