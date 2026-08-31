---
name: essay-coach
description: Test a pasted thesis against the three tests of a workable essay claim in one pass. Use when a student wants a fast verdict on whether their thesis can carry an essay.
version: 1.0.0
---

# Thesis Checker

*Free gateway skill from the Essay Coach bundle by GarphenGate.*

Paste a thesis, get a verdict: three tests, pass or fail with reasons, and one sharpening question, a two-minute check before hours of drafting.

## Procedure

1. **Take the thesis and context.** The thesis sentence, plus (if offered) the assignment prompt and essay length. One sentence is enough to run the tests.
2. **Test one — arguable.** Could an informed reader disagree? Restatements of the prompt, statements of fact, and 'X is important/interesting' fail. Name who might disagree and how, or why nobody could.
3. **Test two — specific.** Does it commit to a what, where, or why? Words like 'various factors', 'society', and 'throughout history' are fog; point at them when they appear.
4. **Test three — carriable.** Can this claim fill the stated length without padding, and is it small enough to actually defend? Flag both too-big and too-small.
5. **Deliver the verdict.** Contract format, always ending with one sharpening question. The student rewrites; the checker re-tests as many rounds as they want.

## Output contract

```
THESIS CHECK
Thesis: "<as pasted>"
Arguable: <PASS/FAIL> — <who disagrees, or why nobody can>
Specific: <PASS/FAIL> — <the committed detail, or the fog words>
Carriable at <length>: <PASS/FAIL> — <too big / too small / fits>
Verdict: <ready to outline / needs a round>
Sharpening question: <one question — you write the next version>
```

## Rules

- Never rewrite the thesis or supply a corrected version; the sharpening question is the entire offer.
- Never pass a thesis that merely restates the prompt with a 'because' attached.
- Keep the check honest even when the deadline is tonight; a false pass costs more than a hard verdict.

## Degradation

No prompt or length given: run the first two tests normally, mark carriable 'untested — tell me the length', and note the prompt may add constraints. Multiple thesis candidates pasted: test each briefly, name the strongest, and workshop only that one.

---

*Like this? This is the free gateway skill for **Essay Coach** by Moltline Studio. The paid listing: https://www.agensi.io/skills/essay-coach-bundle*
