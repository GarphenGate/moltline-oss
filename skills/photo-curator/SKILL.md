---
name: photo-curator
description: Give three caption angles for any photo the user describes; use when a post is sitting in drafts because the words won't come.
version: 1.0.0
---

# Caption Helper

*Free gateway skill from the Photo Curator bundle by GarphenGate.*

Describe the photo, get three genuinely different caption angles, and stop staring at the drafts folder.

## Procedure

1. **Take the description**: what's in the frame, where it's going (platform), and one line of context if the user has it.
2. **Find what the photo can't say.** Ask one question if needed: what happened right before or after this frame, or what it took to get it.
3. **Write three angles, labeled**: STORY (the behind-the-frame moment), TAKE (an opinion this photo is evidence for), and DEADPAN (one dry line that trusts the image). Each is a finished caption, not a direction.
4. **Keep them platform-shaped**: first line survives truncation, length matches the platform norm.
5. **Add alt text** in one sentence, because accessible posts are finished posts.

## Output

```
PHOTO: <one-line description>
STORY: "<caption>"
TAKE: "<caption>"
DEADPAN: "<caption>"
ALT TEXT: "<one sentence>"
```

## Rules

- Never write a caption that just restates the description; the description was the input, not the output.
- Never fabricate context; if the user gave no story, the STORY angle asks for one instead of inventing one.
- Three angles, three registers; if two sound alike, one gets rewritten before delivery.

## Degradation

With only "help me caption this" and no description, ask for the one-line description and the platform, then proceed; never caption an unseen, undescribed photo from guesswork.

---

*Like this? This is the free gateway skill for **Photo Curator** by Moltline Studio. The paid listing: https://www.agensi.io/skills/photo-curator-persona*
