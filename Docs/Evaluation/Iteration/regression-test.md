# Regression Test Suite

This document defines the standard regression test suite for the AI Product Assistant.

The purpose of these tests is to verify that changes to the System Prompt preserve existing behavior while improving maintainability or capability.

---

# RT01 — Incomplete User Story

## Objective

Verify that the AI identifies missing information without inventing facts.

## Prompt

```text
Analyze the following Product Backlog Item.

As a customer, I want faster checkout.
```

## Expected Behavior

### Product Backlog Item Type

- Detects the item as a User Story.

### Quality Assessment

- Identifies missing user value.
- Identifies missing acceptance criteria.
- Identifies lack of measurable outcome.
- Explains why the story is not implementation-ready.

### Missing Information

Prioritizes missing information that blocks refinement.

Examples include:

- user value
- measurable outcome
- acceptance criteria
- scope clarification

### Coaching

- Asks clarifying questions.
- Does not invent business goals.

### Analysis

Clearly separates:

- Evidence
- Reasoning
- Assumptions
- Limitations

### Recommendations

Recommendations are traceable to identified gaps.

---

# RT02 — Technical Improvement

## Objective

Verify Product Backlog Item Type detection for Technical Improvement.

## Prompt

```text
Analyze the following Product Backlog Item.

Improve dashboard performance.
```

## Expected Behavior

### Product Backlog Item Type

- Detects Technical Improvement.
- Explains uncertainty if appropriate.
- Does not classify as Bug without evidence.

### Quality Assessment

Identifies missing:

- scope
- baseline
- measurable target
- acceptance criteria
- user/business value

### Coaching

Requests clarification instead of making assumptions.

### Analysis

No fabricated technical causes.

---

# RT03 — Contradictory User Story

## Objective

Verify evidence-based reasoning when requirements appear internally inconsistent.

## Prompt

```text
Analyze the following Product Backlog Item.

As a customer,
I want checkout to require fewer steps,
so that security is increased by requiring additional verification.
```

## Expected Behavior

### Product Backlog Item Type

- Detects User Story.

### Analysis

Identifies the apparent contradiction.

Explains:

- evidence
- reasoning

without assuming a solution.

### Assumptions

Does not assume implementation techniques.

### Recommendations

Suggests clarification rather than resolving the conflict
