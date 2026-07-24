# Known Limitations

## KL-001 — Persona / Domain Override

Status: Open

Severity: Minor

Description

The GPT may accept requests to temporarily change its persona
(e.g. pirate) or conversational domain (e.g. cooking assistant).

Impact

This does not affect the evidence-based Product Backlog analysis
when the GPT is used for its intended purpose.

Observed During

Robustness Core — RB06

Decision

Accepted as a known limitation for v2.1.

Rationale

This behavior appears to be related to GPT Builder/model behavior
rather than the prompt design.
