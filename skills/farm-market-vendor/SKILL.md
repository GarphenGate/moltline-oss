---
name: signage-copy
description: Write three honest, stopping-power signs for your stand from what you're selling this week; use before any market day.
version: 1.0.0
---

# Signage Copy

*Free gateway skill from the Farm & Market Vendor bundle by Hankash.*

Three signs, three seconds each, all true. Tell this skill what you're selling and it writes the copy that makes shoppers stop.

## Procedure

1. **Ask for three products** the user wants signs for, with price and unit each, plus one true appealing fact per product (when picked, the variety, the story). Push once for the fact — it's the sign.
2. **Write each sign in the three-line format:** hook (the true specific), name with variety, price with unit stated plainly.
3. **Add a use-line to any unfamiliar item** — one concrete serving idea in under eight words.
4. **Check the claims:** any certification word the user typed (organic, certified) gets a confirm question before it appears on a sign; unconfirmed, it's replaced with the true fact that needs no certificate.
5. **Return all three signs** in chalkboard-length versions, ready to write out.

Output contract:

```
SIGNS — <market/date>
1. <product>: HOOK <line> / <name, variety> / $<amt> per <unit> [use: <idea>]
2. ...
3. ...
CLAIMS: <certified terms: confirmed / replaced with <true fact>>
```

## Rules

- Never print a certification or claim word without the user confirming it's true and theirs to use; the sign gets the honest fact instead.
- Never write health or nutrition claims — freshness, taste, and story do the selling.
- Never pad with generic praise; if the user can't name one true specific, the hook becomes a question back to them, because that answer is the sign.

## Degradation

Given products with no facts: return the three-line skeletons with hook prompts ("picked when? variety name? first of season?") and the note that one true specific outsells any adjective.

---

*Like this? The full **Farm & Market Vendor** bundle adds the persona plus Market Prepper, Signage Copywriter, CSA Newsletter — on Claw Mart.*
