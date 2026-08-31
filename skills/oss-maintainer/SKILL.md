---
name: oss-maintainer
description: Bug and feature templates that produce reports maintainers can act on. Use when the user's issue queue is full of unusable reports or they are setting up a new repository.
version: 1.0.0
---

# Issue Templates

*Free gateway skill from the OSS Maintainer bundle by GarphenGate.*

Half of triage pain is self-inflicted by a blank issue box. These two templates make good reports the default and unusable ones visibly incomplete.

## Procedure

1. **Ask three calibration questions:** what the project is, what one piece of information reporters most often omit (version, config, platform), and whether reporters are mostly developers or end users. Tune field wording to that audience.
2. **Generate the bug template** below, adapting the environment fields to the project's stack.
3. **Generate the feature request template,** which asks for the problem before the proposal, because proposals without problems are scope creep in disguise.
4. **Deliver both as ready-to-commit files** for the repository's issue-template directory, with a one-line description of where to put them for the user's forge (GitHub, GitLab, or other).

```
BUG REPORT TEMPLATE (fields)
- What happened: <one or two sentences>
- What you expected instead:
- Minimal reproduction: <smallest steps or snippet that shows it>
- Version: <project version> | Environment: <OS / runtime / relevant config>
- Started when: <first noticed / after upgrading from>

FEATURE REQUEST TEMPLATE (fields)
- The problem: <what you cannot do today, and the cost of that>
- Your current workaround:
- Proposed solution (optional):
- Would this change existing behavior: <yes/no/unsure>
```

## Rules

- Never add more than six fields to either template; long templates get skipped and the blank box returns by the side door.
- Never make the reproduction field optional in the bug template; it is the one field that pays for triage.
- The feature template must ask for the problem before the proposal, in that order, always.

## Degradation

If the user cannot say what reporters typically omit, ship the general-purpose versions above unchanged and suggest revisiting after the next ten issues reveal the pattern.


---

*Like this? This is the free gateway skill for **OSS Maintainer** by Moltline Studio. The paid listing: https://www.agensi.io/skills/oss-maintainer-persona*
