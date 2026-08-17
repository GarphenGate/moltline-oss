---
name: meeting-master
description: Estimate what a recurring meeting really costs in attendee-hours and money, and judge whether it earns it; use before accepting or renewing any recurring invite.
version: 1.0.0
---

# Meeting Cost Counter

*Free gateway skill from the Meeting Master bundle by GarphenGate.*

Put a price tag on the recurring meeting and then ask the only question that matters: would you buy this outcome at this price?

## Procedure

1. **Collect the inputs:** attendee count, duration, frequency, and (optionally) a rough average hourly cost. If the user declines to estimate cost, use attendee-hours alone; never insist on salary data.
2. **Compute the bill:** attendee-hours per occurrence, per month, per year; multiply by hourly cost if provided. Show the arithmetic in one line so it is checkable.
3. **Audit the return.** Ask what the meeting produced in its last three occurrences: decisions, unblocked work, or coordination that prevented a concrete problem. "Alignment" without an example counts as nothing.
4. **Render a verdict:** EARNS IT (keep as is), RESTRUCTURE (halve duration, halve frequency, or cut the attendee list; state which and why), or KILL (recommend cancellation with a one-line replacement, usually a doc or an async update).
5. **Draft the change note** if the verdict is RESTRUCTURE or KILL: two sentences the user can send to attendees, framed on respect for their time.

## Output

```
MEETING COST — <meeting>
BILL: <n> people x <m> min x <freq> = <hours>/yr (~$<x>/yr if cost given)
RETURN (last 3): <what it produced, or "nothing concrete">
VERDICT: EARNS IT | RESTRUCTURE (<change>) | KILL (replace with <alternative>)
DRAFT NOTE: "<two sentences>"
```

## Rules

- Never inflate or guess salary figures; without user-provided cost, report attendee-hours only.
- Never verdict KILL on a meeting the user does not own without framing the draft as a proposal to the owner.
- "It's always been on the calendar" is not a return; verdicts rest on produced outcomes only.

## Degradation

If the user cannot recall what the last three occurrences produced, that fact is itself the finding: verdict RESTRUCTURE at minimum, and suggest attending the next occurrence with a one-line log to settle the question.

---

*Like this? The full **Meeting Master** bundle adds the persona plus Agenda Builder, Minutes Writer, Action Tracker — on Claw Mart.*
