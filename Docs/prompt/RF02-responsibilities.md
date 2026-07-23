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
## 2. Responsibilities

Your responsibilities are to:

1. Help Product Owners improve the quality of Product Backlog Items.

2. Analyze Product Backlog Items using evidence-based reasoning.

3. Identify missing, ambiguous, or inconsistent information.

4. Help Product Owners think critically through coaching rather than making decisions for them.

5. Recommend improvements while preserving the Product Owner's intent.
```

---

## Removed Instructions

The following instructions were removed because they already exist elsewhere in the System Prompt.

| Removed Instruction | Preserved By |
|---------------------|--------------|
| Explain reasoning transparently | Reasoning |
| Distinguish Evidence / Reasoning / Assumptions / Limitations | Reasoning |
| Ask clarifying questions when information is insufficient | Rules |
| Avoid unsupported assumptions and fabricated facts | Rules |
| Encourage coaching rather than prescription | Role, Framework |

No capability should be lost because these behaviors remain defined in their dedicated modules.

---

## Expected Behavior

After refactoring, the AI should still:

- Help Product Owners improve Product Backlog Items.
- Analyze Product Backlog Items using evidence-based reasoning.
- Identify missing information.
- Coach Product Owners rather than replacing their thinking.
- Preserve Product Ownership.
- Preserve existing output structure.

---

## Regression Test Scope

RF02 only refactors the **Responsibilities** section.

Since no reasoning logic, pipeline, framework, or output structure has changed, executing the complete regression suite is unnecessary.

The following regression tests provide sufficient coverage:

| Test | Purpose |
|------|---------|
| RT01 | Verify evidence-based analysis for an incomplete User Story. |
| RT02 | Verify Product Backlog Item Type detection for a Technical Improvement. |
| RT03 | Verify evidence-based reasoning for contradictory requirements. |
| RT04 | Verify recognition of a high-quality Product Backlog Item. |

---

## Execution Checklist

- [ ] Replace only the Responsibilities section.
- [ ] Update the GPT Builder.
- [ ] Execute RT01.
- [ ] Execute RT02.
- [ ] Execute RT03.
- [ ] Execute RT04.
- [ ] Compare the behavior with the baseline.
- [ ] Record PASS or FAIL.

---

## Result

| Test | Result | Notes |
|------|--------|-------|
| RT01 | ✅ PASS | No behavioral regression observed. |
| RT02 | ✅ PASS | Product Backlog Item Type detection preserved. |
| RT03 | ✅ PASS | Evidence-based reasoning for contradictory requirements preserved. |
| RT04 | ✅ PASS | High-quality Product Backlog Item recognized correctly with only minor refinement suggestions. |

Overall

✅ PASS

⬜ FAIL

---

## Conclusion

The Responsibilities refactoring successfully reduced duplicated instructions without introducing observable behavioral regressions.

The AI continues to:

- Help Product Owners improve Product Backlog Items.
- Perform evidence-based reasoning.
- Identify missing information.
- Coach rather than replace Product Owner decision-making.
- Preserve Product Ownership.
- Maintain the expected output structure.

The refactoring confirms that several responsibilities were duplicated by the Rules, Reasoning, Role, and Framework modules. Removing these duplicates improved maintainability and reduced prompt size without affecting the AI's observable behavior.

Overall Result: PASS
