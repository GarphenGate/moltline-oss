---
name: exercise-a-day
description: Serve one small daily coding exercise at the learner's level with test cases and laddered hints. Use each day the learner checks in, or whenever they ask for today's exercise.
version: 1.0.0
---

# Exercise-a-Day

*Free gateway skill from the Coding Teacher bundle by Hankash.*

One exercise a day, sized for one sitting, pitched at the learner's level, with test-case examples, three laddered hints, and a solution that unlocks only after a real attempt.

## Procedure

1. **Serve at level.** One exercise matched to the learner's level and language. Rotate skill areas across the week (data shaping, conditionals, loops, strings, small design); every third day revisits an area they previously needed hints on.
2. **Spec by behavior.** State what to build plus 3 input/output examples that double as tests. One 'edge to consider' included, because the happy path is only half the exercise.
3. **Hold the ladder.** Three hints: nudge question, concept pointer, fragment-on-a-different-problem. Each requires a try at the previous rung. No solution before a genuine attempt.
4. **Review.** Check their code against the stated cases, probe one edge, and debug by questions if it breaks. Then unlock the reference solution for comparison; the learner names one difference.
5. **Track the streak.** Log solved level and hints used; three clean days moves the level up, repeated rung-3 days move it down. The level move is stated, not silent.

## Output contract

```
EXERCISE OF THE DAY — day <n> (<language>, level <level>)
Build: <behavior>
Cases: <input → output> x3
Edge to consider: <one case>
Hints: 3 available — attempt first.

DAY RESULT: <clean / hints used: n / walkthrough>
Your lesson: "<learner's one sentence>"
Streak: <n> · Level: <holds / up / down>
```

## Rules

- Never show the solution before an attempt or an explicit give-up, and a give-up still gets hint one offered first.
- Never serve an exercise resembling the learner's coursework or an active assignment; daily exercises are original.
- Keep it to one exercise sized under 30 minutes; appetite for more feeds tomorrow's pitch, not today's second serving.

## Degradation

No stated level or language: ask for the language, serve one easy and one medium probe on day one, and set the level from the attempts. Learner can't run code today: swap in a trace-and-predict exercise at the same level, streak intact.

---

*Like this? The full **Coding Teacher** bundle adds the persona plus Concept Ladder, Exercise Generator, Learner Code Reviewer — on Claw Mart.*
