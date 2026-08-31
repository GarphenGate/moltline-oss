---
name: git-wizard
description: Build a correct .gitignore for your exact stack, and clean up files already tracked by mistake. Use when starting a repo or when build artifacts keep showing up in diffs.
version: 1.0.0
---

# Gitignore Builder

*Free gateway skill from the Git Wizard bundle by GarphenGate.*

Build the .gitignore your exact stack needs — and handle the files that were committed before the rule existed.

## Procedure

1. Identify the stack: languages, frameworks, build tools, editors, and OS in play. Infer what is visible from any pasted file list, and ask one batched round for the rest.
2. Compose the file in labeled sections: per-language build outputs and caches, per-tool artifacts, editor and OS noise, and a project-specific section for local env files and generated assets. Every non-obvious pattern gets a trailing comment saying what it ignores.
3. Check for the classic mistakes: ignoring lockfiles that should be committed, patterns broad enough to swallow source (a bare directory name matching everywhere), and negation rules ordered so they cannot work.
4. Detect the already-tracked problem: files matching the new rules that git currently tracks will keep appearing until untracked. List them and provide the untrack commands, clearly labeled as changing the repository.
5. Deliver in the contract below.

Deliverable format:

```
GITIGNORE: <stack summary>
<the .gitignore content, sectioned and commented>

Already tracked but now ignored: <files | none found>
Untrack commands (run only after review; removes from tracking, not from disk): <commands>
Deliberately NOT ignored: <lockfiles, etc. — why they stay committed>
```

## Rules

- Never ignore dependency lockfiles by default; committing them is the norm, and ignoring them is an explicit user decision.
- Never emit an untrack command as if routine; it changes the repository for everyone and is labeled for review before running.
- Secrets and env files are ignored AND flagged: ignoring them going forward does not un-commit what is already in history, and the note says so.

## Degradation

If the stack cannot be determined, produce a minimal OS-and-editor base file plus a short question list, rather than a kitchen-sink file that hides real problems in noise.

---

*Like this? This is the free gateway skill for **Git Wizard** by Moltline Studio. The paid listing: https://www.agensi.io/skills/git-wizard-bundle*
