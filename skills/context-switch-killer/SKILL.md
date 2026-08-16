---
name: interrupt-capture
description: Park any incoming interruption in one line and return to flow in under ten seconds; use the moment a ping, thought, or 'quick question' lands mid-focus.
version: 1.0.0
---

# Interrupt Capture

*Free gateway skill from the Context-Switch Killer bundle by Hankash.*

The interrupt arrives either way. This decides in ten seconds whether it gets your next two hours.

## Procedure

1. **Run the one-question triage**: does this cost more than everything in the current flow block if it waits two hours? Almost always no. Genuinely yes (page, blocked teammate, hard deadline): take it — after a 10-second TRAP note of the current state.
2. **Park everything else in one line** on the park list: `<what> · <who's waiting, if anyone> · <park time>`. One line, no formatting decisions, no app-switching if a text file is closer.
3. **Say the return line if a human is waiting** — offered ready-made: 'On it after 12:00, ping me with BLOCKING if it can't wait.' Silence reads as ignoring; a stated time reads as a system.
4. **Return to the task immediately.** No 'quick peek' at the source of the interrupt; the peek is the switch.
5. **Drain the park list at the next batch window or day's end**: handle, schedule, or delete each line. A park list that only grows is a backlog wearing a disguise, and it kills trust in the ritual.

Output contract:

```
PARK — <time>
<what> · <who> · parked <time>
(return line sent: yes/no)
---
Drain (at window): handled / scheduled <when> / deleted — one verdict per line
```

## Rules

- Never spend more than ten seconds on the capture; if it needs a decision, the decision is 'park it' and the thinking happens at the drain.
- Never park on-call pages, emergencies, or a teammate who says BLOCKING; the triage question exists exactly so real urgency gets through fast.
- Never end the day with an undrained park list; parked items belong to the system only until the next window, then they get verdicts.
- The park list holds work items, not a record of who interrupts; it is never used as evidence against colleagues.

## Degradation

Mid-flow with no park list set up yet: use anything within reach — reply draft to self, paper, terminal comment — capture the one line, and set up the real list at the next window; the ritual matters, the container doesn't.

---

*Like this? The full **Context-Switch Killer** bundle adds the persona plus Batch Planner, Interruption Log, Re-entry Notes — on Claw Mart.*
