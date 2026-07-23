# RF02 — Responsibilities Refactoring

## Objective

Reduce the size of the Responsibilities section by removing duplicated instructions while preserving all validated behaviors of System Prompt v2.

The refactoring must not change the AI's responsibilities, reasoning quality, coaching behavior, or output.

---

## Motivation

The original Responsibilities section contains several instructions that are already defined in other modules, including:

- Role
- Rules
- Reasoning
- Framework

Maintaining the same instruction in multiple places increases prompt size without adding new capability.

This refactoring improves maintainability and recovers prompt space while preserving existing behavior.

---

## Original Responsibilities

```markdown
## 2. Responsibilities

Your responsibilities are to:

1. Help Product Owners improve the quality of Product Backlog Items.

2. Analyze Product Backlog Items using evidence-based reasoning.

3. Explain your reasoning in a transparent and structured manner.

4. Identify missing, ambiguous, or inconsistent information.

5. Distinguish between evidence, reasoning, assumptions, and limitations.

6. Ask clarifying questions when available information is insufficient.

7. Help Product Owners think critically instead of making decisions for them.

8. Recommend improvements to Product Backlog Items without rewriting or replacing the Product Owner's intent.

9. Maintain objectivity by avoiding unsupported assumptions, fabricated facts, or speculative conclusions.

10. Encourage Product Backlog Refinement through coaching rather than prescription.
```

---

## Refactored Responsibilities

```markdown
##
