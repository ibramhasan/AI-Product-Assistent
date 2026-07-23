# Iteration 07 — Output Requirement

## Objective

Validate that the assistant consistently produces responses using the project's standard output structure.

The focus of this iteration is not the correctness of the analysis itself, but the consistency, completeness, and flexibility of the response format.

---

# Scope

This iteration validates whether the assistant can:

- produce outputs using the defined section order,
- include every required section,
- explicitly indicate when information is missing,
- avoid duplicate information,
- maintain recommendation traceability,
- provide concise summaries,
- allow users to override the default output format.

---

# Test Results

| Test | Description | Result |
|------|-------------|--------|
| TC01 | Follow Standard Output Order | ✅ PASS |
| TC02 | Preserve Missing Sections | ✅ PASS |
| TC03 | Avoid Duplicate Information | ✅ PASS |
| TC04 | Recommendation Traceability | ✅ PASS |
| TC05 | Summary Behavior | ✅ PASS |
| TC06 | User Output Override | ✅ PASS |

---

# Key Findings

## 1. Output consistently follows the standard structure

The assistant produces responses using the predefined section order.

Default output:

1. Product Backlog Item Type
2. Product Backlog Item Quality Assessment
3. Missing Information
4. Coaching Questions
5. Product Backlog Analysis
6. Recommendations
7. Summary

The section order remains consistent across analyses.

---

## 2. Missing information is explicitly represented

When required information is unavailable, the assistant does not remove the corresponding section.

Instead, it explicitly communicates that the information is:

- Missing
- Unknown
- Cannot be determined from available evidence

This improves transparency and keeps the output predictable.

---

## 3. Information is not unnecessarily duplicated

Each section serves a distinct purpose.

Observations include:

- Analysis explains findings.
- Recommendations focus on improvement actions.
- Summary consolidates earlier observations.

Repeated information is minimized.

---

## 4. Recommendations are traceable

Recommendations include clear justification.

Rather than presenting recommendations as isolated advice, each recommendation explains why it exists based on previous analysis.

This significantly improves explainability.

---

## 5. Summary behaves as a summary

The Summary section consolidates key findings.

It does not introduce:

- new evidence,
- new recommendations,
- additional assumptions.

This maintains a clear separation between analysis and conclusion.

---

## 6. User requests can override the default format

When users explicitly request a different output format (for example, "Give me only recommendations."), the assistant follows the user's request.

This behavior is consistent with the Output Requirement:

> Unless the user explicitly requests otherwise...

The default structure remains the standard behavior while still allowing user flexibility.

---

# Overall Assessment

The Output Requirement successfully standardizes the assistant's responses.

The assistant consistently demonstrates:

- predictable output structure,
- complete section coverage,
- explicit handling of missing information,
- minimal duplication,
- recommendation traceability,
- flexible user-directed formatting.

---

# Conclusion

Iteration 07 successfully validates the Output Requirement layer.

The assistant now produces responses that are both consistent and adaptable.

Together with the validated Role, Responsibilities, Rules, Framework, Pipeline, and Reasoning layers, the project now possesses a complete and modular System Prompt architecture ready for integration.
