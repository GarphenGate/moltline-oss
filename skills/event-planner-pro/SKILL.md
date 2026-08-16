---
name: run-of-show-template
description: Turn an event's basic shape into a starter minute-by-minute show timeline; use for any event to see what a real run-of-show looks like.
version: 1.0.0
---

# Run-of-Show Template

*Free gateway skill from the Event Planner Pro bundle by Hankash.*

The show-day timeline that prevents chaos: every minute owned, every handoff cued. This skill builds the starter version from your event's basic shape.

## Procedure

1. **Ask for the anchors:** event date, doors-open, program start, hard end, venue, and the program's segments in order with rough lengths.
2. **Build backwards and forwards:** load-in and setup blocks before doors (defaults offered by event type — user's numbers win), segments with transition minutes between them, buffer before program start, strike after hard end.
3. **Add the owner column** filled with role names (venue lead, AV, MC, catering) as placeholders that must become real names and cell numbers before show day — flagged as such.
4. **Mark the fragile rows** — AV moments, speaker handoffs, food service, anything outdoor — with a fallback cell reading "plan B here" so the gaps are visible, not hidden.
5. **Return the timeline** with a completion checklist: names for roles, fallbacks written, venue times confirmed in writing.

Output contract:

```
RUN OF SHOW (starter) — <event>, <date>
| Time | Duration | Item | Owner (role - add name+cell) | Fallback |
COMPLETE BEFORE SHOW: [ ] real names+cells [ ] fallbacks on fragile rows [ ] venue times confirmed in writing
```

## Rules

- Never zero out transition or buffer minutes to make the program fit the window; show the overrun honestly and suggest what to trim.
- Never present venue access times as confirmed — they render as confirm-with-venue items until the user says they're in writing.
- Never fill the fallback column with invented plans; visible gaps are the point of the starter.

## Degradation

Given only a date and headcount, produce the generic skeleton for that event size with every row marked as an assumption to replace — a worksheet, labeled as one.

---

*Like this? The full **Event Planner Pro** bundle adds the persona plus Vendor Communicator, Run-of-Show Builder, Event Budgeter — on Claw Mart.*
