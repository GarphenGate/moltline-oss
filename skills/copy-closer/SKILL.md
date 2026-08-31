---
name: copy-closer
description: Generate ten CTAs matched to a page's actual intent instead of defaulting to 'Learn More'; use whenever any button, link, or ask needs words and the cursor is blinking.
version: 1.0.0
---

# CTA Generator

*Free gateway skill from the Copy Closer bundle by GarphenGate.*

Ten call-to-action options matched to what the page actually asks and what the click actually delivers — because 'Learn More' is where conversions go to nap.

## Procedure

1. **Get two facts**: what action the page wants (buy, book, subscribe, download, start trial) and what literally happens after the click (checkout, calendar, form, inbox). If either is missing, ask for exactly that and nothing else.
2. **Generate ten CTAs across five stances**, two each: first-person ownership, outcome-forward, effort-reduction, risk-reduction, and specific-deliverable. Every one must truthfully describe the click's real destination.
3. **Add microcopy to the top half**: one under-button line each that lowers the click's perceived risk (what happens next, no-card note, time estimate) — honest ones only.
4. **Mark the top three** for the stated intent with a one-line reason tied to the reader's likely hesitation at that moment.
5. **Flag mismatches** discovered along the way: if the page's ask and the click's destination disagree (button says 'Start free', click opens a sales call), say so — that mismatch costs more than any button copy gains.

## Output

```
CTA OPTIONS — action: <what> / after click: <what>
1. [ownership] "<cta>" + micro: "<line>"
... (10, stance-labeled)
Top 3: #<n> — <reason>, #<n> — <reason>, #<n> — <reason>
Mismatch flag: <ask vs destination conflict, if found>
```

## Rules

- Never generate a CTA that overpromises the click ('Get instant results' into a contact form); the button describes the real next screen.
- Never include manufactured urgency or fake scarcity in CTA or microcopy; if real scarcity exists, the user states it first.
- 'Learn More', 'Submit', and 'Click Here' appear only if the user asks why they underperform, with the explanation.
- Must not exceed ten options; a wall of forty buttons helps nobody choose.

## Degradation

With only a URL or page description and no stated action, infer the most likely intent, generate against it, and label the inference for correction. With a multi-purpose page ('it's our homepage'), generate for the primary action only and note that a page asking three things needs a hierarchy decision before button copy matters.

---

*Like this? This is the free gateway skill for **Copy Closer** by Moltline Studio. The paid listing: https://www.agensi.io/skills/copy-closer-persona*
