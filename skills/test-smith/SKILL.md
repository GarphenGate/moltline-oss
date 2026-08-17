---
name: test-namer
description: Rename tests so failures explain themselves without opening the file. Use when a suite's failure output reads like a phone book, or before sharing a suite with collaborators.
version: 1.0.0
---

# Suite Namer

*Free gateway skill from the Suite Smith bundle by GarphenGate.*

Name tests so a failure message alone tells you what broke, under what condition, and why it matters.

## Procedure

1. Take the test list or file the user provides and extract, for each test: the behavior verified, the condition, and the expected outcome. Read the body when the current name hides them.
2. Rewrite each name into the project's convention using the pattern: subject, condition, expected outcome (for example: "retry gives up after three failures and surfaces the last error").
3. Flag names that cannot be fixed because the test asserts nothing behavioral; naming cannot rescue a meaningless test, so mark it for the user's review instead of polishing it.
4. Output the rename table below, ready to apply.

Rename table:

```
TEST RENAMES: <file>
Old name -> New name
<row per test>
Unfixable (test asserts no behavior, review needed): <list>
Convention used: <pattern + example>
```

## Rules

- Never encode implementation details (method names, internal classes) into a test name; names outlive refactors.
- Never produce a name that could describe two different failures; ambiguity in a name is a debugging tax.
- Keep names under about twelve words; longer means the test covers too much and should split.

## Degradation

Given only failure output instead of test files, rename what appears in the output, mark each rename "from failure text only," and ask for the file to verify the assertions match the new names.

---

*Like this? The full **Suite Smith** bundle adds the persona plus Suite Strategist, Test Writer, Coverage Gapper — on Claw Mart.*
