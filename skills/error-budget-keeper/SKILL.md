---
name: error-budget-keeper
description: The five sections every postmortem needs, sized for small teams. Use when the user wants to run their first postmortem or standardize how incidents get written up.
version: 1.0.0
---

# Postmortem Template

*Free gateway skill from the Error Budget Keeper bundle by GarphenGate.*

The smallest postmortem format that still changes anything: five sections, one page, blameless by construction. Fill it within 48 hours of the incident while memory is still evidence.

## Procedure

1. **Copy the template** below into wherever the team keeps documents; the format matters more than the tool.
2. **Fill Impact and Timeline first,** from alerts, deploys, and chat logs; recollection-only entries get marked as such.
3. **Fill Contributing Causes** by asking 'what made that reasonable at the time' until every cause is systemic. If a sentence names a person, it is not done yet.
4. **Limit Action Items to five,** each with an owner and a date, then put the 30-day check on a calendar before closing the document.
5. **Share it with the whole team,** including whoever was closest to the incident; a postmortem read by nobody teaches nobody.

```
POSTMORTEM: <title> - <incident date>
1. Impact: <who was affected, how long, how bad, in plain numbers>
2. Timeline: <hh:mm> <event> [source or 'recollection']
3. Contributing causes: <systemic factors, plural - no names>
4. What went well: <anything worth deliberately keeping>
5. Action items (max 5): <fix - owner - due date>
30-day check: <date>
```

## Rules

- Never let the document assign blame to a person; the template's causes section accepts only systemic factors.
- Never skip 'What went well'; teams that only record failure learn to hide incidents.
- Never file the postmortem without dates on the action items; undated actions are wishes.

## Degradation

For an incident that happened weeks ago with no records, fill the template from group recollection in a 30-minute conversation, label the whole document reconstructed, and treat the evidence gap as action item one.


---

*Like this? This is the free gateway skill for **Error Budget Keeper** by Moltline Studio. The paid listing: https://www.agensi.io/skills/error-budget-keeper-persona*
