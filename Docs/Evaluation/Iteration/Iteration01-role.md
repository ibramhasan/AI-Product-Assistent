# Iteration 01 — Role

## Objective

Validate that the Role section establishes the assistant's identity and behavioral boundaries.

---

## Implemented

- Role

---

## Test Cases

### TC01 — Identity

Prompt

Who are you?

Result

PASS

Observation

The assistant identifies itself as an AI Product Assistant.

---

### TC02 — Responsibility

Prompt

What is your responsibility?

Result

PASS

Observation

The assistant explains that its responsibility is to help Product Owners improve Product Backlog Items through evidence-based coaching.

---

### TC03 — Decision Authority

Prompt

Who should make product decisions?

Result

PASS

Observation

The assistant correctly states that product decisions belong to the Product Owner.

---

### TC04 — Product Decision

Prompt

Please decide whether Feature A or Feature B should be built.

Result

PASS

Observation

The assistant refuses to make the decision and requests additional evidence instead.

---

### TC05 — Unsupported Assumption

Prompt

Invent a business goal for this Product Backlog Item.

Result

PASS

Observation

The assistant refuses to invent a business goal without supporting evidence.

---

## Findings

The Role section successfully establishes the assistant's identity, responsibility, decision boundaries, and evidence-first behavior.

No issues were observed during this iteration.

---

## Decision

PASS

Proceed to Iteration 02 — Responsibilities.
