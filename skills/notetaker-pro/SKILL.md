---
name: note-formatter
description: Clean raw meeting scrawl or reading notes into structured, linkable entries without losing your words; use on any note too messy to trust in a month.
version: 1.0.0
---

# Note Formatter

*Free gateway skill from the Notetaker Pro bundle by GarphenGate.*

From scrawl to a note future-you can find, trust, and link, without the formatter putting words in your mouth.

## Procedure

1. **Take the mess as-is:** typed fragments, transcribed scribbles, a wall of un-punctuated text. Ask nothing before the first pass.
2. **Separate the layers.** Sort the content into: SOURCE MATERIAL (quotes and claims from a source, with the source named or marked unstated), THE USER'S THINKING (reactions, disagreements, ideas), and LOOSE ENDS (fragments too ambiguous to place). The layer boundary is the formatter's real product; mixed layers are how notes lie later.
3. **Structure within layers:** short headed sections, the user's own phrasing preserved. Tighten grammar only where meaning is unambiguous; anything genuinely unclear goes to LOOSE ENDS as-is rather than being guessed into fluency.
4. **Stamp the header:** title in the user's words, date, source with provenance type (quote/paraphrase/own), and up to three suggested tags.
5. **Return the note with its open questions:** each LOOSE END restated as a question only the user can answer ("does 'check Feldman' mean the 2019 paper or a person?"), so ambiguity is resolved by the author, not the formatter.

## Output

```
# <title in the user's words>
date: <date> | source: <source or "unstated"> | type: <quote/paraphrase/own mix noted>
tags: <up to 3>
## From the source
<claims and quotes, attributed>
## My thinking
<the user's reactions, their phrasing kept>
## Loose ends
- <fragment> → <clarifying question>
```

## Rules

- Never blend the source's claims with the user's thinking; the section boundary is inviolable, and uncertain lines go to loose ends.
- Never invent a source, a date, or a fluent version of an ambiguous fragment; missing stays visibly missing.
- Must not rewrite the user's voice into house style; grammar may be tightened, phrasing belongs to the author.

## Degradation

Given a note in a language mix or heavy shorthand, format what is parseable, preserve the rest verbatim in loose ends, and return a short legend of shorthand guesses for the user to confirm once, so future formatting passes learn their notation.

---

*Like this? The full **Notetaker Pro** bundle adds the persona plus Capture Inbox, Note Filer, Weekly Synthesis — on Claw Mart.*
