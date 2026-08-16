---
name: okr-grader
description: Paste your existing OKRs and get a hard critique of vague, sandbagged, or fantasy ones; use before the quarter locks, while rewrites are still free.
version: 1.0.0
---

# OKR Grader

*Free gateway skill from the OKR Navigator bundle by Hankash.*

Paste the OKRs you have. Get back the ones a tough friend would let you keep, and the rewrite for each one they wouldn't.

## Procedure

1. **Parse the paste.** Separate objectives from key results, tolerating any format. Mismatched structures (KRs with no parent, objectives with no KRs) get noted as structural findings.
2. **Grade every key result** against five checks: NUMBER (is there a measurable target?), BASELINE (is the starting point stated or known?), SOURCE (is it clear where the number gets read?), HONESTY (50/50 odds, neither sandbag nor fantasy: judged from the user's answers if unclear, and asked), OUTCOME (does it measure changed reality or just shipped output?).
3. **Grade each objective** on two checks: does it describe a changed state rather than a task list, and would its KRs landing actually mean the objective happened (the coherence check)?
4. **Issue verdicts:** KEEP (passes), REWRITE (fails 1-2 checks; provide the rewritten version, preserving the user's intent), CUT (fails 3+ or duplicates another; say what to do instead). Every REWRITE includes the concrete rewrite, not just the complaint.
5. **Summarize the pattern** in two lines: the dominant failure mode across the set (usually all-outputs or no-baselines) and the single highest-value fix.

## Output

```
OKR CRITIQUE
O1: <verdict> — <one line>
  KR1.1: <KEEP|REWRITE|CUT> — fails: <checks> 
    rewrite: "<new KR with number, baseline, source>"
STRUCTURAL: <orphan KRs, KR-less objectives>
PATTERN: <dominant failure mode>
HIGHEST-VALUE FIX: <one line>
```

## Rules

- Never soften a verdict to be kind; the kindness is the rewrite that comes with it.
- Never rewrite a KR into something the user didn't mean; rewrites preserve intent and fix measurability, and ambiguous intent gets a question instead.
- Must not pass a KR on charm; "launch the redesign" fails NUMBER and OUTCOME no matter how good the redesign sounds.

## Degradation

If the paste is a goals list with no OKR structure, grade it as raw ambitions: apply the NUMBER/OUTCOME checks anyway, and return a starter OKR structure built from the two strongest items, labeled STARTER DRAFT.

---

*Like this? The full **OKR Navigator** bundle adds the persona plus OKR Drafter, Check-in Cadence, Quarter Scorer — on Claw Mart.*
