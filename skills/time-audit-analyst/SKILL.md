---
name: time-log-template
description: Set up the lightest time-tracking format that still supports leak-finding and utilization math; use when starting tracking or after abandoning a heavier system.
version: 1.0.0
---

# Time Log Template

*Free gateway skill from the Time Audit Analyst bundle by Hankash.*

Five fields, thirty seconds an entry — the minimum that still lets the analysis work later.

## Procedure

1. **Ask three setup questions**: where will entries live (spreadsheet, notes app, tracker), how does the user bill (hourly, fixed-fee, mixed), and what are the 3-7 buckets work actually falls into?
2. **Issue the template** with the five fields that survive every failed tracking system: date, client/project, bucket, duration to the quarter hour, and a note with one concrete noun ("revised pricing section", not "work").
3. **Add the billable flag** as written for their billing model — hourly users mark billable yes/no; fixed-fee users mark in-scope/over-scope, which is what makes creep visible later.
4. **Set the capture ritual**: entries at natural breaks or a 5-minute end-of-day sweep, whichever the user will actually do. Same-day capture is the one non-negotiable; reconstructed weeks are fiction.
5. **Show one filled example day** in their format, using their buckets.

Output contract:

```
TIME LOG — <name>
date | client/project | bucket | hours (0.25) | in-scope? | note (one concrete noun)
Example:
2026-08-10 | Acme | delivery | 1.5 | yes | drafted audit findings deck
2026-08-10 | internal | admin | 0.5 | - | invoicing run
Buckets: <their 3-7>
Ritual: <their chosen capture moment>
Review: after 2 full weeks — then the log can be analyzed
```

## Rules

- Never add fields beyond the five plus the flag; every extra field costs adoption and adds nothing the analysis needs.
- Never let bucket count pass seven; more buckets means slower entries and mushier data.
- Quarter-hour precision is the floor and the ceiling; six-minute increments belong to law firms and abandoned systems.
- If the user's last three tracking attempts died, say plainly that the ritual matters more than the tool, and set the smallest ritual they'll keep.

## Degradation

If the user resists per-entry logging entirely, fall back to the end-of-day three-line version (top client hours, other hours, one note) and be honest about what it buys: utilization math yes, leak-finding only partially.

---

*Like this? The full **Time Audit Analyst** bundle adds the persona plus Timesheet Analyst, Billable Leak Finder, Utilization Report — on Claw Mart.*
