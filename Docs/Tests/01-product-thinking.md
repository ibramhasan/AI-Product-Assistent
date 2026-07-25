# Product Thinking Tests

This document defines the expected behavior of the Product Thinking capability.

---

# Happy Path

## PT-HP-001 — Identify a Product Problem

### Intent

Understand a product problem before exploring solutions.

### User Input

Our mobile banking application has experienced a 30% drop in user retention over the last three months. We want to understand why this is happening before deciding what to build next.

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Understand the product context.
- Identify the primary product problem.
- Clarify the desired outcome.
- Distinguish facts from assumptions.
- Produce a Problem Statement.
- Recommend the next capability.

### Should Not

- Recommend implementation.
- Create Product Backlog Items.
- Design an Increment.
- Prioritize features.

### Success Criteria

- Produces a Problem Statement.
- Clearly identifies the product problem.
- Distinguishes facts from assumptions.
- Recommends Evidence-Based Decision as the next capability.

### Failure Criteria

- Immediately proposes a solution.
- Creates Product Backlog Items.
- Begins implementation planning.
- Skips producing the Problem Statement.

---

## PT-HP-002 — Discover Customer Pain Points

### Intent

Explore customer problems before discussing solutions.

### User Input

Customers frequently abandon the checkout process before completing payment. We want to understand what problems they are experiencing.

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Explore the customer journey.
- Identify customer pain points.
- Clarify the desired outcome.
- Distinguish observations from assumptions.
- Produce a Problem Statement.
- Recommend the next capability.

### Should Not

- Suggest UI improvements.
- Recommend technical solutions.
- Create Product Backlog Items.
- Estimate implementation effort.

### Success Criteria

- Focuses on understanding customer problems.
- Identifies information gaps.
- Produces a Problem Statement.
- Recommends Evidence-Based Decision.

### Failure Criteria

- Assumes the root cause without evidence.
- Suggests features immediately.
- Skips problem exploration.

---

## PT-HP-003 — Clarify a Product Goal

### Intent

Clarify the desired Product Goal before exploring solutions.

### User Input

Our company wants to improve customer engagement, but we're not sure what outcome we should target first.

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Understand the business objective.
- Clarify the desired product outcome.
- Explore the underlying product problem.
- Produce a Problem Statement.
- Recommend the next capability.

### Should Not

- Recommend features.
- Build a roadmap.
- Create Product Backlog Items.
- Design an Increment.

### Success Criteria

- Clarifies the desired outcome.
- Identifies the product problem.
- Produces a Problem Statement.
- Recommends Evidence-Based Decision.

### Failure Criteria

- Begins solution design immediately.
- Defines implementation work.
- Skips product discovery.

---

## PT-HP-004 — Assess Whether a Problem Is Worth Solving

### Intent

Determine whether sufficient understanding exists before investing in a solution.

### User Input

We have received several customer complaints about slow search performance, but we don't yet know how widespread the issue is or how much impact it has.

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Understand the reported problem.
- Identify known facts and unknowns.
- Clarify the business impact.
- Produce a Problem Statement.
- Recommend the next capability.

### Should Not

- Assume the problem is significant.
- Recommend technical optimization.
- Create Product Backlog Items.

### Success Criteria

- Makes uncertainty explicit.
- Produces a Problem Statement.
- Identifies information gaps.
- Recommends Evidence-Based Decision.

### Failure Criteria

- Treats assumptions as facts.
- Suggests implementation immediately.

---

## PT-HP-005 — Understand Stakeholder Needs

### Intent

Understand stakeholder perspectives before discussing product solutions.

### User Input

Marketing wants faster feature releases while Customer Support wants better product stability. We need to better understand the underlying product problem.

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Understand stakeholder perspectives.
- Identify desired outcomes.
- Clarify the underlying product problem.
- Produce a Problem Statement.
- Recommend the next capability.

### Should Not

- Decide which stakeholder is correct.
- Prioritize requests.
- Build a roadmap.
- Create Product Backlog Items.

### Success Criteria

- Captures stakeholder perspectives.
- Produces a Problem Statement.
- Identifies the shared product problem.
- Recommends Evidence-Based Decision.

### Failure Criteria

- Takes sides immediately.
- Recommends implementation.
- Skips understanding stakeholder goals.

---

# Edge Case

## PT-EC-001 — Insufficient Problem Context

### Intent

Determine whether the assistant requests clarification when the available information is insufficient.

### User Input

Our product isn't performing well. What should we do?

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Recognize that the problem statement is incomplete.
- Ask clarifying questions.
- Identify missing information before drawing conclusions.

### Should Not

- Guess the root cause.
- Recommend features.
- Create Product Backlog Items.

### Success Criteria

- Requests additional context.
- Avoids unsupported assumptions.
- Delays producing a complete Problem Statement until sufficient information is available.

### Failure Criteria

- Invents facts.
- Jumps directly to solutions.

---

## PT-EC-002 — Conflicting Stakeholder Perspectives

### Intent

Verify that conflicting stakeholder inputs are explored rather than prematurely resolved.

### User Input

Sales believes customers need more features, while Customer Support believes stability is the bigger issue. We don't know which direction to take.

### Expected Capability

Product Thinking

### Expected Artifact

Problem Statement

### Expected Behavior

- Capture both stakeholder perspectives.
- Identify areas of agreement and disagreement.
- Clarify the underlying product problem.

### Should Not

- Take sides.
- Recommend a solution.

### Success Criteria

- Presents the differing perspectives objectively.
- Produces a balanced Problem Statement.
- Recommends Evidence-Based Decision if additional evaluation is required.

### Failure Criteria

- Chooses one stakeholder's opinion without justification.
- Skips problem clarification.

---

# Anti Pattern

## PT-AP-001 — Request to Create Product Backlog Items

### Intent

Verify that the assistant does not perform Backlog Engineering while operating as Product Thinking.

### User Input

Please create Product Backlog Items for this feature.

### Expected Capability

Backlog Engineering

### Expected Behavior

- Recognize that the request belongs to another capability.
- Recommend switching to Backlog Engineering.

### Should Not

- Produce Product Backlog Items while remaining in Product Thinking.

### Success Criteria

- Routes to the correct capability.

### Failure Criteria

- Creates Product Backlog Items.

---

## PT-AP-002 — Request to Design an Increment

### Intent

Verify that the assistant does not perform Increment Design while operating as Product Thinking.

### User Input

Please design the next Increment for our product.

### Expected Capability

Increment Design

### Expected Behavior

- Recognize the requested capability.
- Recommend Increment Design.

### Should Not

- Produce an Increment Specification.

### Success Criteria

- Routes to Increment Design.

### Failure Criteria

- Produces an Increment Specification.

---

## PT-AP-003 — Request for an Implementation Solution

### Intent

Verify that the assistant avoids prescribing implementation details before the product problem is understood.

### User Input

Our retention is dropping. Tell us exactly what feature we should build.

### Expected Capability

Product Thinking

### Expected Behavior

- Explain that the product problem should be understood first.
- Continue Product Thinking.

### Should Not

- Recommend implementation.
- Suggest technical solutions.

### Success Criteria

- Maintains Product Thinking.
- Refocuses the conversation on understanding the problem.

### Failure Criteria

- Recommends a feature or implementation immediately.
