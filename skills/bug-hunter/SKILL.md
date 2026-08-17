---
name: bug-hunter
description: Turn a vague 'it's broken' into a report a maintainer can act on. Use whenever a bug needs to be filed, handed off, or posted to an issue tracker.
version: 1.0.0
---

# Bug Report Formatter

*Free gateway skill from the Bug Hunter bundle by GarphenGate.*

Turn "it's broken" into a report a maintainer can act on without a follow-up question.

## Procedure

1. Extract three things from the user's description: what they did, what they expected, what happened instead. Ask targeted questions for whatever is missing, batched into one round.
2. Capture environment: app or library version, OS, runtime, relevant config. Mark unknowns as "unknown" rather than guessing.
3. Reduce the steps to the shortest numbered path that triggers the problem, and put exact error text in a fenced block, untrimmed.
4. Classify severity honestly: crash or data loss, broken feature, degraded behavior, or cosmetic.
5. Emit the format below, ready to paste into any issue tracker.

Report format:

```
Title: <symptom + component + condition, one line>
Environment: <versions, OS, runtime>
Steps to reproduce:
  1. ...
Expected: ...
Actual:
  <exact output or error, fenced>
Severity: <level> | Regression from: <version | unknown>
```

## Rules

- Never paraphrase error messages; exact text is the most searchable evidence in the report.
- Never include secrets, tokens, or personal data from logs; redact and note the redaction.
- One bug per report; a second symptom gets a second report.

## Degradation

If the user cannot answer environment or steps questions, ship the report with explicit "unknown" fields and a short list of what to add later, rather than holding the report hostage to completeness.

---

*Like this? The full **Bug Hunter** bundle adds the persona plus Repro Builder, Hypothesis Tracker, Root-Cause Writer — on Claw Mart.*
