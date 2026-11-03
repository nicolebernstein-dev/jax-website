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
### Engagement state — 2026-11-03
**Status:** at risk — Form redirect working; Salesforce sync blocked — awaiting Pardot completion action fix and test submission

**Done this session**
- Provided detailed completion action sequence for Pardot form (assign → campaign → email → notify → tag)
- Documented 30-registration threshold changes (Status and email swap to Waitlist)

**Open items**
- Add 'Assign prospect to user/queue' completion action before 'Add to Salesforce Campaign' in Pardot form
- Assign existing test prospects to a user in Pardot to trigger sync
- Submit new test form with fresh +test address after fix is applied
- Verify lead and campaign member appear in Salesforce within 10–15 minutes
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- At 30 registrations, change both 'registered' to 'waitlist' in Pardot Thank You Code
- Preview both thank-you pages on computer and phone; report desired changes

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Waitlisted prospects must also sync to Salesforce (keep assignment step unchanged)
- Thank You Code uses postMessage signal + try/catch window.top.location redirect to handle browser blocking
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links

**Blockers**
- Pardot form missing 'Assign prospect to user/queue' completion action — prevents lead creation in Salesforce

**Next**
- Add 'Assign prospect to user/queue' completion action to Pardot form (place before 'Add to Salesforce Campaign')
- Assign existing test prospects to a user in Pardot to trigger retroactive sync
- Submit new test form with fresh +test email address
- Verify lead and campaign member appear in Salesforce within 10–15 minutes
- Report results before proceeding with Yoast SEO and thank-you page preview

**Checked live on 2026-11-03:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-03
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | NY World Tour Event Registration Page |
| Session | `e68d87da-5721-417e-adfc-c7124417d40e` |
**In its own words (excerpt):**
Here's the order to use in the form's **Completion Actions**, top to bottom:

1. **Assign prospect to user** (or **Assign prospect via Salesforce active assignment rule**, or **Assign to queue**, whichever your other Jax forms use). This is the step that makes Pardot create the lead in Salesforce.
2. **Add to Salesforce Campaign:** `event-26-12-ny-world-tour-edu`, Status **Registered**.
3. **Send autoresponder email:** `event-26-12-ny-world-tour-edu – Registration Confirmation`.
4. **Notify user** (optional): the event owner, if you want an email for each registration.
5. **Add tag** (optional): `event-26-12-ny-registered`.

**At 30 registrations**, change only two of these:
- Step 2: Status → **Waitlisted**
- Step 3: email → **Waitlist Confirmation**
- (and step 5's tag → `event-26-12-ny-waitlisted`, if you use it)

Leave step 1 as it is. Waitlisted people need to sync to Salesforce too.

Once you've saved the form, assign your existing test prospects to a user, then submit one more test with a new +test address. Tell me when that's done and I'll check Salesforce for the lead and the campaign member.

Sources: engagement context (context/handoff.md) and the D01 forms guide from ea

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
