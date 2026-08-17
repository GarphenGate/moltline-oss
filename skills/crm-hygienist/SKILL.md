---
name: crm-hygienist
description: List every open deal with no activity in 14 or more days, ranked by value with days-silent attached; use as the Monday-morning two-minute pipeline truth serum.
version: 1.0.0
---

# Stale Deal Lister

*Free gateway skill from the CRM Hygienist bundle by GarphenGate.*

One paste, one ranked list of the deals going quietly cold.

## Procedure

1. **Take any export or paste** containing deal name, value, stage, and last activity date. Ask for nothing else; this is the two-minute version.
2. **Compute days silent** per open deal from last activity to today. If the data distinguishes inbound from outbound touches, use days since last inbound and say so; if not, note that true silence is probably longer than shown.
3. **Filter to 14+ days silent** and rank by deal value, descending — the expensive silence first.
4. **Annotate each entry** with one factual line: days silent, stage, and close date status (upcoming, this week, or already past).
5. **Total the cold value** and hand over the list with one closing question per top-three deal: 'what would reactivate this, and is it worth doing this week?'

Output contract:

```
STALE DEALS — <date> · threshold: 14 days
| # | Deal | Value | Stage | Days silent | Close date |
Cold pipeline total: $X across N deals (X% of open pipeline)
Top 3 worth a decision this week: ...
Note: <inbound/outbound caveat if applicable>
```

## Rules

- Never soften the days-silent number or exclude a big deal because it's somebody's favorite; the list is the list.
- Never recommend closing or killing anything here; this skill reports silence, and the close-or-work call belongs to the full cleanup with the human deciding.
- Deals past their close date get marked plainly, not quietly re-sorted to the bottom.
- The list touches no records and messages no prospects; it is a report, full stop.

## Degradation

Without last-activity dates in the export, fall back to deal age from created date, retitle the output OLD DEALS (age, not silence), and state clearly that activity data would make this list twice as useful.

---

*Like this? The full **CRM Hygienist** bundle adds the persona plus Pipeline Cleaner, Note Enricher, Next-Step Enforcer — on Claw Mart.*
