---
name: language-tutor
description: Deliver one genuinely useful phrase each day with usage notes and a memory hook. Use at the start of the day, or whenever the learner asks for their daily phrase.
version: 1.0.0
---

# Phrase-a-Day

*Free gateway skill from the Language Tutor bundle by GarphenGate.*

One phrase a day, chosen for real-life usefulness, delivered with pronunciation, register, a memory hook, and a challenge to actually use it.

## Procedure

1. **Choose for usefulness.** Pick a phrase the learner could plausibly deploy this week, matched to their level and any stated interests. Rotate categories: social glue, survival, opinion, humor-safe.
2. **Present it whole.** The phrase, a natural translation (meaning, not word-by-word), a rough pronunciation guide, and a register flag: formal, neutral, or casual-only.
3. **Hook it.** One memory hook: an image, a sound-alike, or a link to a phrase the learner already has. One hook, not three.
4. **Set the challenge.** A concrete use-it task: drop it into today's conversation practice, or write one original sentence with it right now.
5. **Callback.** Tomorrow's delivery opens by asking for yesterday's phrase from memory before revealing today's.

## Output contract

```
PHRASE OF THE DAY — day <n> (<language>)
Phrase: <target-language phrase>
Means: <natural translation>
Sounds like: <rough pronunciation>
Register: <formal / neutral / casual-only> — <when to use, one line>
Hook: <one memory hook>
Challenge: <one concrete use-it task>
Yesterday's callback: can you still say "<meaning>"?
```

## Rules

- Never teach a phrase without its register; a casual phrase used formally is worse than silence.
- Never give word-by-word translations as the meaning; idioms get their real equivalent plus a literal note only if it helps the hook.
- Keep phrases age-appropriate and safe to use with strangers unless explicitly flagged otherwise.

## Degradation

Unknown level: default to high-frequency neutral-register phrases and ask one placement question with the first delivery. Learner missed days: resume with a two-phrase catch-up maximum; the streak restarts, the backlog does not avalanche.

---

*Like this? This is the free gateway skill for **Language Tutor** by Moltline Studio. The paid listing: https://www.agensi.io/skills/language-tutor-bundle*
