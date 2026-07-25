# Experiment Design Tests

This document defines the expected behavior of the Experiment Design capability.

---

# Happy Path

## ED-HP-001 — Design an Experiment to Validate a Hypothesis

### Intent

Design an experiment to validate a product hypothesis.

### User Input

We believe simplifying the onboarding process will improve user activation, but we need evidence before committing to implementation.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Identify the hypothesis.
- Define the learning objective.
- Select an appropriate experiment.
- Define measurable success criteria.
- Produce an Experiment Charter.
- Recommend the next capability.

### Should Not

- Recommend implementation.
- Create Product Backlog Items.
- Design an Increment.

### Success Criteria

- Produces an Experiment Charter.
- Defines a measurable hypothesis.
- Defines clear success criteria.
- Recommends the next capability.

### Failure Criteria

- Suggests implementation immediately.
- Omits measurable success criteria.
- Skips defining the hypothesis.

---

## ED-HP-002 — Select the Smallest Valuable Experiment

### Intent

Design the smallest experiment capable of reducing uncertainty.

### User Input

We are unsure whether users will use a new recommendation feature. We want the quickest way to learn.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Evaluate possible experiment approaches.
- Select the smallest useful experiment.
- Explain the learning objective.
- Produce an Experiment Charter.

### Should Not

- Recommend building the full feature.
- Recommend unnecessary work.

### Success Criteria

- Chooses an appropriately scoped experiment.
- Explains why the experiment is sufficient.
- Produces an Experiment Charter.

### Failure Criteria

- Recommends a large implementation.
- Ignores learning cost.

---

## ED-HP-003 — Define Success Metrics

### Intent

Design an experiment with measurable outcomes.

### User Input

We want to validate whether adding social login increases registration completion.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Define measurable success metrics.
- Define failure criteria.
- Produce an Experiment Charter.

### Should Not

- Leave success undefined.

### Success Criteria

- Success metrics are measurable.
- Failure criteria are explicit.

### Failure Criteria

- Uses vague success definitions.

---

## ED-HP-004 — Evaluate Experiment Cost

### Intent

Balance learning value against experimentation cost.

### User Input

Running a six-month pilot would provide excellent data, but we need a faster approach.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Evaluate experiment alternatives.
- Balance learning value and cost.
- Recommend the most appropriate experiment.

### Should Not

- Ignore experiment cost.
- Maximize learning regardless of effort.

### Success Criteria

- Explains the trade-off.
- Produces an Experiment Charter.

### Failure Criteria

- Recommends unnecessarily expensive experiments.

---

## ED-HP-005 — Reduce Decision Uncertainty

### Intent

Design an experiment that reduces decision uncertainty.

### User Input

We are uncertain whether customers value automated reporting enough to justify further investment.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Identify uncertainty.
- Define the learning objective.
- Design an appropriate experiment.
- Produce an Experiment Charter.

### Should Not

- Make the decision without experimentation.

### Success Criteria

- Produces an Experiment Charter.
- Clearly links the experiment to the uncertainty.

### Failure Criteria

- Skips defining the learning objective.

---

# Edge Case

## ED-EC-001 — Undefined Hypothesis

### Intent

Verify that the assistant requests clarification when no hypothesis is provided.

### User Input

Please design an experiment.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Ask for the hypothesis or learning objective.
- Explain why additional context is required.

### Should Not

- Invent assumptions.

### Success Criteria

- Requests clarification.

### Failure Criteria

- Designs an experiment without a learning objective.

---

## ED-EC-002 — Unmeasurable Success Criteria

### Intent

Verify that success criteria are made measurable.

### User Input

We want customers to like the feature more.

### Expected Capability

Experiment Design

### Expected Artifact

Experiment Charter

### Expected Behavior

- Recognize that success criteria are vague.
- Recommend measurable success metrics.

### Should Not

- Accept vague criteria.

### Success Criteria

- Converts vague outcomes into measurable metrics.

### Failure Criteria

- Leaves success criteria ambiguous.

---

# Anti Pattern

## ED-AP-001 — Request to Design an Increment

### Intent

Verify that implementation planning is delegated to Increment Design.

### User Input

Please design the next Increment.

### Expected Capability

Increment Design

### Expected Behavior

- Recommend switching to Increment Design.

### Should Not

- Produce an Increment Specification.

### Success Criteria

- Routes to Increment Design.

### Failure Criteria

- Designs an Increment.

---

## ED-AP-002 — Request to Create Product Backlog Items

### Intent

Verify that Product Backlog Items are delegated to Backlog Engineering.

### User Input

Please create Product Backlog Items for this experiment.

### Expected Capability

Backlog Engineering

### Expected Behavior

- Recommend Backlog Engineering.

### Should Not

- Produce Product Backlog Items.

### Success Criteria

- Routes to Backlog Engineering.

### Failure Criteria

- Creates Product Backlog Items.

---

## ED-AP-003 — Request to Make a Product Decision

### Intent

Verify that decision making is delegated to Evidence-Based Decision.

### User Input

Based on this information, decide whether we should proceed.

### Expected Capability

Evidence-Based Decision

### Expected Behavior

- Recommend Evidence-Based Decision.

### Should Not

- Produce a Decision Recommendation while remaining in Experiment Design.

### Success Criteria

- Routes to Evidence-Based Decision.

### Failure Criteria

- Makes the decision directly.
