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
**Status:** at risk — Case study draft saved; link migration & module rebuild blocked on WordPress admin & theme code

**Done this session**
- Identified blocker: ACF block structure not accessible via API; HTML fallback created instead

**Open items**
- WordPress admin: back up live database, install Better Search Replace, run dry run & execute link migration
- Obtain Continuing Studies case study block code (Code editor → copy all) or duplicate & swap text manually
- Rebuild case study draft 3101 with proper card modules (Challenges, Solution, Results) once block structure known
- Set Category, Topic, Featured image, Meta description on case study
- Recheck all 20 pages and test every link after link migration completes
- Test live page in browser (desktop & mobile); verify form, heading sizes, spacing
- Submit test registration and confirm thank-you page redirect
- Confirm Pardot email greeting wording; remove 2 test leads from Salesforce campaign

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes 28px; 'Spaces are limited.' 14px with line space after Reserve button
- Link migration: case-study replacement must run first to avoid old addresses
- Case study results: $1M+ delivery value, $1M+ extra scope, month early & 15% under budget, 8.6/10 staff satisfaction

**Blockers**
- WordPress API returns finished HTML only, not ACF block code—cannot rebuild Challenges/Solution/Results as editable card modules without theme code
- Link migration runbook awaiting WordPress admin execution (back up, install Better Search Replace, dry run, execute, clear cache)
- Slack token type does not allow message search or member lookup—cannot identify or contact Karen without external input
- 17 of 20 audit pages not yet tested for sandbox/localhost links; migration may surface unmapped addresses

**Next**
- Send Continuing Studies case study block code (WordPress Code editor) or confirm manual duplicate & swap approach
- WordPress admin: execute link migration runbook; report completion
- Rebuild case study draft 3101 with proper card modules once block structure received
- Session will recheck all 20 pages and test every link after migration completes

**Checked live on 2026-11-11:** the repository
### Last session — 2026-11-11
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | CGOE Case Study |
| Session | `457065f1-5972-4c2f-b430-ee65e7eb64ba` |
**In its own words (excerpt):**
Not yet. I can only write the page content as code, and I can't see how the site's modules are put together.

**Why:** the Challenges, Solution and Results sections in the Continuing Studies example are ACF blocks from your theme. To recreate them I'd need each block's name and field names. The WordPress connection only returns the finished page HTML, not the block code underneath. The connected repository (`jax-website`) doesn't have the theme in it either; it only holds a Salesforce project skeleton. If I guessed the block names, I'd probably save blocks the editor can't open, so I wrote HTML that looks the same instead. That's also why those sections show up as Custom HTML in the editor instead of card modules.

**Two ways to get real modules:**

1. **Send me the example's block code (recommended, about 2 minutes for you).** Open the Continuing Studies case study in the WordPress editor, click the ⋮ menu at the top right, choose **Code editor**, then copy everything and paste it here or attach it as a text file. That shows me the exact block names and fields. I'd then rebuild draft 3101 with the same card modules and our text, so you can edit each card like any other. I'd confir

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
