---
name: ticket-template
description: The ticket format that prevents mid-sprint surprises, ready to adopt today. Use when the user wants a standard ticket structure or asks why their tickets keep going sideways.
version: 1.0.0
---

# Ticket Template

*Free gateway skill from the Sprint Mechanic bundle by GarphenGate.*

Most mid-sprint surprises were visible in the ticket, or would have been if the ticket had a place to hold them. This is that ticket, with instructions for adopting it.

## Procedure

1. **Hand over the template** below, unchanged, and walk through why each field exists in one line each.
2. **Tune it to their tooling.** Ask what tracker the team uses and adapt field names to it (description, custom fields, checklists) without dropping any field.
3. **Test it on a real ticket.** Have the user pick their most recent problem ticket and refile it in the template; the fields that were empty are usually where the surprise came from. Point at that connection explicitly.
4. **Set the adoption rule:** new tickets use the template starting now; old tickets get converted only when they are next touched.

```
TICKET: <verb-first title>
Problem: <who hurts, and how, in plain language>
Desired outcome: <the observable end state>
Acceptance criteria:
  - Given <state>, when <action>, then <checkable result>
Out of scope: <what this ticket deliberately does not cover>
Dependencies: <tickets, people, or decisions this waits on>
Open questions: <question - owner>
Size feel: <XS | S | M | L - L means consider splitting>
```

## Rules

- Never let 'Out of scope' stay empty; scope creep enters through the field nobody filled in.
- Never merge acceptance criteria into prose; each criterion is a separate, checkable line.
- Keep the whole ticket under one screen; a ticket that scrolls is a spec, and specs live elsewhere with a link.

## Degradation

If the user cannot share a real past ticket for the test drive, run step 3 on a hypothetical built from their description of a recent surprise, and label it as such.


---

*Like this? The full **Sprint Mechanic** bundle adds the persona plus Ticket Groomer, Estimation Coach, Standup Notes — on Claw Mart.*
