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
**Status:** at risk — Case study draft created & saved. Link migration runbook awaiting WordPress admin execution. Karen notification still blocked.

**Done this session**
- Created draft case study (entry 3101) on live WordPress from 5 slides; saved and verified as draft
- Structured case study with Mission, Challenges, Solution, Results matching Continuing Studies layout

**Open items**
- WordPress admin: back up live database, install Better Search Replace, run dry run of 3 replacements in order
- WordPress admin: execute replacements, clear caches, spot-check for pantheonsite and localhost in page source
- Recheck all 20 pages and test every link after migration completes
- Test live page in browser on computer and phone; verify form position, heading sizes, spacing
- Submit test registration and confirm thank-you page redirect works
- Confirm Pardot email greeting wording matches 'Hi,' or report actual text
- Remove 2 test leads from Salesforce campaign
- Case study: set Category (Case Study), Topic (Higher Education), Featured image, Meta description; review Results wording for repetition; optionally rebuild Challenges/Solution/Results with card blocks

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes 28px; 'Spaces are limited.' 14px with line space after Reserve button
- Link migration: case-study replacement must run first to avoid old addresses
- Case study results: $1M+ delivery value, $1M+ extra scope, month early & 15% under budget, 8.6/10 staff satisfaction

**Blockers**
- Slack token type does not allow message search or member lookup—cannot identify or contact Karen without external input
- 17 of 20 audit pages not yet tested for sandbox/localhost links; migration may surface unmapped addresses

**Next**
- WordPress admin: execute link migration runbook (back up, install Better Search Replace, dry run, execute, clear cache, spot-check)
- WordPress admin: report completion; session will recheck all 20 pages and test every link
- Case study editor: set Category, Topic, Featured image, Meta description; review Results wording
- Provide Karen's Slack member ID, alternative contact channel, or send draft notification yourself

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
I created the case study as a draft on www.jaxconsult.com. It is not live. I read it back afterwards and confirmed it saved as a draft.

- **Draft:** [$1M in Delivery Value in 30 Days: AI-Accelerated Salesforce for Higher Education](https://www.jaxconsult.com/?post_type=case-study&p=3101) (Case Studies, entry 3101)
- **Planned address:** /insights/ai-accelerated-salesforce-higher-education/

**One thing to know first:** the text I wrote for the preview last turn wasn't kept when this session resumed. I rewrote it from your five slides in the same structure. Please read it through rather than assuming it matches the preview word for word.

**What's in it.** It follows the same layout as the Continuing Studies case study:
- **Mission:** a university's graduate and professional education center. Stanford, CGOE and the other customers on the slides are not named.
- **Salesforce Products:** Education Cloud, Agentforce, Data360, Salesforce Knowledge and Revecast Orchestrate.
- **Challenges (4 cards):** the large migration scope, staff answering the same questions over and over, AI that staff have to be able to trust, and a fixed budget and timeline.
- **Solution (4 cards, blue band):** s

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
