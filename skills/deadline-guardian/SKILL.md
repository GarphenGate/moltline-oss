---
name: deadline-lister
description: One list of everything due in the next 14 days, sorted by risk rather than by date; use Monday morning or any time the week feels ominous.
version: 1.0.0
---

# Deadline Lister

*Free gateway skill from the Deadline Guardian bundle by GarphenGate.*

Fourteen days of obligations on one screen, sorted by which ones can actually hurt you.

## Procedure

1. **Sweep for dates** from whatever the user provides: task lists, calendar pastes, email fragments, memory. Prompt once for the classic hiding places: invoices due, client review windows, renewals, and promises made on calls.
2. **Normalize each item:** deliverable, who it is for, date, and days remaining. Ambiguous dates ("end of next week") get pinned to the earliest plausible day and marked ASSUMED.
3. **Risk-sort, not date-sort.** Score each item by consequence of missing (client trust, money, legal/renewal lockout, internal only) crossed with readiness (done, in motion, not started). A not-started client deliverable in 6 days outranks a nearly-done one due tomorrow.
4. **Render three bands:** DANGER (high consequence, low readiness), WATCH (one of the two), FINE (in motion or low consequence). Within bands, order by date.
5. **Cap the commentary.** One line per item, and one closing line naming the single item to start today.

## Output

```
NEXT 14 DAYS — <date>
DANGER:
- <deliverable> — <for whom> — due <date> (<n>d) — not started
WATCH: <same shape>
FINE: <deliverable> — <date>
ASSUMED DATES: <items needing confirmation>
START TODAY: <the one item>
```

## Rules

- Never sort purely by date; the whole point is that the scariest item is often not the nearest one.
- Never drop an ambiguous date; pin it early, mark it ASSUMED, and list it for confirmation.
- Must not name more than one START TODAY item; two urgent starts is a triage failure, not a plan.

## Degradation

With nothing to sweep, build the list by interview: "walk me through each client, then internal obligations, then anything with a renewal or expiry." Mark the result FROM MEMORY and recommend a five-minute check against email before trusting the FINE band.

---

*Like this? The full **Deadline Guardian** bundle adds the persona plus Commitment Tracker, Workload Forecaster, Renegotiation Drafter — on Claw Mart.*
