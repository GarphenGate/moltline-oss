---
name: auto-shop-service-desk
description: Generate the five repair-status message templates every shop needs, in your shop's voice; use to set up proactive customer updates.
version: 1.0.0
---

# Status Templates

*Free gateway skill from the Auto Shop Service Desk bundle by GarphenGate.*

The five messages that stop phone tag: checked in, estimate ready, parts delay, ready for pickup, and follow-up. This skill writes them in your shop's voice, ready to reuse.

## Procedure

1. **Ask for the shop's basics:** name, how customers usually get updates (text or email), hours, and one sentence of how the counter actually talks — or a sample message to match.
2. **Draft the five templates** with slots marked in angle brackets: checked in (car's in, diagnosis timing, next contact time), estimate ready (it's ready, how to review and approve, invitation for questions), parts delay (what slipped, new date, next contact time), ready for pickup (total slot, hours, payment forms), day-after follow-up (everything good, reply if not).
3. **Hold the three-question standard in each:** where the car is, what happens next, when they'll hear from you — the third question is the phone-tag killer.
4. **Keep text versions under 300 characters** where the content allows; provide the email version where it doesn't.
5. **Return the set** with a one-line usage note per template — when it fires and what to fill in.

Output contract:

```
STATUS TEMPLATES — <shop name>
1. CHECKED IN: <template with <slots>>
2. ESTIMATE READY: ...
3. PARTS DELAY: ...
4. READY FOR PICKUP: ...
5. FOLLOW-UP: ...
Each: [use when: ...] [fill: <slots>]
```

## Rules

- Never include diagnostic language or urgency claims in a template — findings and urgency come from the tech per visit, not from boilerplate.
- Never write a template that omits the next-contact time; that line is the point.
- Never send messages; these are templates the shop fills and sends.

## Degradation

No voice sample: default to friendly-straight counter voice, label it a default, and offer one revision pass once the user pastes a real message they've sent.

---

*Like this? The full **Auto Shop Service Desk** bundle adds the persona plus Estimate Explainer, Status Updater, Review Requester — on Claw Mart.*
