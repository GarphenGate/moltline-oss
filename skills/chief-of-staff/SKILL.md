---
name: standup-summarizer
description: "Turn rough notes into a crisp yesterday/today/blockers update; use before a standup, an investor ping, or any moment someone asks what you have been doing."
version: 1.0.0
---

# Standup Summarizer

*Free gateway skill from the Chief of Staff bundle by Hankash.*

From messy notes to a standup update that sounds like someone in control, in under a minute.

## Procedure

1. **Take the raw material.** Accept notes in any form: bullet fragments, a commit log, a stream-of-consciousness paragraph. Do not ask for cleanup; cleanup is the job.
2. **Sort into three buckets.** Yesterday (done, past tense, shipped things first), Today (intent, max three items), Blockers (things waiting on someone else, named).
3. **Compress.** One line per item. Cut process narration ("spent time looking into...") in favor of outcomes ("chose X over Y").
4. **Flag the gap.** If the notes show work but no shippable outcome, say so honestly rather than inflating; "investigated three approaches, decision tomorrow" is a legitimate line.
5. **Return the update** ready to paste, in the founder's register: plain, confident, no filler.

## Output

```
YESTERDAY: <done items, one line each>
TODAY: <max 3 intents>
BLOCKERS: <item — who/what it waits on, or "none">
```

## Rules

- Never invent work that is not in the notes; an inflated standup is a debt that comes due.
- Never list more than three items under TODAY; a ten-item today is a plan to disappoint.
- Blockers name a person or dependency, not a mood; "stuck" is not a blocker, "waiting on Stripe support since Tuesday" is.

## Degradation

Given no notes at all, ask three questions (what shipped? what is next? what is stuck?) and build the update from the answers. Given only a commit log, derive Yesterday from it and leave Today for the user to fill by prompt.

---

*Like this? The full **Chief of Staff** bundle adds the persona plus Morning Briefing, Task Triage, Meeting Prep — on Claw Mart.*
