---
name: grocery-organizer
description: Turn meal plans and scattered scraps into one clean, deduplicated grocery list. Use before a grocery run or when notes and requests have piled up all week.
version: 1.0.0
---

# Grocery Organizer

*Free gateway skill from the Household Manager bundle by Hankash.*

Take the week's meal plan, the notes on the fridge, and three people's texts, and hand back one list that survives the store.

## Procedure

1. Collect every input the user has: a meal plan, pasted notes, half-remembered requests. Nothing needs to be pre-cleaned; scraps are the expected input.
2. Explode meals into ingredients with quantities scaled to the household size the user states.
3. Deduplicate across sources, summing quantities, and convert to buyable units (one 500g bag, not 380g of flour).
4. Run the pantry check: list the ten items most likely already owned and ask the user to strike what they have before finalizing.
5. Output the final list:

```
GROCERIES — <date>
Produce: <item, qty>
Dairy & eggs: ...
Meat & fish: ...
Pantry: ...
Frozen: ...
Household: ...
Check at home first: <struck items, kept visible>
```

## Rules

- Never drop an input item silently; anything ambiguous lands in the list with a question mark, not on the floor.
- Never substitute around an allergy or dietary need the user has stated; those constraints are absolute, and conflicts are flagged, not resolved quietly.
- Quantities scale from the stated household size; never guess servings without saying so.
- The pantry check is mandatory; a list that rebuys the cupboard is a failed list.

## Degradation

With no meal plan, build the list from the user's answers to three questions: what are you cooking, who's eating, what ran out this week.

---

*Like this? The full **Household Manager** bundle adds the persona plus Chore Rotation, Maintenance Scheduler, Shopping Lister — on Claw Mart.*
