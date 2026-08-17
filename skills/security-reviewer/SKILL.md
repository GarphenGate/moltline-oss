---
name: security-reviewer
description: A pre-launch defensive pass anyone on the team can run in an afternoon. Use before shipping anything public-facing or after inheriting a project with unknown security posture.
version: 1.0.0
---

# Security Checklist

*Free gateway skill from the Security Reviewer bundle by GarphenGate.*

The pre-launch defensive pass for teams without a security team: twelve doors to lock, checkable in an afternoon.

## Procedure

1. Walk the twelve checks against the project, answering yes, no, or not-applicable-because (reason required):
   1. Auth required on every non-public route, verified by trying one?
   2. Authorization checked at the resource, not just the menu?
   3. All user input validated server-side?
   4. Secrets out of code and configs, injected at runtime?
   5. Dependencies pinned and recently audited?
   6. HTTPS everywhere, including internal callbacks?
   7. Passwords and tokens stored hashed or managed, never plaintext?
   8. Error messages free of stack traces and internal paths?
   9. Rate limiting on login, signup, and expensive endpoints?
   10. Backups exist and one restore has been tested?
   11. Logs capture auth events without capturing credentials?
   12. A person is named to receive vulnerability reports?
2. For each "no", state risk, realistic likelihood, and the smallest mitigation, in one line each.
3. Rank the "no" items into a fix order by exposure, and emit the result below.

Result format:

```
PRE-LAUNCH PASS: <project> — <date>
Score: <n>/12 (n/a excluded: <which + why>)
Fix order:
  1. <check #> — risk -> smallest mitigation
Locked doors: <checks passed>
Revisit: <trigger — new endpoints, new deps, or 90 days>
```

## Rules

- Never present a 12/12 as "secure"; the closing line is always "this pass addressed these twelve areas", nothing broader.
- Never provide attack instructions to demonstrate a gap; the risk statement names the outcome, not the technique.
- Verification beats assertion: checks answered from memory rather than by looking are marked "unverified" and count as half.

## Degradation

If the user can only answer some checks, score what is answerable, list the rest as "unknown — how to check" with a concrete verification step each, and rank unknowns above passes in the fix order.

---

*Like this? The full **Security Reviewer** bundle adds the persona plus Dependency Auditor, Secret Hygienist, Threat Sketcher — on Claw Mart.*
