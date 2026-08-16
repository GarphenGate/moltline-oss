---
name: notice-templates
description: Produce clean drafts of routine tenant notices like entry, rent reminders, and policy updates; use whenever a standard notice needs writing.
version: 1.0.0
---

# Notice Templates

*Free gateway skill from the Landlord Assistant bundle by Hankash.*

The routine notices — entry, rent reminder, policy update, quiet hours — written properly: calm, factual, dated, one topic each.

## Procedure

1. **Pick the notice type** from the routine set: planned entry/inspection, rent payment reminder, policy or rule reminder, utility or amenity interruption, move-out logistics. Anything involving eviction, deposits, habitability disputes, or lease termination is out of this skill's scope and gets an attorney-review flag instead of a draft.
2. **Collect the variables:** unit, tenant name, dates and time windows, the lease term the notice rests on (ask for the lease's actual language), and contact for questions.
3. **Draft it:** what, when, why in one sentence, what the tenant needs to do (if anything), and who to contact. Courteous, factual, under 150 words.
4. **Mark the confirm-items:** any line that depends on lease terms or local notice rules is bracketed for the user to verify before sending — entry-notice hours and lead times especially, since they vary by jurisdiction.
5. **Return the draft plus a one-line log entry** for the user's records.

Output contract:

```
NOTICE: <type> — Unit <n>
CONFIRM BEFORE SENDING: <lease/local items the user must verify>
---
<notice text, under 150 words>
---
LOG: <date> | <unit> | <notice type> | <effective date>
```

## Rules

- Never state notice periods, entry rules, or legal requirements as fact — they appear as confirm-items sourced to the user's lease and locality.
- Never draft eviction, lockout, or deposit-related notices; those get referred to the user's attorney.
- Never send anything; drafts only.

## Degradation

Missing lease language: the draft completes with the dependent line marked "confirm against your lease," and the notice is labeled not-ready-to-send until the user confirms.

---

*Like this? The full **Landlord Assistant** bundle adds the persona plus Tenant Communicator, Maintenance Dispatcher, Renewal Reminder — on Claw Mart.*
