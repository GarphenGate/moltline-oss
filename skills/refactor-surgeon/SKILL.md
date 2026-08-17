---
name: smell-checklist
description: A 10-point pass that grades any file's structural health in minutes. Use when reviewing unfamiliar code, prioritizing cleanup, or sanity-checking your own module before review.
version: 1.0.0
---

# Smell Checklist

*Free gateway skill from the Refactor Surgeon bundle by GarphenGate.*

Grade any file's structural health with a fixed 10-point pass — fast, repeatable, and honest about what matters.

## Procedure

1. Take one file (pasted or described). If given a whole directory, ask the user to pick one file; the checklist is per-file by design.
2. Score each of the ten points as pass, flag, or fail, with a one-line reason quoting the code:
   functions do one job; file has one reason to change; no duplicated logic blocks; names say what things are; no dead or commented-out code; dependencies point one direction; error paths are handled, not swallowed; no magic values without names; state is as local as possible; a newcomer could explain the file in two minutes.
3. Weight the grade by change frequency if known: fails in hot files matter, fails in frozen files mostly do not.
4. Emit the scorecard below.

Scorecard format:

```
SMELL CHECKLIST: <file> — grade: <A-F>
 1. One job per function        pass|flag|fail — <reason>
 ...
10. Two-minute explainability   pass|flag|fail — <reason>
Top fix: <the single change that raises the grade most>
```

## Rules

- Never fail a point without quoting or citing the specific code that fails it.
- Never let the grade imply the file must be fixed; the Top fix line plus change frequency carries the recommendation.
- One file per pass; comparative audits are a different job.

## Degradation

If the file is too large to read in full, grade the largest two functions plus the file's imports and say the grade covers only what was read.

---

*Like this? The full **Refactor Surgeon** bundle adds the persona plus Refactor Planner, Smell Detector, Strangler Guide — on Claw Mart.*
