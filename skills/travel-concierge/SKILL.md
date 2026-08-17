---
name: travel-concierge
description: Generate a trip-specific packing list from destination, duration, and planned activities. Use once a trip is booked or whenever the user says they need to pack.
version: 1.0.0
---

# Packing List

*Free gateway skill from the Travel Concierge bundle by GarphenGate.*

A packing list built from this trip, not from a generic template with 90 items you'll ignore.

## Procedure

1. Ask for the minimum: destination, dates, planned activities, and how the user travels (carry-on only or checked, laundry access or not).
2. Derive the drivers: expected weather range for those dates (stated as an estimate to verify against a forecast), dress codes any activity implies, and the laundry cycle that sets clothing counts.
3. Produce the list grouped and counted:

```
PACKING — <destination>, <n> days
Clothing (laundry every <n> days): <item x count>
Footwear: ...
Toiletries & meds: your usual prescriptions and toiletries — count the days
Documents & money: <what to carry, what to photograph>
Tech & chargers: ...
Activity-specific: <per planned activity>
Leave behind: <the 3 things people pack for this trip and never use>
```

4. Flag anything that must be bought before departure with a buy-by date.
5. Offer one compression pass on request: what to cut to go carry-on only.

## Rules

- Never pad the list; every item ties to the destination, dates, or a named activity.
- Never give medication or health advice beyond "pack your usual prescriptions and check them off"; specifics belong to the user's pharmacist or doctor.
- Weather is an estimate until checked against a forecast; say so on the list itself.
- The Leave-behind section is mandatory; a packing list that only adds is half a packing list.

## Degradation

Given only a destination, produce the seasonal baseline list with counts left as formulas (shirts = days until laundry + 1) and note which missing detail would firm each section up.

---

*Like this? The full **Travel Concierge** bundle adds the persona plus Trip Researcher, Itinerary Builder, Booking Prepper — on Claw Mart.*
