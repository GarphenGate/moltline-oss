---
name: upgrade-checklist
description: The safe path through any major version bump, as a reusable checklist. Use when the user is about to take a major upgrade and wants the steps that prevent the classic disasters.
version: 1.0.0
---

# Upgrade Checklist

*Free gateway skill from the Dependency Warden bundle by Hankash.*

Every painful major bump skipped one of the same eight steps. This is the checklist that keeps them unskipped, reusable for any dependency in any stack.

## Procedure

1. **Copy the checklist** below into the upgrade's ticket or notes; it is the artifact, and each step gets checked with a one-line note, not just a tick.
2. **Work it strictly in order.** The order is load-bearing: reading notes before scanning usage wastes the scan; upgrading before branching removes the escape hatch.
3. **Stop at any failed step.** A failed step means the bump is not ready, and the note on that step becomes the blocker to resolve; proceeding past a failure converts a chore into an incident.
4. **Keep the completed checklist** with its notes; a stack of them becomes the project's upgrade playbook and the estimate source for next time.

```
MAJOR BUMP CHECKLIST: <dep> <current> -> <target>
[ ] 1. Release notes read across the FULL version range - notes: ...
[ ] 2. Usage scanned: call sites counted and located - notes: ...
[ ] 3. Breaking changes mapped to our call sites - notes: ...
[ ] 4. Escape hatch ready: branch + rollback step written down - notes: ...
[ ] 5. Bump applied in isolation (no other changes in the same commit) - notes: ...
[ ] 6. Full test suite green + deprecation warnings reviewed - notes: ...
[ ] 7. Behavioral spot-checks on changed-semantics areas - notes: ...
[ ] 8. Staged rollout or canary where the stack allows - notes: ...
Done: <date> - actual effort: <time> (feed this into the next estimate)
```

## Rules

- Never combine the bump commit with feature work or refactors; step 5 exists so a revert stays a one-liner.
- Never skip step 1 because the target 'is only one major ahead'; the whole range gets read, mid-range minors hide breaks.
- Never call the upgrade done while deprecation warnings are silenced instead of reviewed; silenced warnings are step 1 of the next disaster.

## Degradation

For stacks without a test suite (step 6 impossible as written), substitute a written manual smoke script covering the scanned call sites, and record that substitution in the checklist notes as accepted risk.


---

*Like this? The full **Dependency Warden** bundle adds the persona plus Upgrade Planner, Changelog Digester, Breakage Assessor — on Claw Mart.*
