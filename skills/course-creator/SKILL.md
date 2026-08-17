---
name: course-creator
description: Generate a course's first module map from a single topic prompt; use when the course is still just an idea and a pile of expertise.
version: 1.0.0
---

# Course Outline

*Free gateway skill from the Course Creator bundle by GarphenGate.*

One topic prompt in, a credible module map out: enough structure to see the course, honest about what's still a guess.

## Procedure

1. **Take the topic and probe once**: who is this for, and what should they be able to do afterward? If the user doesn't know yet, pick the most likely student and label the choice ASSUMED.
2. **Draft the exit capability** in one sentence, stated as something demonstrable.
3. **Map five to seven modules** in dependency order, each titled as a capability, each with two or three lesson bullets and one named check.
4. **Place the arc markers**: the module-1 early win, the midpoint milestone, and the finale artifact.
5. **Flag the risks**: which modules assume knowledge the student may lack, and which look too big to finish. One line each.

## Output

```
COURSE IDEA: <topic> / STUDENT: <who (ASSUMED?)>
EXIT: <capability sentence>
1. <capability module> — <2-3 lesson bullets> — check: <artifact>
...
ARC: early win <...> / midpoint <...> / finale <...>
RISKS: <assumption flags + too-big flags>
NEXT: the two questions to answer before building
```

## Rules

- Never title modules as topics; capabilities only, even in a first draft.
- Never present the assumed student as settled; ASSUMED labels stay until the user confirms.
- Five to seven modules in the first map; a twelve-module first draft frightens the creator and the student alike.

## Degradation

If the topic is too broad for one course ("photography"), return two or three narrower course ideas with one-line exit capabilities each, and outline whichever the user picks.

---

*Like this? The full **Course Creator** bundle adds the persona plus Curriculum Outliner, Lesson Scripter, Worksheet Builder — on Claw Mart.*
