---
name: reading-comprehension-coach
description: Turn any pasted passage into comprehension questions with answer locations. Use to self-quiz after a reading or to check that an assigned text was actually understood.
version: 1.0.0
---

# Question Generator

*Free gateway skill from the Reading Comprehension Coach bundle by GarphenGate.*

Paste a passage, get questions that check understanding rather than memory of the first sentence.

## Procedure

1. Take the pasted passage; ask only one thing if missing: is this for self-quizzing or for quizzing someone else?
2. Read the whole passage before writing anything; identify its claim, its evidence, and one place a careless reader would go wrong.
3. Write five questions: two literal, two inference, one about the argument's structure.
4. Attach the answer location (paragraph or sentence) to each; write the answers in a separate block so self-quizzers can hide them.
5. Aim one question directly at the spot where a careless reader goes wrong.

Deliver in this format:

```
COMPREHENSION CHECK — <passage>
Q1 [literal] <question> (ans: para <n>)
Q2 [literal] <question> (ans: para <n>)
Q3 [inference] <question> (ans: paras <n>-<m>)
Q4 [inference] <question> (ans: para <n>)
Q5 [argument] <question> (ans: whole passage)
--- answers below ---
A1..A5: <one line each>
```

## Rules

- Never write a question answerable without reading past the first paragraph.
- Never quiz on trivia (dates, names) unless the passage's argument turns on them.
- Questions use the passage's own terms; introducing outside vocabulary tests the reader's background, not their comprehension.

## Degradation

- Passage described but not pasted: write the five questions anyway, mark answer locations "approximate," and note the check is unverified against the source.

---

*Like this? This is the free gateway skill for **Reading Comprehension Coach** by Moltline Studio. The paid listing: https://www.agensi.io/skills/reading-comprehension-coach-persona*
