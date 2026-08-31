---
name: brand-voice-keeper
description: Reveal a brand's actual voice through five forced-choice questions with instant analysis; use at the very start of voice work, or to get a vague client saying concrete things about how they sound.
version: 1.0.0
---

# Voice Quiz

*Free gateway skill from the Brand Voice Keeper bundle by GarphenGate.*

Five forced-choice questions that make a vague brand say something concrete, then a one-page readout of the voice they actually chose — the fastest honest start to voice work.

## Procedure

1. **Ask five questions, one at a time**, each a forced choice between two rewritten versions of the same message (not abstract adjectives): an apology for downtime, a product announcement, a pricing explanation, a social reply to praise, a headline. Each pair contrasts one dimension: formality, warmth, humor, directness, plainness vs. flourish.
2. **Probe one choice.** After the five, ask one follow-up on the most revealing pick: "what made you choose that one?" The reason often matters more than the choice.
3. **Read out the result**: 3 named voice leanings with the evidence ("you picked the version that led with the fix, twice — this brand explains before it charms"), plus the tension if their picks conflicted, stated plainly.
4. **Translate to first rules**: three starter do/don't pairs derived directly from their picks, each with an example sentence.
5. **Name the next step**: these picks plus real writing samples become a full voice guide; the quiz is the doorway, not the destination.

## Output

```
VOICE QUIZ — <brand>
Picks: Q1 <A/B> ... Q5 <A/B> — probe: "<their reason>"
Leanings:
1. <leaning> — evidence: <which picks>
Tension: <conflict between picks, if any>
Starter rules:
DO <rule> — e.g. "<sentence>" / DON'T <rule> — e.g. "<sentence>"
Next: <what a full guide would add>
```

## Rules

- Never ask for adjectives ("are you playful or professional?"); every question is a forced choice between concrete sentences.
- Never smooth over contradictory picks; the tension is the most useful finding and gets stated, kindly.
- The readout cites the picks as evidence for every leaning; no leaning appears without its supporting choices.
- Must not present the quiz result as a finished voice guide; it is labeled a starting read, pending real samples.

## Degradation

With a user answering on a client's behalf who keeps saying "I'm not sure," switch to artifact mode: ask for any two pieces of the client's writing and run the quiz as predictions ("based on these, they'd pick A — agree?"). With no brand at all yet, run the quiz on the founder's natural writing voice and label the result founder-voice, the usual best seed.

---

*Like this? This is the free gateway skill for **Brand Voice Keeper** by Moltline Studio. The paid listing: https://www.agensi.io/skills/brand-voice-keeper-persona*
