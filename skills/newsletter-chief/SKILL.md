---
name: subject-line-tester
description: Rank five subject line variants with stated reasons rather than vibes; use right before every send, when the issue is done but the subject line is a shrug.
version: 1.0.0
---

# Subject Line Tester

*Free gateway skill from the Newsletter Chief bundle by Hankash.*

Five subject line variants for a finished issue, ranked with reasons a human can argue with, plus the preview text that completes each one.

## Procedure

1. **Read the issue first** (or its summary). The subject line is a promise; the tester must know what the issue can actually pay off.
2. **Generate five variants across mechanics**: plain-benefit statement, curiosity with payoff, specific number or detail, question the reader is asking themselves, and personal or story-led. All five must be honest about the contents.
3. **Pair each with preview text** that extends the promise instead of repeating the subject or leaking "View in browser".
4. **Rank all five** with a one-line reason each, judged against: match to this issue's actual strength, clarity at a phone-width glance, and fit with the user's past subject style if known. Reasons cite the issue, never generic "curiosity performs well" lore.
5. **Name the risk on the top pick** — every subject has one (too plain, too cute, over-promises) — so the user chooses with eyes open.

## Output

```
SUBJECT TEST — <issue title/date>
1. "<subject>" + preview: "<text>" — why ranked here: <reason>
... (5, ranked)
Top pick risk: <one line>
House style note: <fits past sends? one line>
```

## Rules

- Never write a subject line the issue cannot pay off; a great open rate on a broken promise raises the next issue's ignore rate.
- Never use fake urgency, fake personalization, or "RE:"/"FWD:" deception; these are banned regardless of performance.
- All-caps and multiple exclamation marks are out; one emoji at most, and only if the user's past sends use them.
- Rankings must cite the specific issue; a reason that could apply to any newsletter is not a reason.

## Degradation

With no issue text provided, ask for a two-line summary of the lead item and generate against that, marking the ranking LOW CONFIDENCE. With no history of past subject lines, skip the house-style ranking factor and note that A/B testing inside the user's platform is the real judge.

---

*Like this? The full **Newsletter Chief** bundle adds the persona plus Issue Planner, Curation Digester, Growth Prompter — on Claw Mart.*
