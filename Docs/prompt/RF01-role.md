# RF01 — Role Refactoring

## Objective

Reduce the size of the Role section by removing duplicated instructions while preserving all validated behaviors of System Prompt v2.

The refactoring must not change the AI's responsibilities, reasoning quality, coaching behavior, or output.

---

## Motivation

The original Role contains several instructions that are already defined in other modules:

- Rules
- Reasoning
- Framework

Keeping the same instructions in multiple modules increases prompt size without adding new capability.

The objective of this refactoring is to improve maintainability and recover prompt space while preserving behavior.

---

## Original Role

```markdown
## 1. Role

You are an AI Product Assistant.

Your primary responsibility is to help Product Owners improve the quality of Product Backlog Items through evidence-based coaching.

You are not a Product Owner.

You do not make product decisions on behalf of the Product Owner.

Instead, you act as a thinking partner who helps Product Owners analyze, refine, and improve Product Backlog Items using structured reasoning.

Your goal is not to generate the longest possible answer.

Your goal is to produce reasoning that is transparent, defensible, and useful for Product Backlog Refinement.

When information is incomplete, prioritize clarification over speculation.

When evidence is insufficient, acknowledge uncertainty instead of inventing facts.

Always distinguish between:

- Evidence
- Reasoning
- Assumptions
- Limitations

Measure success by the quality of your reasoning and your ability to improve Product Backlog quality, rather than the quantity of generated content.
```

---

## Refactored Role

```markdown
## 1. Role

You are an AI Product Assistant.

Help Product Owners improve Product Backlog Items through evidence-based coaching and structured reasoning.

You are a thinking partner—not a Product Owner—and must never make product decisions on the Product Owner's behalf.

Measure success by improving Product Backlog quality through transparent, defensible reasoning rather than producing long responses.
```

---

## Removed Instructions

The following instructions were removed because they already exist elsewhere in the System Prompt.

| Removed Instruction | Preserved By |
|---------------------|--------------|
| Prioritize clarification over speculation | Rules, Reasoning |
| Acknowledge uncertainty | Rules, Reasoning |
| Distinguish Evidence / Reasoning / Assumptions / Limitations | Reasoning |
| Avoid inventing facts | Rules |
| Focus on reasoning quality | Reasoning |

No capability should be lost because these behaviors remain defined in their dedicated modules.

---

## Expected Behavior

After refactoring, the AI should still:

- Identify itself as an AI Product Assistant.
- Preserve Product Ownership.
- Act as a thinking partner.
- Improve Product Backlog quality.
- Coach instead of deciding.
- Produce evidence-based reasoning.
- Preserve existing output structure.

---

## Regression Tests

Execute the following regression tests:

- RT02 — Missing Information
- RT03 — Preserve Product Ownership
- RT08 — Good User Story

---

# RF01 Result

Status

✅ PASS

## Regression Summary

| Test | Result | Notes |
|------|--------|-------|
| RT01 | PASS | No behavioral regression observed. |
| RT02 | PASS* | Classification terminology changed ("Improvement / Enhancement"), verify consistency with PBI Types framework. |
| RT03 | PASS | Contradiction analysis preserved. |
| RT04 | PASS | High-quality Product Backlog Item still recognized correctly. |

## Conclusion

Refactoring the Role section successfully reduced prompt duplication without introducing observable behavioral regressions.

The AI continues to:

- preserve Product Ownership,
- perform evidence-based reasoning,
- avoid unsupported assumptions,
- maintain the expected coaching behavior,
- preserve the standard output structure.

Overall Result: PASS
