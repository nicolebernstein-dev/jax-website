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
**Status:** on track — Meta description drafted; draft 3101 title & Mission updated by another editor; category, topic & Yoast paste still pending

**Done this session**
- Drafted three meta description options (149, 139, 144 characters) for draft 3101
- Verified draft 3101 live state: title, Mission, featured image now set by another editor

**Open items**
- Paste meta description into Yoast SEO panel on draft 3101 (choose one of three options provided)
- Set Case Study category and matching topic on draft 3101
- Preview draft 3101 in browser (desktop & mobile); verify card layout, spacing, form
- Publish draft 3101 to live
- WordPress admin: execute link migration runbook (back up, install Better Search Replace, dry run, execute, clear cache)
- Recheck all 20 pages and test every link after link migration completes
- Review & decide whether to reword second Results card (starts with '$1M+' like first)

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes 28px; 'Spaces are limited.' 14px with line space after Reserve button
- Link migration: case-study replacement must run first to avoid old addresses
- Hero image uses standard sans-serif (not Jax brand font); designer can rebuild if exact match needed
- Focus keyphrase for Yoast: AI-accelerated Salesforce

**Blockers**
- Link migration runbook awaiting WordPress admin execution
- 17 of 20 audit pages not yet tested for sandbox/localhost links; migration may surface unmapped addresses

**Next**
- Paste chosen meta description into Yoast SEO panel on draft 3101
- Set category and topic on draft 3101
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
Here's a meta description for draft 3101. It's 149 characters, which is under Yoast's limit of about 155, so search results won't cut it off:

> **A university education center used AI-accelerated Salesforce delivery to gain $1M+ in value in 30 days, finishing a month early and 15% under budget.**

Two other options, if you'd like a different angle:
- **Leads with products (139 characters):** How AI-accelerated delivery with Education Cloud and Agentforce produced $1M+ in value in 30 days for a university, early and under budget.
- **Leads with the headline (144 characters):** $1M in delivery value in 30 days: how a university moved to Education Cloud, added an Agentforce assistant, and finished early and under budget.

**Suggested focus keyphrase:** AI-accelerated Salesforce

**You'll need to paste it into Yoast yourself.** I don't have a way to set it. The draft's Yoast fields aren't available through the WordPress connection. To add it, open draft 3101, go to the Yoast SEO panel, and paste it into the Meta description field.

**The draft has changed since I last saved it.** I just checked the live draft, and someone has edited it:
- The title is now "$1M in Delivery Value in 30 

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
