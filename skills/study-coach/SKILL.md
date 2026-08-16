---
name: flashcard-maker
description: Convert any notes into clean question-and-answer flashcards ready for review or import. Use when the student pastes notes, a chapter, or a vocab list and wants cards to drill from.
version: 1.0.0
---

# Flashcard Maker

*Free gateway skill from the Study Coach bundle by Hankash.*

Turn pasted notes into flashcards that test one thing each, phrased as questions the student must retrieve, not statements to reread.

## Procedure

1. **Take the notes and the target.** Ask what deck size feels usable (default: up to 20 cards) and whether cards are for self-quizzing here or export to an app.
2. **Extract card-worthy items.** One fact, definition, or cause-effect link per card. Skip filler, duplicate phrasings, and anything the notes state ambiguously; list skipped ambiguities at the end as questions for the teacher.
3. **Write the fronts as questions.** 'What does X do?' beats 'X'. For processes, split steps across cards rather than one giant card.
4. **Write the backs short.** The shortest complete answer, one clarifying line max. If a back exceeds three lines, split the card.
5. **Offer a first pass.** Propose drilling 5 cards immediately, question first, attempt required before the back is shown.

## Output contract

```
DECK — <topic> (<n> cards)
1. Q: <question>
   A: <short answer>
2. ...
Skipped as unclear in your notes: <items or 'none'>
```

Export format on request: `question<TAB>answer` lines, one per card, ready for app import.

## Rules

- Never put more than one testable fact on a card; split instead.
- Never write a front answerable by pattern-matching a keyword in the question to the same keyword in the answer.
- Keep answers on the student's material; do not silently add outside facts to the deck.

## Degradation

Notes too thin for the requested deck size: make fewer, better cards and say the material supports only that many. Handwriting photo or unreadable input: ask the student to type or re-shoot the unclear parts rather than guessing content.

---

*Like this? The full **Study Coach** bundle adds the persona plus Spaced Drills, Quiz Generator, Curriculum Planner — on Claw Mart.*
