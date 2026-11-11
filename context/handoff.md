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
**Status:** on track — Case study draft 3101 rebuilt with proper card modules; ready for WordPress metadata & browser testing

**Done this session**
- Rebuilt case study draft 3101 with acf/card-simple blocks (Challenges, Solution, Results)
- Verified card modules saved and readable from WordPress; no client names exposed
- Documented block code extraction method for future case studies

**Open items**
- Set Case Study category and matching topic on draft 3101
- Add featured image to draft 3101
- Add meta description in Yoast on draft 3101
- Review & decide whether to reword second Results card (starts with '$1M+' like first)
- Preview draft 3101 in browser (desktop & mobile); verify card layout, spacing, form
- WordPress admin: back up live database, install Better Search Replace, run dry run & execute link migration
- Recheck all 20 pages and test every link after link migration completes
- Test live page form submission and thank-you page redirect; confirm Pardot email greeting

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes 28px; 'Spaces are limited.' 14px with line space after Reserve button
- Link migration: case-study replacement must run first to avoid old addresses
- Extract block code from Code editor first, then build new pages from it

**Blockers**
- Link migration runbook awaiting WordPress admin execution (back up, install Better Search Replace, dry run, execute, clear cache)
- 17 of 20 audit pages not yet tested for sandbox/localhost links; migration may surface unmapped addresses

**Next**
- Set category, topic, featured image, and meta description on draft 3101
- Preview draft 3101 in browser and verify card layout, spacing, form behavior
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
I saved draft 3101 with the same card modules as the Continuing Studies example. It's still a draft, so nothing is live. I read it back from the site afterwards: the content is now three `acf/card-simple` blocks, the theme displays them as normal card sections, and the status is still draft.

- **Draft:** [$1M in Delivery Value in 30 Days: AI-Accelerated Salesforce for Higher Education](https://www.jaxconsult.com/?post_type=case-study&p=3101)
- **Challenges:** 4 cards, white background, left-aligned.
- **Solution:** 4 cards on the black-to-blue gradient.
- **Results:** 4 cards with the checkmark icon, centered, under the heading "RESULTS:".
- **What didn't change:** Mission, Salesforce Products, the title and the web address. I checked again and no client names appear anywhere.

You can now edit each card in the block editor the same way you would on the example page.

**Still to do in WordPress before you publish:**
1. Set the Case Study category and the matching topic. Both are still empty.
2. Add a featured image. There isn't one yet.
3. Add a meta description in Yoast. There isn't one yet.
4. Decide whether to reword the second Results card. It starts with "$1M+", the same as t

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
