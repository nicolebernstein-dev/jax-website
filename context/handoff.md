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
**Status:** waiting — Campaign event-26-12-ny-world-tour-edu created in production; awaiting approval to add member statuses

**Done this session**
- Confirmed campaign event-26-12-ny-world-tour-edu exists in jaxconsultingllc org (Id 701UJ00001boDNdYAM)

**Open items**
- Approve campaign on the card to proceed with member status changes
- Add member statuses (Registered, Waitlisted, Attended, No Show)
- Build WordPress draft page at /nyc-education-ai-2026/
- Write Pardot guide documentation

**Decisions**
- Campaign type: Seminar/Conference
- Campaign status: Planned and Active
- Event date: December 2, 2026
- Member statuses: Registered (default), Waitlisted, Attended, No Show

**Blockers**
- None

**Next**
- Await approval on the card
- Add member statuses to campaign in org
- Create WordPress draft page
- Write Pardot guide

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
I created the campaign **event-26-12-ny-world-tour-edu** in `jaxconsultingllc` (Id `701UJ00001boDNdYAM`) and checked it in the org. It's set to Seminar / Conference, Planned and Active, dated December 2, 2026.

The next step is waiting for your approval on the card. That command changes the campaign's member statuses. Salesforce set the defaults to "Sent" and "Responded", so it renames those to **Registered** (the default) and **Waitlisted**, and adds **Attended** and **No Show**. Once you approve it, I'll check the statuses in the org, then build the WordPress draft page at `/nyc-education-ai-2026/` and write the Pardot guide.
<!-- orchestrate:session-state:end -->
