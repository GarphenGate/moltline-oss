---
name: thankyou-drafter
description: Draft a specific, warm donor thank-you letter from gift details; use right after any donation arrives.
version: 1.0.0
---

# Thank-You Drafter

*Free gateway skill from the Nonprofit Organizer bundle by Hankash.*

The thank-you that earns a second gift is fast, personal, and names what the money does. This skill drafts that letter from whatever gift details you have.

## Procedure

1. **Collect the minimum:** donor name, gift amount, what the gift supports, and whether this donor has given before. Ask for whichever of the four is missing.
2. **Ask for one concrete program detail** the gift touches — a number, a name, a moment. This becomes the letter's anchor sentence.
3. **Draft the letter:** open with the specific thanks, anchor paragraph, one line on what happens next for the donor (newsletter, invite, nothing oversold), warm close with a real person's name and title.
4. **Length discipline:** under 180 words. A thank-you is not an annual report.
5. **Deliver for review** with the anchor sentence highlighted so the user can verify the fact before sending from their own email or mail merge.

Output contract:

```
TO: <donor> — $<amount>, <first-time | repeat>
ANCHOR (verify this fact): <sentence>
---
<letter, under 180 words>
```

## Rules

- Never send the letter — this skill drafts, the user sends after confirming the anchor fact.
- Never invent a program detail; if the user can't supply one, the letter says what the fund is for in the org's own words and nothing more.
- Never include tax or deductibility language beyond what the user supplies as their standard receipt text.

## Degradation

Given only a name and amount, produce the honest minimal version — thanks, the fund's stated purpose, warm close — and tell the user plainly that one verified specific would make it twice the letter.

---

*Like this? The full **Nonprofit Organizer** bundle adds the persona plus Grant Boilerplater, Donor Thanker, Volunteer Coordinator — on Claw Mart.*
