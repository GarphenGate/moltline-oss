---
name: calendar-healthcheck
description: One pasted week in, one blunt verdict out on how sick the calendar is and where it hurts most; use as the fast first look before any deeper surgery.
version: 1.0.0
---

# Calendar Health Check

*Free gateway skill from the Calendar Surgeon bundle by GarphenGate.*

The two-minute triage: paste a week, get a diagnosis and the single most urgent intervention.

## Procedure

1. **Take one pasted week** in any format. Ask only one clarifying question at most (usually: "which of these are recurring?").
2. **Compute four vitals**: meeting hours as % of working hours; longest unbroken focus stretch; number of context switches per day (distinct meeting topics); % of meetings with no stated purpose visible.
3. **Grade each vital** green / yellow / red against honest thresholds (meetings >60% of hours: red; longest focus stretch <90 min: red; >6 switches/day: yellow at best).
4. **Name the primary ailment** in one plain sentence ("Your week has no stretch long enough to think in").
5. **Prescribe exactly one next step** — the highest-leverage single move, not a program.

Output contract:

```
CALENDAR HEALTH CHECK — week of <date>
Meeting load: X% [G/Y/R]
Longest focus stretch: Xh [G/Y/R]
Context switches/day: X [G/Y/R]
Purposeless meetings: X% [G/Y/R]
Diagnosis: <one sentence>
Do this first: <one move>
```

## Rules

- Never soften a red to a yellow to be kind; the free skill's only job is an honest reading.
- Never prescribe more than one action; a triage that ends in a program is a sales pitch, not a diagnosis.
- If the week pasted is atypical (user says so, or it's a holiday week), say the verdict is provisional and ask for a normal week.
- State assumptions when the paste lacks working-hours context (default: 40-hour week).

## Degradation

If the paste is unreadable or partial, compute whichever vitals survive, mark the rest NO DATA, and still deliver a diagnosis scoped to what was measurable.

---

*Like this? The full **Calendar Surgeon** bundle adds the persona plus Calendar Audit, Meeting Diet, Block Scheduler — on Claw Mart.*
