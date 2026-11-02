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
### Engagement state — 2026-11-02
**Status:** on track — Member statuses live; WordPress draft ready; awaiting Pardot forms A & B to publish

**Done this session**
- Ran member status update script successfully
- Verified 4 member statuses now live on campaign (Registered, Waitlisted, Attended, No Show)
- Confirmed WordPress draft page built and accessible at /nyc-education-ai-2026/

**Open items**
- Build Pardot Form A with 'Add to Salesforce Campaign' action set to Registered
- Build Pardot Form B with 'Add to Salesforce Campaign' action set to Waitlisted
- Provide Pardot Form A link for landing page
- Provide confirmation email text for forms
- Add Form A to WordPress page and publish once forms ready
- Write Pardot guide documentation (optional)

**Decisions**
- Campaign type: Seminar/Conference
- Campaign status: Planned and Active
- Event date: December 2, 2026
- Member statuses: Registered (default), Waitlisted, Attended, No Show
- Preserve existing 'Connected' status; new statuses added after it
- Use Registered count for seat availability, not Responded total (Waitlisted counts as Responded)

**Blockers**
- None

**Next**
- Build Pardot Form A (Registered action) and Form B (Waitlisted action)
- Send Form A link and confirmation email text
- Add Form A to WordPress page and publish

**Checked live on 2026-11-02:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-02
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | NY World Tour Event Registration Page |
| Session | `e68d87da-5721-417e-adfc-c7124417d40e` |
**In its own words (excerpt):**
I ran the script once, unchanged, and it finished without errors. It updated 2 existing statuses and inserted 2 new ones. A query of the org afterwards shows campaign `event-26-12-ny-world-tour-edu` now has these member statuses:

| Order | Status | Default | Counts as Responded |
|---|---|---|---|
| 1 | **Registered** | ✅ | Yes |
| 2 | **Waitlisted** | | Yes |
| 3 | Connected (already there, left as it was) | | No |
| 4 | **Attended** | | Yes |
| 5 | **No Show** | | No |

Waitlisted is marked as Responded, so Salesforce's Responded count includes waitlisted people. To see how many seats are taken, use the Registered count, not the Responded total.

**Where things stand**
- **Done and checked:** the campaign and its member statuses, and the WordPress draft page [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065) at `/nyc-education-ai-2026/`. The page isn't published, and its form slot still says "Registration form coming soon".
- **Next, you:** build Pardot Form A and Form B. Form A's "Add to Salesforce Campaign" action should set **Registered**, and Form B's should set **Waitlisted**. Then send me Form A's link and your confirmation email text.
- **Next, me:** add 

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
