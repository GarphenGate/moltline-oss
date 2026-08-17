---
name: life-admin-clerk
description: Surface every expiry date the household is currently gambling on, in one sitting. Use when the user wants to know what's expiring or has ever been burned by a lapsed document.
version: 1.0.0
---

# Renewals Lister

*Free gateway skill from the Life Admin Clerk bundle by GarphenGate.*

One guided sweep, one list: every expiry you're currently trusting to luck, sorted by how soon it bites.

## Procedure

1. **Run the sweep as a quick interview,** category by category: passports (everyone in the household), driving licenses, vehicle registration/inspection, insurance policy end dates, payment cards, professional certifications, and the subscriptions that auto-renew for real money. For each: expiry date if known, or 'unknown' — which is the finding.
2. **Sort the results into three bands:** RED (inside 6 months, or unknown for a critical document), YELLOW (6-18 months), GREEN (18+ months).
3. **Attach the honest note to each RED item:** typical processing time for that document type, marked 'typical — verify with the issuing office,' so the user sees why 'five months away' can mean 'start now.'
4. **End with the two-step exit:** tonight, find the unknowns in the documents drawer; this week, start the reddest item. Ongoing lead-time alerts, in-flight tracking, and application checklists are the paid Life Admin Clerk bundle.

Output contract — always produce this format:

```
RENEWALS — household sweep · <date>
RED: <item> — expires <date or UNKNOWN> — typical processing ~<time> [verify]
YELLOW: <item> — <date>
GREEN: <n> items, nearest <date>
UNKNOWNS TO FIND TONIGHT: <list>
THIS WEEK: start <reddest item>
```

## Rules

- Never soften an unknown critical date; 'unknown passport expiry' sits in RED until the date is found, because unknown is the riskiest status there is.
- Never present typical processing times as official; every one carries [verify] and the pointer to the issuing office.
- Never wander into advice about the documents' legal or coverage content; this list is dates, bands, and next steps only.

## Degradation

User is away from all documents: run the sweep on memory, mark everything approximate, and output the same list with 'confirm against the actual documents' as the standing first step.

---

*Like this? The full **Life Admin Clerk** bundle adds the persona plus Paperwork Tracker, Renewal Reminder, Document Checklister — on Claw Mart.*
