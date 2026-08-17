---
name: function-explainer
description: Paste one function and get what it does, why it exists, and its gotchas. Use when the learner wants a fast, honest read on a single piece of code.
version: 1.0.0
---

# Function Explainer

*Free gateway skill from the Code Explainer bundle by GarphenGate.*

One function in, one structured explanation out: the what, the why, and the sharp edges, at reading-in-a-hurry length.

## Procedure

1. **Take the paste,** plus optional context (language version, framework, where it is called from). Missing context narrows the claims, it does not stop the explanation.
2. **State the what** in two sentences of plain English: inputs, outputs, and the transformation between them, as observable behavior rather than a line-by-line retelling.
3. **Infer the why carefully:** what problem this function most plausibly solves, labeled as inference unless comments or naming make it explicit.
4. **Hunt the gotchas** in a fixed sweep: edge inputs (empty, null, zero, huge), hidden state or side effects, error behavior (throws, swallows, returns sentinel), performance traps, and anything that behaves differently than the name suggests.
5. **Deliver the card** below; if the function exceeds roughly 50 lines or calls into significant unseen code, say which parts of the explanation are limited by that.

```
FUNCTION: <name or 'anonymous'>
What: <two sentences, observable behavior>
Why (inferred unless stated): <the problem it solves>
Signature says / behavior does: <match | mismatch: <detail>>
Gotchas:
  - <edge case or side effect> - <what happens> - <when it bites>
Unclear without more context: <list - or 'nothing significant'>
One-line summary you could put in a comment: <it>
```

## Rules

- Never retell the code line by line; the explanation is behavior-level or it is not an explanation.
- Never present an inferred purpose as stated fact; the label 'inferred' stays on until evidence removes it.
- Never skip the gotcha sweep even for tiny functions; three-line functions with a hidden mutation are a classic.
- If the pasted code appears mid-refactor or truncated, say so instead of explaining a fragment as a whole.

## Degradation

If the language or framework is unrecognized from the paste alone, explain what is structurally certain, ask one identifying question, and hold the gotcha sweep until the runtime semantics are known.


---

*Like this? The full **Code Explainer** bundle adds the persona plus Walkthrough Guide, Diagram Narrator, Concept Bridger — on Claw Mart.*
