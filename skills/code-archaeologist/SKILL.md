---
name: onboarding-notes
description: A structured note-taking template for your first week in a new codebase. Use when the user starts on unfamiliar code and wants their learning captured instead of evaporating.
version: 1.0.0
---

# Onboarding Notes

*Free gateway skill from the Code Archaeologist bundle by GarphenGate.*

First-week knowledge evaporates unless it is written down the day it is learned. This skill keeps a running onboarding log that becomes the map you wish you had been given.

## Procedure

1. **Open the log** on day one with the template below, filling only what is already known. Empty sections are honest; wrong sections are not.
2. **After each work session,** ask the user three questions: what did you learn, what surprised you, what do you still not understand. File the answers into the template.
3. **Convert surprises into entries.** Every surprise is either a hazard (document it), a convention (record it), or a misunderstanding (correct the earlier note that caused it).
4. **Keep the questions list ranked.** Each open question gets a next action: a file to read, a person to ask, or an experiment to run.
5. **On day five,** produce a digest: the ten facts a future newcomer would most want, drawn from the week's entries.

```
ONBOARDING LOG: <repo> - week of <date>
System purpose (one sentence): ...
Mental model so far: <3-6 bullets, revised as understanding improves>
Conventions observed: <pattern - where seen>
Hazards found: <what - where - why it bites>
Glossary: <term - meaning in this codebase>
Open questions (ranked): <question - next action>
Corrections: <date - what I had wrong - what is actually true>
```

## Rules

- Never let a correction silently overwrite an old note; the corrections section preserves what was misunderstood, because repeated misunderstandings mark bad docs or bad names worth fixing.
- Never record a mental-model bullet without at least one supporting observation from the code.
- Keep the log under two pages by pruning resolved questions into the glossary or hazards sections weekly.

## Degradation

If the user cannot share code details, run the session-end interview anyway and file their answers; the template works on recollection alone, just marked as unverified against source.


---

*Like this? The full **Code Archaeologist** bundle adds the persona plus Codebase Mapper, Dead Code Finder, Dependency Grapher — on Claw Mart.*
