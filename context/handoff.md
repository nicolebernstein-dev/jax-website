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
**Status:** at risk — WordPress draft page built; member statuses blocked on approval card; Pardot form link needed

**Done this session**
- Created WordPress draft page at /nyc-education-ai-2026/ (page 3065)
- Verified campaign member statuses in org; noted new 'Connected' status

**Open items**
- Approve card to add member statuses (Registered, Waitlisted, Attended, No Show)
- Obtain Pardot Form A link for landing page form slot
- Add member statuses to campaign after approval
- Publish WordPress page once form link is available
- Write Pardot guide documentation

**Decisions**
- Campaign type: Seminar/Conference
- Campaign status: Planned and Active
- Event date: December 2, 2026
- Member statuses: Registered (default), Waitlisted, Attended, No Show
- Preserve existing 'Connected' status; add new statuses after it

**Blockers**
- Approval card not yet approved to proceed with member status changes
- Pardot Form A link not yet provided for landing page

**Next**
- Approve the card to enable member status update
- Provide Pardot Form A link
- Add member statuses to campaign once approval runs
- Update WordPress page with Pardot form link and publish

**Checked live on 2026-11-02:** Google Workspace
### Last session — 2026-11-02
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | NY World Tour Event Registration Page |
| Session | `e68d87da-5721-417e-adfc-c7124417d40e` |
**In its own words (excerpt):**
I created the landing page as a WordPress draft and checked it on the site: [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065), page 3065, at `/nyc-education-ai-2026/`. It isn't published. The form slot shows "Registration form coming soon" until you send me the Pardot Form A link.

The member statuses are not set up yet. That change is waiting on the approval card. When you approve it, it renames "Sent" to **Registered** (the default) and "Responded" to **Waitlisted**, then adds **Attended** and **No Show**. A status called **Connected** has appeared on the campaign since the last check, so I'm leaving it as it is and adding the new statuses after it. Once it runs, I'll check the statuses in the org.

Sources: the Google Doc's Landing Page section · checked live: the campaign's member statuses, and the WordPress draft read back after I created it · not checked: who added the "Connected" status
<!-- orchestrate:session-state:end -->
