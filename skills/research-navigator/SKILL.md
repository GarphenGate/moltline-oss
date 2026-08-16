---
name: citation-formatter
description: Convert any pasted reference into clean APA, MLA, or Chicago format with missing fields flagged. Use whenever a reference needs formatting or restyling from one citation format to another.
version: 1.0.0
---

# Citation Formatter

*Free gateway skill from the Research Navigator bundle by Hankash.*

Paste any reference in any state (a URL, a messy citation, half a memory of a paper) and get it back formatted in APA, MLA, or Chicago, with every missing or uncertain field flagged instead of faked.

## Procedure

1. **Parse what arrived.** Extract every available field: authors, year, title, container, publisher, volume, pages, DOI/URL. State the detected source type (journal article, book, chapter, web page, report); ask if it's ambiguous.
2. **Confirm the target.** Ask which style (APA 7, MLA 9, Chicago 17 notes or author-date) if not stated; default APA 7 with the default named.
3. **Format from real fields only.** Build the citation using exactly the fields present. Each absent field gets a bracketed flag in place, not a plausible guess.
4. **Show the gaps.** Under the citation, list what's missing and where to find it (usually the article's landing page or the book's copyright page).
5. **Offer siblings.** On request: the same reference in the other two styles, plus the matching in-text form for the chosen style.

## Output contract

```
FORMATTED CITATION — <style>
<the citation, with [MISSING: field] markers where data is absent>
In-text: <the matching in-text/note form>
Missing fields: <field — where to find it> (or 'complete')
Confidence: <parsed cleanly / check the fields marked ?>
```

## Rules

- Never invent an author, year, page, or DOI to complete a citation; a flagged gap is correct, a guessed field is misconduct-adjacent.
- Never present a from-memory 'known paper' completion as verified; anything added from recall is marked 'verify against the original'.
- Keep one reference per pass unless a batch is requested; batches return in the same flagged format.

## Degradation

Input too thin to identify the source (title fragment only): return a search strategy (where to look, what terms) instead of a citation. Style not among the big three: format in the closest base style and list the deviations to check in the venue's guide.

---

*Like this? The full **Research Navigator** bundle adds the persona plus Literature Mapper, Source Logger, Citation Hygienist — on Claw Mart.*
