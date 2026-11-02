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
**Status:** at risk — Form redirect working; Salesforce sync blocked — needs 'Assign prospect to user' action in Pardot before campaign sync can work.

**Done this session**
- Confirmed Salesforce campaign has 0 members and no leads created today
- Identified root cause: prospects must be assigned to user/queue before Salesforce sync occurs
- Provided fix: add 'Assign prospect to user' completion action above 'Add to Salesforce Campaign' in Pardot

**Open items**
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Add 'Assign prospect to user/queue' completion action before 'Add to Salesforce Campaign' in Pardot form
- Assign existing test prospects to a user in Pardot to trigger sync
- Submit new test form with fresh +test address after fix is applied
- At 30 registrations, change both 'registered' to 'waitlist' in Pardot Thank You Code
- Preview both thank-you pages on computer and phone; report desired changes

**Decisions**
- Thank You Code uses postMessage signal + try/catch window.top.location redirect to handle browser blocking
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links
- Prospect assignment to user/queue is required before Salesforce sync

**Blockers**
- Pardot form missing 'Assign prospect to user/queue' completion action — prevents lead creation in Salesforce

**Next**
- Add 'Assign prospect to user/queue' completion action to Pardot form (place before 'Add to Salesforce Campaign')
- Assign existing test prospects to a user in Pardot to trigger retroactive sync
- Submit new test form with fresh +test email address
- Verify lead and campaign member appear in Salesforce within 10–15 minutes
- Report results and proceed with Yoast SEO settings and thank-you page preview

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
Glad the form and redirect are working now.

On timing: once a prospect is set up to sync, the new lead and campaign member usually show up in Salesforce within a few minutes, and almost always within 10–15. If nothing has appeared after that, more waiting won't help. Something in the setup is stopping it.

That's what's happening here. I checked Salesforce just now:
- The campaign **event-26-12-ny-world-tour-edu** has **0 members**.
- **No leads** were created today, and there's no lead for any of your +test addresses.
- The only matching contact is your own record, and it was last changed on October 12.

So the problem isn't that the campaign member is missing. The person never reached Salesforce at all, and a campaign member can't exist until there's a lead or contact to attach it to.

**The likely cause:** Pardot only creates a Salesforce lead once a prospect is **assigned to a user or queue**. Unassigned prospects stay in Pardot only, so "Add to Salesforce Campaign" has no record to add.

**How to fix it:**
1. Open the form's **Completion Actions** in Pardot.
2. Add **Assign prospect to user** (or to a queue or active assignment rule, whichever your other Jax forms use), and p

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
