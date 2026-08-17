---
name: helptext-reviewer
description: Paste your --help output and get a concrete rewrite with reasons. Use when the user suspects their help text confuses people or wants a fast second opinion on it.
version: 1.0.0
---

# Help Text Reviewer

*Free gateway skill from the CLI Craftsman bundle by GarphenGate.*

One paste, one review, one rewrite. The full Help Text Writer builds from scratch; this takes what exists and returns the improved version with every change justified.

## Procedure

1. **Take the paste** of the current --help output, plus (optional but valuable) one sentence on what the tool does and who uses it.
2. **Score it against the five checks:** summary line answers 'is this the tool I need'; a copy-pasteable example appears in the first ten lines; options show defaults; error-prone flags are explained, not just named; total length fits one screen.
3. **Write the rewrite,** preserving the tool's actual flags and behavior exactly as described; where the paste is ambiguous about behavior, keep the original wording and mark the ambiguity rather than inventing semantics.
4. **Deliver both parts** in the format below: the rewrite ready to use, then the change log with a one-line reason per change so the user learns the pattern, not just the fix.

```
HELP TEXT REVIEW
Score: <n>/5 - <failed checks named>
--- REWRITE ---
<the improved help text, complete>
--- CHANGES ---
1. <what changed> - <why, one line>
Ambiguities kept as-is: <list, with the question to resolve each - or 'none'>
```

## Rules

- Never invent flags, defaults, or behaviors not present in the paste; ambiguity is marked, not filled.
- Never return criticism without the rewrite; the rewrite is the review.
- Keep the rewrite within one screen (about 25 lines); if the original cannot fit, the review says what moves to subcommand help.

## Degradation

If the paste is a fragment or the tool's purpose is unstated, review what is present, mark the summary line as provisional, and list the two questions whose answers would complete the rewrite.


---

*Like this? The full **CLI Craftsman** bundle adds the persona plus CLI UX Designer, Help Text Writer, Packaging Guide — on Claw Mart.*
