# Handoff — current state

> **Rewritten at the end of every session.** This file is *now*; [`gotchas.md`](gotchas.md) is *forever*.
> If this file and [`../CONTEXT.md`](../CONTEXT.md) disagree, this one is newer.

**Last updated:** 2026-11-02 · **By:** <session or person>

---

## Where things stand

> **Not yet filled in.** — Where is the work right now, in two or three sentences? Someone picking
> this up cold reads this first.

## In progress

| What | State | Where it lives | Blocked on |
|---|---|---|---|
| | | | |

## Next steps

<!-- Ordered. The top item should be the one to do next, not the most interesting one. -->

1.

## Waiting on someone else

| What | Who | Since | Chased? |
|---|---|---|---|
| | | | |

## Things the next session should know

<!-- Anything true right now that is not obvious from the code: a half-finished refactor, a
     deliberately disabled test, a workaround that needs removing, a deploy that is half-applied.
     If you leave something in a strange state, this is where you say so. -->

-

<!-- orchestrate:session-state:start -->
<!-- Written by Orchestrate at the end of each session. Edits inside this block are
     replaced next session; anything OUTSIDE it is yours and is never touched. -->
### Engagement state — 2026-11-11
**Status:** on track — Hero image & newsletter copy ready; case study draft 3101 awaits WordPress metadata, browser test & publication

**Done this session**
- Created hero image (1200×630px) with navy, gradient, $1M headline, stat pills, chart—no client names
- Wrote newsletter copy (75 words + 35-word version) with headline, subhead, button text, alt text, tracking tags

**Open items**
- Set Case Study category and matching topic on draft 3101
- Add featured image to draft 3101 (hero image ready to upload)
- Add meta description in Yoast on draft 3101
- Review & decide whether to reword second Results card (starts with '$1M+' like first)
- Preview draft 3101 in browser (desktop & mobile); verify card layout, spacing, form
- Publish draft 3101 to live (required before newsletter link works)
- WordPress admin: back up live database, install Better Search Replace, run dry run & execute link migration
- Recheck all 20 pages and test every link after link migration completes

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes 28px; 'Spaces are limited.' 14px with line space after Reserve button
- Link migration: case-study replacement must run first to avoid old addresses
- Extract block code from Code editor first, then build new pages from it
- Hero image uses standard sans-serif (not Jax brand font); designer can rebuild if exact match needed

**Blockers**
- Link migration runbook awaiting WordPress admin execution (back up, install Better Search Replace, dry run, execute, clear cache)
- 17 of 20 audit pages not yet tested for sandbox/localhost links; migration may surface unmapped addresses

**Next**
- Upload hero image to draft 3101 as featured image
- Set category, topic, and meta description on draft 3101
- Preview draft 3101 in browser and verify card layout, spacing, form behavior
- Publish draft 3101 to live
- WordPress admin: execute link migration runbook; report completion
- Recheck all 20 pages and test every link after migration completes

**Checked live on 2026-11-11:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-11
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | CGOE Case Study |
| Session | `457065f1-5972-4c2f-b430-ee65e7eb64ba` |
**In its own words (excerpt):**
I made the hero image and wrote the newsletter copy. Both are attached to this session. I didn't upload or change anything in WordPress.

**Hero image** (1200 × 630 px)
- It uses Jax navy with the same black-to-blue gradient as the case study's Solution section.
- The headline is a large "$1M", with "in delivery value in 30 days" underneath.
- Below that are three stat pills: 5,817 hours saved, 1 month early, and about 15% under budget.
- A rising bar chart sits on the right. No client names appear.
- The size works as the case study's featured image too, which is still on your to-do list.

**Newsletter summary** (about 75 words)
> A university's graduate and professional education center needed a large Salesforce move done on a fixed budget and timeline. They also wanted AI their staff could trust. With Education Cloud, Agentforce and Revecast Orchestrate, the team delivered more than $1M in value in 30 days. The project saved 5,817 hours, finished a month early and came in about 15% under budget. Staff rated the new Agentforce assistant 8.6 on average across 339 conversations.

The document also has:
- a headline and optional subhead
- a shorter version, about 35 words
- the butt

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
