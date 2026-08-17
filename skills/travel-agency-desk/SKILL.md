---
name: travel-agency-desk
description: Format any trip's bookings into the day-by-day itinerary layout clients love to receive; use to see agency-polish structure on a real trip.
version: 1.0.0
---

# Itinerary Template

*Free gateway skill from the Travel Agency Desk bundle by GarphenGate.*

The format that makes clients feel handled: every day answers what happens, when, where, and who to call. This skill applies it to whatever trip details you paste.

## Procedure

1. **Take the raw trip:** bookings, notes, an email thread — any form. Extract dates, locations, and booked items into chronological order.
2. **Render the standard layout:** trip header (travelers, dates, agency contact), then one block per day — date and location, logistics lines with times in local time and confirmation numbers, a short what-to-expect note, and an if-something-goes-wrong contact line.
3. **Mark what's missing** rather than smoothing over it: unbooked segments render as GAP lines, unknown times as "confirm time," absent contacts as "add local contact."
4. **Keep the voice plain:** what the day holds in ordinary sentences, no brochure language.
5. **Return the formatted draft** for the user to complete and brand.

Output contract:

```
ITINERARY — <travelers>, <destination>, <dates>
DAY <n> — <date>, <location>
  <time (TZ)> — <item> (conf #<ref> | confirm time)
  Note: <one plain sentence>
  Contact: <name, phone | add local contact>
GAPS: <list>
```

## Rules

- Never invent times, confirmation numbers, or contacts to make the layout look complete — missing data renders as explicit markers.
- Never state visa or entry requirements; if the trip crosses borders, the header points the traveler to official sources.
- Never use brochure superlatives; the notes describe, they don't sell.

## Degradation

Given only a destination and dates, produce the empty day-by-day skeleton with markers throughout — useful as a worksheet, labeled as one.

---

*Like this? The full **Travel Agency Desk** bundle adds the persona plus Itinerary Drafter, Supplier Communicator, Trip Doc Packager — on Claw Mart.*
