# Moltline Studio — Free Agent Skills

![MCPize Health](https://mcpize.com/badge/health/13dfabef3d368e2ac5a340c36c470c6a9733f62b9305bab7cfcbf9e5b9d64470)

**138 free, production-grade `SKILL.md` gateway skills** for AI agents. Every
folder under `skills/` is a self-contained skill with a valid `SKILL.md` — drop
it into Claude Code, Cursor, Codex CLI, Gemini CLI, or any SKILL.md-compatible
agent and it works immediately. No dependencies, no signup, no API keys. Built,
versioned, and QA-tested by [Moltline Studio](https://moltlinestudio.com).

## Install a skill

Clone the repo, then copy any skill folder into your agent's skills directory.

**Cursor** — project-level (`.cursor/skills/` or `.agents/skills/`) or user-level
(`~/.cursor/skills/`):

```bash
git clone https://github.com/GarphenGate/moltline-oss.git
cp -r moltline-oss/skills/api-architect .cursor/skills/   # one skill, this project
cp -r moltline-oss/skills/* ~/.cursor/skills/             # all 138, every project
```

**Claude Code / Claude Desktop:**

```bash
cp -r skills/api-architect ~/.claude/skills/
```

**Codex CLI, Gemini CLI, or any SKILL.md-compatible agent** — copy the folder
into that agent's skills directory; `.agents/skills/` is the emerging
cross-tool convention.

Then invoke it by name in your agent. Each `SKILL.md` declares its own `name`
and `description` in YAML frontmatter, so compatible agents pick it up
automatically.

## What is a gateway skill?

Each skill here is the **free gateway** to a larger Moltline persona bundle. The
gateway does one focused, genuinely useful job on its own; the full bundle
(persona + additional skills) is available on the marketplaces below. Free is
free forever — the gateway is not a crippled demo.

## Catalog (138 skills)

<details>
<summary><b>Browse all 138 skills</b></summary>

- **`accommodations-planner`** — Plain-language explanations of common accommodation terms teachers meet in official plans \u2014 what each generally looks like in classrooms. Use when a plan lands with vocabulary you have not implemented before.
- **`accounting-practice-pal`** — Generate a starter document checklist for a new client by situation, in plain English. Use at first contact, before the engagement details are even settled.
- **`api-architect`** — Run 12 questions against any endpoint before it ships to catch the mistakes that become permanent. Use as the final gate before merging any API change.
- **`appointment-keeper`** — One list of everything expiring in the next 90 days, sorted by how soon it bites. Use quarterly or whenever expiry anxiety strikes.
- **`art-critique-partner`** — Guide a self-critique of any piece through seven questions; use before sharing work or whenever no critique partner is available.
- **`auto-shop-service-desk`** — Generate the five repair-status message templates every shop needs, in your shop's voice; use to set up proactive customer updates.
- **`blog-machine`** — Produce the post skeleton that beats the blank page for any topic in two minutes; use when starting from zero, before a client call, or to unstick a post you cannot begin.
- **`bookkeepers-assistant`** — List every uncategorized or oddly-categorized transaction in an export, sized and sorted for fastest cleanup. Use when the user wonders how messy their books are or pastes an export to check.
- **`brand-voice-keeper`** — Reveal a brand's actual voice through five forced-choice questions with instant analysis; use at the very start of voice work, or to get a vague client saying concrete things about how they sound.
- **`bug-hunter`** — Turn a vague 'it's broken' into a report a maintainer can act on. Use whenever a bug needs to be filed, handed off, or posted to an issue tracker.
- **`calendar-surgeon`** — One pasted week in, one blunt verdict out on how sick the calendar is and where it hurts most; use as the fast first look before any deeper surgery.
- **`car-keeper`** — Generate the maintenance calendar for the user's exact vehicle and driving pattern. Use when the user asks what maintenance their car needs and when, or wants a service schedule to start from.
- **`career-upskiller`** — Ten questions that reveal your real gap for a target role. Use before spending money on any course, or when you suspect the gap is not what you think.
- **`celebration-planner`** — Everything to lock in for a celebration, grouped by weeks-out with lead times built in. Use when the user asks what they need to do for an upcoming party or wants a party checklist.
- **`certification-tracker`** — The full path to a target certification on one page, with verify markers. Use when deciding whether to pursue a cert or what the first unblocking step is.
- **`chief-of-staff`** — Turn rough notes into a crisp yesterday/today/blockers update; use before a standup, an investor ping, or any moment someone asks what you have been doing.
- **`classroom-commander`** — Get a quick, dignified playbook to reset a class period that's going sideways \u2014 right now or for tomorrow. Use in the planning minutes before or after the rough one.
- **`cli-craftsman`** — Paste your --help output and get a concrete rewrite with reasons. Use when the user suspects their help text confuses people or wants a fast second opinion on it.
- **`clinic-office-helper`** — Generate the office FAQ page skeleton covering what patients actually ask clinics. Use when building or overhauling the practice's FAQ or welcome packet.
- **`code-archaeologist`** — A structured note-taking template for your first week in a new codebase. Use when the user starts on unfamiliar code and wants their learning captured instead of evaporating.
- **`code-explainer`** — Paste one function and get what it does, why it exists, and its gotchas. Use when the learner wants a fast, honest read on a single piece of code.
- **`coding-teacher`** — Serve one small daily coding exercise at the learner's level with test cases and laddered hints. Use each day the learner checks in, or whenever they ask for today's exercise.
- **`comedy-writing-room`** — Mine the comedian's ordinary week for ten workable premises; use when the notebook is empty and everything feels done already.
- **`construction-foreman-aide`** — Get the two-minute end-of-day site log format crews actually fill in. Use to standardize daily documentation across projects today.
- **`content-studio-pro`** — Generate ten scroll-stopping openings for any topic, spread across distinct hook mechanics; use before drafting any post, script, or headline when the opening line is the blocker.
- **`context-switch-killer`** — Park any incoming interruption in one line and return to flow in under ten seconds; use the moment a ping, thought, or 'quick question' lands mid-focus.
- **`copy-closer`** — Generate ten CTAs matched to a page's actual intent instead of defaulting to 'Learn More'; use whenever any button, link, or ask needs words and the cursor is blinking.
- **`course-creator`** — Generate a course's first module map from a single topic prompt; use when the course is still just an idea and a pile of expertise.
- **`creative-sprint-coach`** — Deliver a ready-to-start 30-day challenge for the maker's medium; use when someone wants to start a sprint today without designing one.
- **`crm-hygienist`** — List every open deal with no activity in 14 or more days, ranked by value with days-silent attached; use as the Monday-morning two-minute pipeline truth serum.
- **`curriculum-architect-hs`** — Outline a single lesson in backward-design order \u2014 objective, evidence, arc \u2014 in about five minutes. Use for tomorrow's lesson or to feel out the method before planning a full unit.
- **`daily-dispatch`** — Force-rank today's overgrown list down to three with a one-line reason each; use any morning the to-do list is longer than the day.
- **`database-doctor`** — Paste a slow query and schema, get ranked index candidates with reasoning and costs. Use when a specific query is slow and you suspect an index would help.
- **`deadline-guardian`** — One list of everything due in the next 14 days, sorted by risk rather than by date; use Monday morning or any time the week feels ominous.
- **`decision-log`** — Provide the one-page record format for decisions that matter, tuned to the user's situation with a worked example; use when someone wants to start logging decisions today.
- **`delegation-desk`** — A 60-second verdict on whether a task is worth delegating or faster to just do; use whenever you catch yourself doing something someone else could.
- **`deliverability-doctor`** — Check a subject line for spam-risk patterns and get two clean rewrites with the reasoning explained. Use before any send, in about thirty seconds.
- **`dependency-warden`** — The safe path through any major version bump, as a reusable checklist. Use when the user is about to take a major upgrade and wants the steps that prevent the classic disasters.
- **`devflow-engineer`** — Write a clean conventional commit message from a diff or change description. Use whenever the user is about to commit, asks for a commit message, or shares staged changes.
- **`devops-sentinel`** — The ten checks that catch most bad deploys before they leave the driveway. Use as a fast gate before any production deploy when there's no custom checklist yet.
- **`digital-declutter`** — The weekend digital cleanup as a step-by-step checklist with safe stopping points. Use when the mess has reached the point of action, one bounded session at a time.
- **`docs-engineer`** — Paste a README and get the three fixes that most improve a stranger's first five minutes. Use before publishing a repo or when onboarding feedback says setup is confusing.
- **`ecommerce-operator`** — Turn a product photo description and bullet facts into one publishable product description. Use for a quick single-product page without the full catalog treatment.
- **`errand-router`** — Keep one running errand list with zones and deadlines that gets swept weekly and never silently grows. Use when the user wants an errand list started, added to, or reviewed.
- **`error-budget-keeper`** — The five sections every postmortem needs, sized for small teams. Use when the user wants to run their first postmortem or standardize how incidents get written up.
- **`essay-coach`** — Test a pasted thesis against the three tests of a workable essay claim in one pass. Use when a student wants a fast verdict on whether their thesis can carry an essay.
- **`event-planner-pro`** — Turn an event's basic shape into a starter minute-by-minute show timeline; use for any event to see what a real run-of-show looks like.
- **`everyday-pa`** — A morning readout of the three emails that actually need the user today. Use at the start of the day or whenever the user asks what in their inbox matters.
- **`exam-crammer`** — Produce a two-week exam study plan from a syllabus and an exam date in one pass. Use when an exam is about two weeks out and the student has no plan, only a syllabus and rising dread.
- **`family-coordinator`** — The fridge-door summary of the family's week ahead, built in five minutes on Sunday. Use every Sunday evening as the one habit that catches the chaos early.
- **`farm-market-vendor`** — Write three honest, stopping-power signs for your stand from what you're selling this week; use before any market day.
- **`finance-butler`** — Find every recurring charge hiding in pasted statements and list them with annual cost. Use as a first sweep before any subscription cleanup.
- **`fitness-coach-desk`** — Get the weekly client check-in script that takes five minutes and actually gets replies. Use to start a check-in habit this week, even with zero systems.
- **`focus-architect`** — A guided 50-minute single-task sprint with a hard scope line and a clean exit; use when you need one thing finished and your attention keeps sliding off it.
- **`followup-machine`** — Draft a single follow-up nudge that adds value instead of just bumping the thread. Use whenever a reply is overdue and 'just checking in' is on the tip of your fingers.
- **`freelance-agency-desk`** — Generate the problem-first proposal skeleton for any project from a short brief; use before writing any proposal from scratch.
- **`frontend-finisher`** — Check a UI against the eight accessibility issues most products ship with, in fifteen minutes. Use on any page before it goes public, or as a first look at an inherited frontend.
- **`ghostwriter-desk`** — Paste three samples of someone's writing and get a starter voice profile back; use to see voice modeling work before onboarding a real client.
- **`gift-genius`** — Build the master list of birthdays, anniversaries, and dates the user must not miss. Use once to set up, then whenever a new person or date enters the picture.
- **`git-wizard`** — Build a correct .gitignore for your exact stack, and clean up files already tracked by mistake. Use when starting a repo or when build artifacts keep showing up in diffs.
- **`goal-tracker`** — Give a blunt feasibility pass on a list of goals against the hours that actually exist; use at term start, new year, or any moment of excessive ambition.
- **`grant-writing-studio`** — Turn one mission paragraph plus a funder's guidelines into a letter-of-inquiry skeleton tailored to that funder. Use when the user wants to approach a funder and needs the LOI started today.
- **`habit-forge`** — Build a one-glance weekly habit scorecard sized to what the user will actually fill in; use when starting tracking or when a tracker was abandoned.
- **`history-guide`** — Provide a reusable cause-and-effect timeline format for any historical period with a worked entry. Use when starting to study any period, or to convert an existing date list into causal form.
- **`hoa-community-manager`** — Draft courteous, firm-when-needed dues reminders tuned to a resident's payment history; use whenever assessment reminders need to go out.
- **`homeschool-planner`** — The homeschool week on one flexible page, per child. Use every weekend to set the week, or mid-week to re-plan after life happens.
- **`household-manager`** — Turn meal plans and scattered scraps into one clean, deduplicated grocery list. Use before a grocery run or when notes and requests have piled up all week.
- **`inbox-commander`** — Produce a morning summary of what in the inbox actually needs you, in three lines; use daily before opening email, so email does not open you.
- **`insurance-agency-aide`** — Draft a complete quote follow-up sequence in your agency's voice from one quote's details; use right after any quote goes out.
- **`kids-homework-helper`** — Three hints for any homework problem, from nudge to almost-there, never the answer. Use when a child is stuck and a parent wants to help without just telling.
- **`landlord-assistant`** — Produce clean drafts of routine tenant notices like entry, rent reminders, and policy updates; use whenever a standard notice needs writing.
- **`language-learning-coach`** — Get a fresh 15-minute practice menu for your language and level, in under a minute. Use daily, especially on days when motivation is the scarce resource.
- **`language-tutor`** — Deliver one genuinely useful phrase each day with usage notes and a memory hook. Use at the start of the day, or whenever the learner asks for their daily phrase.
- **`lecture-digestor`** — Paste raw lecture notes and get the one-page version with gaps marked. Use after any lecture for a fast, honest compression of what you captured.
- **`legal-office-clerk`** — Generate a thorough client intake template tailored to a small practice's matter types. Use when building or upgrading the firm's intake process.
- **`life-admin-clerk`** — Surface every expiry date the household is currently gambling on, in one sitting. Use when the user wants to know what's expiring or has ever been burned by a lapsed document.
- **`linkedin-outreach-pro`** — Rewrite a draft LinkedIn connection request so it reads honest, specific, and worth accepting. Use on any draft before it goes out.
- **`math-mentor`** — Serve one daily math problem at the student's level with a three-rung hint ladder. Use each day the student checks in, or whenever they ask for today's problem.
- **`meal-planner`** — Three tonight-ideas built from what's already in the kitchen, decided in two minutes. Use at 5pm on any day the plan didn't survive.
- **`meeting-master`** — Estimate what a recurring meeting really costs in attendee-hours and money, and judge whether it earns it; use before accepting or renewing any recurring invite.
- **`membership-org-manager`** — Draft a new-member welcome message series that starts engagement right in the first two weeks; use when onboarding new members or fixing a weak welcome.
- **`memory-athlete`** — Paste a list and get three different mnemonics for it, ready to test. Use for any list that must be remembered by a date, from anatomy to a speech's points.
- **`memory-keeper`** — One good question a day worth answering, filed with its date into a simple record. Use when the user wants a daily journaling prompt or a tiny memory habit.
- **`morning-anchor`** — Put the user's morning routine on one card in two sizes and iterate it weekly. Use when the user wants their routine written down, simplified, or reviewed after a week of use.
- **`move-manager`** — The master pre-move checklist people wish they'd had last time, grouped by weeks-out. Use when the user wants a moving checklist or asks what they are forgetting.
- **`multichannel-sequencer`** — Generate a ready-to-adapt 3-touch starter sequence \u2014 email, LinkedIn, email \u2014 for one ICP in minutes. Use to get a first coordinated motion running today.
- **`newsletter-chief`** — Rank five subject line variants with stated reasons rather than vibes; use right before every send, when the issue is done but the subject line is a shrug.
- **`nonprofit-organizer`** — Draft a specific, warm donor thank-you letter from gift details; use right after any donation arrives.
- **`notetaker-pro`** — Clean raw meeting scrawl or reading notes into structured, linkable entries without losing your words; use on any note too messy to trust in a month.
- **`okr-navigator`** — Paste your existing OKRs and get a hard critique of vague, sandbagged, or fantasy ones; use before the quarter locks, while rewrites are still free.
- **`oss-maintainer`** — Bug and feature templates that produce reports maintainers can act on. Use when the user's issue queue is full of unusable reports or they are setting up a new repository.
- **`pair-programmer`** — Explain your problem once and get back the single question most likely to unblock you. Use when the user is stuck and wants a fast nudge rather than a full session.
- **`parent-homework-coach`** — A 10-minute rescue plan for a homework battle already in progress: reset the room, restart the work, save the night. Use mid-meltdown, when nothing is getting done and everyone is fried.
- **`perf-profiler`** — A fair benchmark setup in five steps, ready to fill in and run. Use when the user wants to measure something quickly without designing a methodology from scratch.
- **`pet-assistant`** — Build the one-page pet profile that sitters, boarders, and vet front desks all ask for. Use when the user wants a pet profile, info sheet, or care card.
- **`photo-curator`** — Give three caption angles for any photo the user describes; use when a post is sitting in drafts because the words won't come.
- **`podcast-producer`** — Generate the episode page format listeners actually use, pre-filled from your episode details; use when setting up a show's notes format or upgrading pages that are just a paragraph and a link.
- **`poetry-workshop`** — Deliver a daily writing prompt with one craft focus attached; use every morning or whenever the page is blank, to build a writing practice fifteen minutes at a time.
- **`pro-exams-study-desk`** — Find the realistic study hours hiding in a working week and rate each slot's quality for deep or light study. Use when the user says they have no time to study or wants to know what their schedule can support.
- **`project-pilot`** — Everything to nail down before a project starts, checked in fifteen minutes; use before committing money or announcing dates to anyone.
- **`reading-butler`** — Sort a to-be-read pile into next, someday, and admit-it-never with honest criteria. Use when the user mentions an out-of-control book pile or wants their reading list sorted.
- **`reading-comprehension-coach`** — Turn any pasted passage into comprehension questions with answer locations. Use to self-quiz after a reading or to check that an assigned text was actually understood.
- **`realestate-wingman`** — Tighten and warm an existing listing description while keeping every stated fact intact. Use when copy exists but reads flat, bloated, or cold.
- **`recruiter-copilot`** — Draft one personalized candidate outreach message that doesn't read like spam; use before sending any sourcing message.
- **`refactor-surgeon`** — A 10-point pass that grades any file's structural health in minutes. Use when reviewing unfamiliar code, prioritizing cleanup, or sanity-checking your own module before review.
- **`report-builder`** — Deliver the update format busy readers finish — lede, deltas, risks, ask — tuned to the user's cadence with one worked example; use to fix a rambling status format today.
- **`research-navigator`** — Convert any pasted reference into clean APA, MLA, or Chicago format with missing fields flagged. Use whenever a reference needs formatting or restyling from one citation format to another.
- **`restaurant-front-desk`** — Paste any single restaurant review and get back the public reply that helps. Use for the review sitting unanswered right now.
- **`sales-call-coach`** — Generate sharp, non-generic discovery questions for a specific prospect and offer. Use before any first call, or when your discovery keeps producing polite answers and no information.
- **`salon-studio-manager`** — Generate ready-to-fill aftercare card templates for your top five services in one pass. Use to standardize aftercare today, before drafting per-client messages.
- **`science-lab-partner`** — Provide the standard lab report skeleton with what belongs in each section and self-check questions. Use when a student faces a blank page before any lab write-up.
- **`script-doctor`** — Adapt twenty proven hook patterns to your specific topic with ready-to-say lines; use when planning content for the week or staring at a topic with no opening in mind.
- **`security-reviewer`** — A pre-launch defensive pass anyone on the team can run in an afternoon. Use before shipping anything public-facing or after inheriting a project with unknown security posture.
- **`smb-ops-desk`** — Build a ranked list of who owes you money, sorted by age and amount, from whatever records exist. Use when the user wants to know where their cash is stuck.
- **`social-secretary`** — Draft the graceful yes, no, or maybe to any invitation, in the user's own voice. Use the moment an invitation needs answering and the right words aren't there.
- **`social-strategist`** — Reshape one idea natively for three platforms with distinct hooks and formats; use whenever one good idea deserves more than one post, or a strong post on one platform should travel.
- **`songwriting-partner`** — Produce twenty titles that suggest a song rather than label a topic; use at the start of a write or when a finished song still has a placeholder name.
- **`sop-writer`** — Generate a fill-in skeleton for documenting any recurring task, pre-seeded from a two-minute description; use to start documenting today without the full interview.
- **`sprint-mechanic`** — The ticket format that prevents mid-sprint surprises, ready to adopt today. Use when the user wants a standard ticket structure or asks why their tickets keep going sideways.
- **`story-smith`** — Generate ten story premises with built-in conflict from your interests; use when starting fresh, between projects, or when every idea feels either empty or already taken.
- **`str-host-manager`** — Draft gracious public replies to guest reviews, positive and negative, that read well to the next guest; use whenever a review needs a public response.
- **`study-coach`** — Convert any notes into clean question-and-answer flashcards ready for review or import. Use when the student pastes notes, a chapter, or a vocab list and wants cards to drill from.
- **`study-group-director`** — Convert any solo study task \u2014 flashcards, rereading, problem sets, essay outlining \u2014 into a structured group format in minutes. Use when the group is meeting but nobody knows what to actually do together.
- **`study-group-facilitator`** — A fill-in study session plan that prevents social hour. Use when a group wants structure fast without a full facilitation setup.
- **`teacher-aide`** — A four-level rubric skeleton adaptable to any assignment in minutes. Use when you need consistent grading language fast, before building a full custom rubric.
- **`test-prep-strategist`** — Find where section time actually goes with a simple per-block time map and one finding. Use after any timed practice section when time ran out or finished suspiciously early.
- **`test-smith`** — Rename tests so failures explain themselves without opening the file. Use when a suite's failure output reads like a phone book, or before sharing a suite with collaborators.
- **`thesis-advisor`** — Your thesis timeline back-planned from the deadline on one page. Use the day the deadline becomes real, or whenever the current plan stops being believable.
- **`time-audit-analyst`** — Set up the lightest time-tracking format that still supports leak-finding and utilization math; use when starting tracking or after abandoning a heavier system.
- **`travel-agency-desk`** — Format any trip's bookings into the day-by-day itinerary layout clients love to receive; use to see agency-polish structure on a real trip.
- **`travel-concierge`** — Generate a trip-specific packing list from destination, duration, and planned activities. Use once a trip is booked or whenever the user says they need to pack.
- **`tutoring-center-admin`** — Turn one session's tutor notes into the after-session note that justifies the fee; use after any tutoring session.
- **`virtual-classroom-producer`** — Generate age-appropriate icebreakers and warm-ups for online sessions in seconds, matched to class size and platform. Use in the ten minutes before any live session that needs to start warm.
- **`visual-brief-writer`** — Generate the one-page design brief template designers thank you for, pre-filled from a short project description; use at any project kickoff.
- **`wardrobe-valet`** — Run the 30-minute closet inventory that maps what's owned, worn, and orphaned. Use when the user wants to start organizing their wardrobe or says they have nothing to wear.
- **`weekly-review-coach`** — Close the week in five minutes with three questions and one adjustment for next week; use any Friday, especially the ones too busy for a full review.
- **`youtube-strategist`** — Rank five candidate titles for the creator's next video with reasons; use whenever a video is done but the title is still a working title.
- **`zine-publisher`** — Generate ten zine themes with a first-page idea for each; use when someone wants to make a zine and doesn't know about what.

</details>

## Also from Moltline

- **Live MCP servers (free tiers, no signup):** `https://mcp.moltlinestudio.com/`
  — 19 endpoints (code review, agent governance, date math, CSV analytics,
  humanizer, merchant math, shipping and dropship economics, Shopify prep,
  a portable memory graph, vision math, SKILL.md lint, and more) exposing
  132 tools, 92 of them free with no signup.
- **Full persona bundles** (persona + focused skills each): on
  [Agensi](https://www.agensi.io) and ClawMart — search "GarphenGate" / "Moltline".
- **Agent protocol reference:** how x402, AP2, ACP, UCP, MPP and A2A are
  actually implemented on one live domain — [https://moltlinestudio.com/protocols.html](https://moltlinestudio.com/protocols.html).
- **All-Access license** ($19/mo, unlocks premium tools on every server, crypto
  accepted): [moltlinestudio.com](https://moltlinestudio.com).

## Support

**support@moltlinestudio.com** — first response within 24h, confirmed defects
fixed within 30 days. That commitment is written into every product we ship.

## License

Free skills in this repository may be used with any AI agent, personally or
commercially. Redistribution or resale of the skills themselves as a competing
pack/catalog, or use of the "Moltline" name/branding, requires written
permission (see [LICENSE](LICENSE)). The premium catalog, personas, and server
implementations are proprietary and not part of this repository.

© 2026 Moltline Studio.
