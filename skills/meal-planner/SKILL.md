---
name: dinner-decider
description: Three tonight-ideas built from what's already in the kitchen, decided in two minutes. Use at 5pm on any day the plan didn't survive.
version: 1.0.0
---

# Dinner Decider

*Free gateway skill from the Meal Planner bundle by GarphenGate.*

It's 5pm, there's no plan, and takeout is circling. Name what's in the kitchen; get three real options.

## Procedure

1. Ask one question: what's actually in the fridge and pantry right now? Accept a messy list; that's the expected input. Note the time available and who's eating.
2. Generate exactly three options from what's named, no shopping allowed:
   - Fastest: on the table in 15 minutes or less.
   - Best use: the option that rescues whatever is closest to expiring.
   - Most satisfying: the one worth the extra 15 minutes tonight.
3. Present them tight:

```
TONIGHT — from your kitchen
1. FASTEST (<mins>): <meal> — <two-line method>
2. BEST USE (<mins>): <meal> — uses up <the at-risk item>
3. WORTH IT (<mins>): <meal> — <two-line method>
Missing exactly one thing? <the single substitution that unlocks a fourth option>
```

4. When the user picks, expand that option into short numbered steps sized to their stated time.
5. If the named ingredients genuinely can't make dinner, say so honestly and name the smallest single purchase that fixes it.

## Rules

- Never require an ingredient the user didn't name; substitutions are offered, not assumed into the plan.
- Never attach virtue or guilt to any option; the 15-minute quesadilla and the 40-minute effort are morally identical dinners.
- Respect stated allergies and dietary needs in all three options, every time.
- Three options is the contract; never present five, and never present one.

## Degradation

If the user won't inventory, ask for just three things: a protein or can they have, a carb they have, and one vegetable in any state. Build the three options from those.

---

*Like this? The full **Meal Planner** bundle adds the persona plus Weekly Menu, Grocery Consolidator, Batch-Cook Planner — on Claw Mart.*
