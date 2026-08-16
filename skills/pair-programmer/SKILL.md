---
name: rubber-duck-lite
description: Explain your problem once and get back the single question most likely to unblock you. Use when the user is stuck and wants a fast nudge rather than a full session.
version: 1.0.0
---

# Rubber Duck Lite

*Free gateway skill from the Pair Programmer bundle by Hankash.*

One paste, one question. The full Rubber Duck runs a session; this returns the single highest-leverage question and gets out of the way.

## Procedure

1. **Take the dump.** Accept the user's description of the problem in whatever shape it arrives: prose, code, error text, or all three.
2. **Locate the gap.** Find the difference between what the user expects and what is happening, and identify the least-verified assumption bridging that gap.
3. **Return exactly one question** aimed at that assumption, plus the two-minute check that would answer it, in the format below.
4. **If they answer,** either the answer exposes the flaw (say so plainly) or it eliminates that assumption; then return the next single question. Maximum three rounds before recommending the full Rubber Duck session.

```
THE QUESTION: <one question about the least-verified, highest-impact assumption>
Why this one: <one sentence>
2-minute check: <the concrete way to answer it>
```

## Rules

- Never return more than one question per round; the discipline is the product.
- Never propose a fix in this skill; unblocking is the job, solving is the user's.
- If the description lacks the expected-vs-actual gap, the one question is a request for exactly that, nothing else.
- After three rounds without movement, must not keep looping; hand off to a full structured session instead.

## Degradation

If the problem statement is a single vague sentence, the question becomes the sharpest possible clarifier: what did you expect, what happened instead, and where did you look; still one message, still no lecture.


---

*Like this? The full **Pair Programmer** bundle adds the persona plus Rubber Duck, Approach Comparer, Kata Coach — on Claw Mart.*
