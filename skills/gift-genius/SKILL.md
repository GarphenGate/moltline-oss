---
name: gift-genius
description: Build the master list of birthdays, anniversaries, and dates the user must not miss. Use once to set up, then whenever a new person or date enters the picture.
version: 1.0.0
---

# Occasion Calendar

*Free gateway skill from the Gift Genius bundle by GarphenGate.*

The one-time sweep that turns 'I'm bad with dates' into a list that does the remembering.

## Procedure

1. Sweep in rings, inside out: household, immediate family, closest friends, extended family that expects a call, colleagues and mentors, then annual occasions that aren't people (anniversaries, memorials the user observes).
2. For each entry capture: name, occasion, date, and the gesture tier the user assigns (gift / card / call / message).
3. Catch the traps explicitly: ask about the dates people feel worst about missing — anniversaries of loss where the user prefers to reach out, kids' birthdays where the gift really goes to the household, and occasions that moved (rescheduled weddings, adopted-day celebrations).
4. Output the master calendar:

```
OCCASION CALENDAR — <n> entries, built <date>
<Month>
- <day> — <person> — <occasion> — tier: <gift|card|call|message>
Unknown dates to hunt down: <people the user wants listed but can't date yet>
```

5. Close with the two follow-ups: where the user will keep this list visible, and the offer to add act-by lead times via Occasion Tracker.

## Rules

- Never guess a date; anyone the user can't date goes to the hunt-down list, and a wrong birthday is worse than a missing one.
- Never assign gesture tiers on the user's behalf; the tier is their call per entry, made explicitly.
- Never treat the calendar as finished; every readout ends by asking if anyone new belongs on it.
- Sensitive dates (losses, estrangements) are recorded exactly as the user words them and never elaborated on.

## Degradation

If the user stalls on the full sweep, capture just ring one (household and immediate family) as a complete, usable calendar, and leave the outer rings as a named next session rather than an unfinished list.

---

*Like this? This is the free gateway skill for **Gift Genius** by Moltline Studio. The paid listing: https://www.agensi.io/skills/gift-genius-bundle*
