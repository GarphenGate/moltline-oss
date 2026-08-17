---
name: devflow-engineer
description: Write a clean conventional commit message from a diff or change description. Use whenever the user is about to commit, asks for a commit message, or shares staged changes.
version: 1.0.0
---

# Commit Message Formatter

*Free gateway skill from the DevFlow Engineer bundle by GarphenGate.*

One job: turn "what I changed" into a commit message a stranger can trust in two years.

## Format

```
<type>(<scope>): <imperative summary, ≤65 chars, no period>

<body: WHY the change, not what — the diff shows what. Wrap at 72.>

<footer: BREAKING CHANGE: ..., Fixes #123, Refs #456>
```

Types: `feat` `fix` `perf` `refactor` `docs` `test` `build` `ci` `chore` `revert`

## Procedure

1. Read the diff (preferred) or the user's description of the change.
2. Determine ONE type. A diff that is honestly two types should be two commits — say so
   and offer the split.
3. Choose the narrowest true scope from the paths touched (`auth`, `api`, `parser`).
4. Summary line: imperative mood ("add", not "added"/"adds"), specific ("fix null deref
   in session refresh", not "fix bug").
5. Body only when the why isn't obvious from the summary. Footer for breaking changes
   and issue references the user mentions.

## Rules

- Never write "update", "misc", "wip", or "various fixes" as a summary — name the actual change or ask.
- Never invent issue numbers or claim a fix for an issue the user didn't reference.
- Breaking change without a `BREAKING CHANGE:` footer is an error — always add it when the API/contract changes.

---

*Like this? The full **DevFlow Engineer** bundle adds a staff-engineer persona plus
coding-loop, code-review, ci-watchdog, and release-notes skills — on Claw Mart.*
