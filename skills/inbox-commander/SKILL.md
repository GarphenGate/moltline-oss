---
name: inbox-digest
description: Produce a morning summary of what in the inbox actually needs you, in three lines; use daily before opening email, so email does not open you.
version: 1.0.0
---

# Inbox Digest

*Free gateway skill from the Inbox Commander bundle by GarphenGate.*

Answer one question before the inbox gets a chance to shout: what in there needs me?

## Procedure

1. **Take the morning's input.** Pasted new-message list, forwarded overnight mail, or the user's quick description of what arrived.
2. **Extract only items that need the user**: a decision, a reply with their authority, or something time-bound today. Everything else is noise for this digest's purposes.
3. **Compress to three lines maximum.** One item per line: who, what they need, by when. If more than three qualify, keep the three with the nearest consequences and add a count of the remainder.
4. **Add the all-clear when true.** An empty digest is a valid and excellent digest: say "Nothing needs you before noon" when that is the honest read.
5. **Stop.** No summaries of newsletters, no FYI recaps, no inbox statistics. Three lines is the contract.

## Output

```
DIGEST — <date>
1. <sender>: <what they need> — by <when>
2. ...
3. ... (+<n> more can wait)
```

## Rules

- Never exceed three lines of items; the fourth-most-important email is by definition not urgent.
- Never include a message just because the sender is senior; seniority without an ask is FYI.
- Must not soften an empty digest with filler; "nothing needs you" builds more trust than manufactured urgency.

## Degradation

With nothing pasted, ask one question: "anything arrive overnight you're worried about?" and digest the answer. If the user lists ten worries, triage them to three by nearest deadline and note the cut.

---

*Like this? The full **Inbox Commander** bundle adds the persona plus Email Triage, Follow-up Chaser, Unsubscribe Auditor — on Claw Mart.*
