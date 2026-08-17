---
name: followup-drafter
description: Draft a complete quote follow-up sequence in your agency's voice from one quote's details; use right after any quote goes out.
version: 1.0.0
---

# Follow-up Drafter

*Free gateway skill from the Insurance Agency Aide bundle by GarphenGate.*

One open quote in, four polite touches out — day 3, 8, 15, and 30 — in your agency's voice, each with one clear ask.

## Procedure

1. **Collect the quote facts:** client first name, line of business, date quoted, and the licensed agent's name. Ask for a sample of the agency's writing if available, to match register.
2. **Draft the four-touch sequence:** day 3 confirms receipt and invites questions for the agent; day 8 offers a walkthrough call with the agent; day 15 asks about timeline with an easy no; day 30 closes the file warmly, door open.
3. **Keep each touch under 90 words,** one question each, the quote date named in every message.
4. **Route substance:** any anticipated question about price, coverage, or comparison is handled by offering the agent's time — the drafts never answer those questions.
5. **Deliver the set with send dates** for the user's calendar; the user sends each one after review.

Output contract:

```
SEQUENCE — <client>, <line>, quoted <date>
DAY 3 (<send date>): <draft>
DAY 8 (<send date>): <draft>
DAY 15 (<send date>): <draft>
DAY 30 (<send date>): <draft>
```

## Rules

- Never include coverage opinions, product recommendations, or premium commentary — this is administrative follow-up; substance belongs to the licensed agent.
- Never send or schedule the messages; the user sends each after review.
- Never add touches beyond the four, and a client's "no" ends the sequence at the graceful close.

## Degradation

No writing sample: default to friendly-professional and say so, inviting one round of tone edits. Missing quote date: sequence from today with the age marked estimated.

---

*Like this? The full **Insurance Agency Aide** bundle adds the persona plus Renewal Reminder, Quote Follow-up, Claims Checklister — on Claw Mart.*
