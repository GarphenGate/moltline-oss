---
name: title-tester
description: Rank five candidate titles for the creator's next video with reasons; use whenever a video is done but the title is still a working title.
version: 1.0.0
---

# Title Tester

*Free gateway skill from the YouTube Strategist bundle by Hankash.*

Five titles for the next video, ranked with reasons, so the working title never becomes the published one by default.

## Procedure

1. **Get the video in two sentences**: what happens in it, and what the viewer walks away with. Ask for the channel's niche if unknown.
2. **Extract the promise** the strongest version of this video can honestly make.
3. **Write five titles from five different click logics** (curiosity gap, stakes, specificity, outcome, contrast); include the creator's own working title as a sixth entry if they shared one.
4. **Rank all entries** by promise strength, clarity at a glance, and honesty against the described video. Give a one-line reason per rank, and say plainly if the working title beat the alternatives.
5. **Flag thumbnail interaction**: for the top pick, note the one thing the thumbnail should show that the title doesn't say.

## Output

```
VIDEO: <two sentences> / PROMISE: <one sentence>
1. "<title>" [<logic>] — <why it ranks here>
2. ...
(working title ranked at #<n>)
TOP PICK THUMB NOTE: <what the thumbnail adds>
```

## Rules

- Never rank a title above others when the video can't keep its promise; honesty outranks click appeal in every tie.
- Never flatter the working title; if it ranks last, it ranks last with the reason stated.
- Five fresh options, five different logics; near-duplicates are collapsed before ranking.

## Degradation

Given only a topic and no description of the actual video, rank on promise strength alone and mark every entry HONESTY UNVERIFIED with a note to re-check against the final cut.

---

*Like this? The full **YouTube Strategist** bundle adds the persona plus Title & Thumbnail Ideator, Series Planner, Analytics Readbacker — on Claw Mart.*
