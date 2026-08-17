---
name: readme-grader
description: Paste a README and get the three fixes that most improve a stranger's first five minutes. Use before publishing a repo or when onboarding feedback says setup is confusing.
version: 1.0.0
---

# README Grader

*Free gateway skill from the Docs Engineer bundle by GarphenGate.*

Grade a README the way a stranger experiences it, then name the three fixes that matter most.

## Procedure

1. Read the pasted README top to bottom exactly once, as a first-time visitor would, noting where understanding or momentum breaks.
2. Score five dimensions, each pass, flag, or fail with a quoted reason: what-is-this clarity in the first screen; a copy-pasteable quickstart; prerequisites stated before they bite; expected output or success signal shown; troubleshooting for the likely failures.
3. Simulate the five-minute test mentally: at which step does a stranger on a clean machine stall first? That stall point anchors fix number one.
4. Pick exactly three fixes, ranked by how much stranger-time each saves. Rewrite the single worst passage as a before and after sample.
5. Emit the grade card below.

Grade card:

```
README GRADE: <A-F> — a stranger's first stall: <step/section>
Dimensions: what-is-this <p|f> | quickstart <p|f> | prereqs <p|f> | success signal <p|f> | troubleshooting <p|f>
Top 3 fixes:
  1. <fix — time it saves>
  2. ...
  3. ...
Rewrite sample: <worst passage, before -> after>
```

## Rules

- Never list more than three fixes; a ten-item critique produces zero edits.
- Never grade on completeness for its own sake; a short README that gets a stranger running beats a wiki that doesn't.
- Quote the README for every fail; critique without evidence is opinion.

## Degradation

If given a repo link but no README text, ask for a paste; if given a fragment, grade only the dimensions the fragment can show and mark the rest not-assessable.

---

*Like this? The full **Docs Engineer** bundle adds the persona plus README Writer, API Doc Writer, Runbook Writer — on Claw Mart.*
