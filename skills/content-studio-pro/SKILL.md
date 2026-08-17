---
name: content-studio-pro
description: Generate ten scroll-stopping openings for any topic, spread across distinct hook mechanics; use before drafting any post, script, or headline when the opening line is the blocker.
version: 1.0.0
---

# Hook Generator

*Free gateway skill from the Content Studio Pro bundle by GarphenGate.*

Ten real openings for one topic, each built on a different mechanic, so the user picks by fit instead of settling for the first line that came out.

## Procedure

1. **Pin the topic and the reader.** One sentence each: what the piece says, and who is scrolling past it. If the user gives only a topic, ask for the audience or infer it and say so.
2. **Draft ten hooks across mechanics**, at least six of these covered: bold claim, specific number or result, open question, mistake-warning, before/after contrast, story cold-open, counterintuitive statement, direct callout of the reader's situation.
3. **Keep each hook honest.** Every hook must be a promise the actual piece keeps; a hook the content cannot pay off is cut and replaced.
4. **Rank the top three** with one line of reasoning each, tied to the stated audience, not to generic engagement lore.
5. **Offer one refinement pass**: the user picks a hook, the skill produces three tighter variants of that one mechanic.

## Output

```
HOOKS — <topic> for <audience>
1. [claim] <hook>
2. [number] <hook>
... (10 total, mechanic labeled)
Top 3: #<n> — <why it fits this audience>, #<n> — <why>, #<n> — <why>
```

## Rules

- Never write a hook the piece cannot pay off; curiosity-gap bait with no payoff is banned even when it would perform.
- Never invent statistics or fake specificity ("97% of creators...") to make a hook stronger; use the user's real numbers or none.
- No more than two hooks per mechanic in the ten; variety is the product.
- Must not rank by vibes; every ranking reason names the audience it fits.

## Degradation

With no audience given and no way to infer one, generate the ten against two contrasting audience guesses (five each), label the split, and ask the user which reader is real. With a topic too broad to hook ("marketing"), narrow it to three concrete sub-angles first and hook the one the user picks.

---

*Like this? The full **Content Studio Pro** bundle adds the persona plus Blog Pipeline, Short-form Repurposer, Newsletter Builder — on Claw Mart.*
