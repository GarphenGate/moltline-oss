---
name: memory-athlete
description: Paste a list and get three different mnemonics for it, ready to test. Use for any list that must be remembered by a date, from anatomy to a speech's points.
version: 1.0.0
---

# Mnemonic Maker

*Free gateway skill from the Memory Athlete bundle by GarphenGate.*

Paste any list; get three ways to never forget it, and a ten-minute test to see which one holds.

## Procedure

1. Take the pasted list; ask only whether order matters and when it must be known by.
2. Build three contrasting mnemonics: an acronym or acrostic (fast, good for short lists), a story chain linking items in sequence (best when order matters), and keyword images (best for foreign or technical terms).
3. Apply the vividness rules to each: concrete, absurd, in motion; flag which of the three fits this list's form best and say why.
4. Tell the user to pick one, rehearse it once, and self-test after ten minutes of doing something else; the one they retrieve best wins.
5. Close with the follow-up schedule: re-test tomorrow and in three days, thirty seconds each.

Deliver in this format:

```
THREE WAYS — <list> (order matters: y/n)
1 ACRONYM: <the build> — best if: <one line>
2 STORY CHAIN: <the chain, images spelled out> — best if: <one line>
3 KEYWORD IMAGES: <item: image> — best if: <one line>
Coach's pick for this list: <which and why>
Test: cold recall in 10 minutes, then tomorrow, then day 3.
```

## Rules

- Never deliver a mnemonic without the ten-minute cold test instruction; untested mnemonics feel like they work right up until the exam.
- Never build all three on the same mechanism; the point of three is that people's imagery tastes differ.
- Lists over 15 items get chunked before mnemonics are built; no single mnemonic should carry more than one chunk.

## Degradation

- User pastes prose instead of a list: extract the list (points, steps, or terms), show it for confirmation, then build the three ways on the confirmed list.

---

*Like this? The full **Memory Athlete** bundle adds the persona plus Mnemonic Builder, Memory Palace Guide, Recall Gamer — on Claw Mart.*
