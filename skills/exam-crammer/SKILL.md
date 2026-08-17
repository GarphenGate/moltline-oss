---
name: study-plan
description: Produce a two-week exam study plan from a syllabus and an exam date in one pass. Use when an exam is about two weeks out and the student has no plan, only a syllabus and rising dread.
version: 1.0.0
---

# Study Plan

*Free gateway skill from the Exam Crammer bundle by GarphenGate.*

One pass from syllabus plus exam date to a two-week plan: weighted topics, daily blocks, and a retrieval-only final stretch.

## Procedure

1. **Take three inputs.** Exam date, syllabus or topic list, and honest hours per day. Ask for a self-rating (solid / shaky / weak) per topic; thirty seconds of honesty here shapes everything.
2. **Weight the topics.** Hours follow weakness times likely exam weight. If weights are unknown, mark them estimated. Name any topic worth sacrificing outright.
3. **Lay the fortnight.** Days 1-11: weighted topic blocks, each day ending with a 15-minute recall sweep. Days 12-14: retrieval and practice only, no new material.
4. **Add the slip rule.** State the one thing to cut if a day is lost, chosen now, not in the panic.
5. **Hand off.** Deliver in the contract format and point to where a scored practice test would sharpen the weights.

## Output contract

```
TWO-WEEK PLAN — <exam> (<h> hrs/day)
Weights: <topic: hours> ... | Sacrificed: <topics or 'none'>
Days 1-11: <per-day blocks + recall sweep topic>
Days 12-14: retrieval only — <what to drill>
Slip rule: lose a day → cut <pre-agreed item>
```

## Rules

- Never spread hours evenly across all topics; the plan exists to be unequal on purpose.
- Never schedule new material in the final three days.
- Never build in more daily hours than the student stated, and never remove sleep to make topics fit.

## Degradation

No syllabus: build from the student's from-memory topic list, flagged 'reconstruct from your course page and I re-plan'. More or less than two weeks out: compress or extend proportionally and keep the retrieval-only tail at roughly the final fifth.

---

*Like this? The full **Exam Crammer** bundle adds the persona plus Study Scheduler, Practice Tester, Weak-Spot Driller — on Claw Mart.*
