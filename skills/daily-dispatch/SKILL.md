---
name: top3-picker
description: Force-rank today's overgrown list down to three with a one-line reason each; use any morning the to-do list is longer than the day.
version: 1.0.0
---

# Top-3 Picker

*Free gateway skill from the Daily Dispatch bundle by GarphenGate.*

Twelve items, one day. This picks the three that count and says out loud what happens to the other nine.

## Procedure

1. **Take the list as-is:** pasted, typed, or dictated, any format. Number the items. No cleanup requested; messy input is the normal case.
2. **Ask the two anchor questions:** any hard deadline landing today, and any person blocked waiting on you? Items matching either get first claim on the three slots.
3. **Fill remaining slots** by consequence: for each candidate, one line on what happens if it waits until next week. The items whose one-liners describe real cost win the slots; "it would nag at me" loses to "the client invoice slips a month."
4. **State the reasons.** Each pick carries its one-line argument, so the user can veto with information. Accept vetoes gracefully: a veto swaps one item, with the swap recorded; it does not reopen the whole ranking.
5. **Sentence the rest** in one visible pass: LATER THIS WEEK (name the day), DELEGATE-OR-ASK (who), or ADMIT IT'S NOT HAPPENING (said kindly, recorded honestly). The unpicked items get closure, not limbo.

## Output

```
TOP 3 — <date>
1. <item> — because: <one line>
2. <item> — because: <one line>
3. <item> — because: <one line>
LATER: <item> → <day>
DELEGATE/ASK: <item> → <who>
NOT HAPPENING (honestly): <items>
```

## Rules

- Never pick four; the whole value is the refusal, and the skill holds the line even when asked nicely.
- Never rank without the blocked-person question; unblocking others beats personal preference and the user should see when that rule decides a slot.
- Must not leave any unpicked item without a sentence; limbo items return tomorrow as guilt, and guilt is not a productivity system.

## Degradation

Given no list at all, build one live: "tell me everything pulling at you today, fast, no order." Transcribe, then run the normal procedure on the transcript. Given one item, confirm it is genuinely the day's work and resist inventing two more to fill slots.

---

*Like this? The full **Daily Dispatch** bundle adds the persona plus Shutdown Ritual, Tomorrow Plan, Priority Stack — on Claw Mart.*
