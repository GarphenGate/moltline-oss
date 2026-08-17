---
name: frontend-finisher
description: Check a UI against the eight accessibility issues most products ship with, in fifteen minutes. Use on any page before it goes public, or as a first look at an inherited frontend.
version: 1.0.0
---

# A11y Quick Check

*Free gateway skill from the Frontend Finisher bundle by GarphenGate.*

The fifteen-minute check for the eight accessibility issues most UIs ship with — hands-on, evidence required.

## Procedure

1. Take one page or flow, and run the eight checks in order, each with its concrete test:
   1. Keyboard path: tab through the whole flow — everything reachable, focus visible, no traps.
   2. Image meaning: informative images have alt text that carries the meaning; decorative ones are marked decorative.
   3. Form labels: every input has a programmatic label, not just placeholder text.
   4. Contrast: body text and controls meet AA ratios, measured, not eyeballed.
   5. Heading structure: one h1, levels don't skip, structure matches the visual hierarchy.
   6. Link and button names: every control's accessible name says what it does out of context.
   7. Zoom: page at 200% zoom loses no content or function.
   8. Motion and flashing: animations respect reduced-motion, nothing flashes.
2. Record pass or fail per check with the evidence (the element, the measured ratio, the keystroke where focus vanished).
3. Emit the card below with the top fix identified by user impact.

Check card:

```
A11Y QUICK CHECK: <page> — <n>/8 passed (engineering check, not certification)
1. Keyboard  pass|fail — <evidence>
...
8. Motion    pass|fail — <evidence>
Top fix: <the failure blocking the most users, with the smallest change>
Full pass recommended if: <2+ fails, or any keyboard fail>
```

## Rules

- Never mark a check passed without its hands-on test performed or its evidence pasted; assumed passes are marked "unchecked", not passed.
- Never present 8/8 as accessible; the card says these eight common issues were checked, and links the deeper pass for the rest.
- Evidence names elements specifically; "some buttons" is not a finding location.

## Degradation

Given markup only and no live page, run checks 2, 3, 5, and 6 statically, mark 1, 4, 7, 8 "requires live page" with the exact manual steps, and score only what was actually checked.

---

*Like this? The full **Frontend Finisher** bundle adds the persona plus Accessibility Passer, Responsive Auditor, Performance Budgeter — on Claw Mart.*
