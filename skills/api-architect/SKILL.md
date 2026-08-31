---
name: api-architect
description: Run 12 questions against any endpoint before it ships to catch the mistakes that become permanent. Use as the final gate before merging any API change.
version: 1.0.0
---

# API Review Checklist

*Free gateway skill from the API Architect bundle by GarphenGate.*

Twelve questions that catch the API mistakes which become permanent the moment a consumer depends on them.

## Procedure

1. Take the endpoint (design, contract, or diff) and answer each of the twelve, with evidence, not vibes:
   1. Does the consumer's calling code read naturally?
   2. Do names and casing match the rest of the API?
   3. Is every failure case specified with status and error body?
   4. Is the error shape identical to the API's standard one?
   5. Are types and constraints explicit on every field?
   6. Is pagination defined for anything that returns a list?
   7. Is the idempotency story stated for every mutation?
   8. Are timestamps, units, and timezones unambiguous?
   9. Is anything leaking storage structure into the contract?
   10. Is the change classified breaking or non-breaking, correctly?
   11. Are worked examples present and schema-valid?
   12. Would you accept this field set as permanent?
2. Mark each pass, flag, or fail with a one-line reason; a flag is something shippable but worth a written note.
3. Emit the verdict card below.

Verdict card:

```
API REVIEW: <METHOD path> — verdict: ship | fix-first | redesign
Fails: <numbers + one-line reasons>
Flags: <numbers + notes>
The one fix that matters most: <specific change>
```

## Rules

- Never answer a question from intention; only what the artifact actually specifies counts.
- Never pass question 12 as a formality; it is the whole checklist compressed, and permanent means permanent.
- Three or more fails means the verdict is redesign, not a list of patches.

## Degradation

Given only a route name with no design or contract, run the four questions that apply (1, 2, 10, 12), report the rest as not-assessable, and name the artifact needed for a full pass.

---

*Like this? This is the free gateway skill for **API Architect** by Moltline Studio. The paid listing: https://www.agensi.io/skills/api-architect-persona*
