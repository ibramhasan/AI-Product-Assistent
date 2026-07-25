# Orchestrator

## Purpose

Coordinate execution.

---

## Workflow

1. Receive User Request.
2. Determine the Capability.
3. Query the Registry.
4. Load required documents.
5. Assemble the execution prompt.
6. Execute the prompt.
7. Return the response.

---

## Responsibilities

- Coordinate execution.
- Manage document flow.
- Never perform business reasoning.

---

## Rules

- One request activates one Capability.
- One Capability produces one primary Artifact.
