# Evidence-Based Decision Tests

This document defines the expected behavior of the Evidence-Based Decision capability.

---

# Happy Path

## EBD-HP-001 — Evaluate Available Evidence

### Intent

Evaluate available evidence before making a product decision.

### User Input

We have analytics showing a 25% increase in customer engagement after introducing personalized recommendations. Customer interviews also indicate positive feedback. Should we continue investing in this capability?

### Expected Capability

Evidence-Based Decision

### Expected Artifact

Decision Recommendation

### Expected Behavior

- Review the available evidence.
- Assess the quality and relevance of the evidence.
- Distinguish facts from assumptions.
- Evaluate remaining uncertainty.
- Produce a Decision Recommendation.
- Recommend the next capability.

### Should Not

- Ignore conflicting evidence.
- Recommend implementation details.
- Create Product Backlog Items.
- Design an Increment.

### Success Criteria

- Evaluates the available evidence.
- Explains the rationale behind the recommendation.
- Makes uncertainty explicit.
- Produces a Decision Recommendation.

### Failure Criteria

- Makes unsupported conclusions.
- Ignores evidence quality.
- Jumps directly to implementation.

---

## EBD-HP-002 — Compare Decision Alternatives

### Intent

Compare multiple alternatives before selecting a recommendation.

### User Input

We can either improve onboarding or optimize search performance. Both initiatives have supporting evidence, but we can only prioritize one this quarter.

### Expected Capability

Evidence-Based Decision

### Expected Artifact

Decision Recommendation

### Expected Behavior

- Identify decision alternatives.
- Compare available evidence.
- Explain trade-offs.
- Assess confidence.
- Produce a Decision Recommendation.

### Should Not

- Recommend both without analysis.
- Ignore trade-offs.
- Build a roadmap.

### Success Criteria

- Compares alternatives objectively.
- Explains trade-offs.
- Produces a Decision Recommendation.

### Failure Criteria

- Chooses an option without justification.
- Ignores available evidence.

---

## EBD-HP-003 — Evaluate a Product Hypothesis

### Intent

Determine whether available evidence supports a product hypothesis.

### User Input

We believe simplifying the registration process will increase conversion. We have usability testing results from twenty participants supporting this hypothesis.

### Expected Capability

Evidence-Based Decision

### Expected Artifact

Decision Recommendation

### Expected Behavior

- Review the available evidence.
- Assess whether the evidence supports the hypothesis.
- Explain confidence and remaining uncertainty.
- Produce a Decision Recommendation.

### Should Not

- Treat assumptions as facts.
- Recommend implementation without evaluation.

### Success Criteria

- Evaluates the hypothesis objectively.
- Makes confidence explicit.
- Produces a Decision Recommendation.

### Failure Criteria

- Accepts the hypothesis without evidence.
- Skips uncertainty assessment.

---

## EBD-HP-004 — Assess Decision Risk

### Intent

Assess the risks associated with a product decision.

### User Input

Launching this feature could increase customer engagement, but it also introduces operational complexity. We want to understand the
