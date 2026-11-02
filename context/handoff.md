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
**Status:** at risk — Form submission fails after Pardot acceptance; thank-you redirect broken. Need Pardot form audit.

**Done this session**
- Identified form submission error occurs in Pardot completion actions, not landing page
- Confirmed Pardot prospect created (ID 98056183) but thank-you redirect fails
- Confirmed Salesforce campaign has 0 members — lead sync not working

**Open items**
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Check test prospect activities: form success listed? confirmation email arrived?
- If form success + no email: verify autoresponder template ticked 'Available for Use' and completion action points to it
- If form success + email arrived: test thank-you code by removing from Thank You Code tab, resubmit, check if error clears
- Add 'Assign prospect to user/queue' completion action before 'Add to Salesforce Campaign' in Pardot form
- Preview both thank-you pages on computer and phone; report desired changes
- At 30 registrations, change 'registered' to 'waitlist' in Pardot Thank You Code Step 6

**Decisions**
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Thank-you page URLs: /nyc-education-ai-2026-registered/ and /nyc-education-ai-2026-waitlist/
- Cutover at 30 registrations: single Step 6 edit in Pardot to change Thank You Code URL
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links
- Pardot Thank You Code sends signal only; landing page listener handles redirect (origin-locked to go.jaxconsult.com)

**Blockers**
- Pardot form completion actions failing — thank-you redirect not executing after prospect creation
- Salesforce lead sync broken — campaign has 0 members despite form submissions
- Google Workspace connection expired — cannot verify event address in Google Doc

**Next**
- Open test prospect 98056183 in Pardot; check Activities for 'Form success' and whether confirmation email arrived
- Based on step 1 result, follow Pardot form audit path: check autoresponder template, thank-you code syntax, or layout template
- Add 'Assign prospect to user/queue' completion action to Pardot form before 'Add to Salesforce Campaign'
- Retest form submission after fixes; verify thank-you page opens in full window and prospect syncs to Salesforce

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
The good news is that your registration got through. Pardot created the prospect, so the form accepted the details. The error comes after that, when Pardot runs the form's final steps: the completion actions and the thank-you message. The page I added can't cause it, because it only acts once Pardot has finished and sent its signal. So the problem is in the Pardot form setup.

I can't open the form in Pardot from here. When I tried to read the prospect through the Pardot API, it returned "Access Denied". So these steps will help you find which part is failing.

**1. Check what Pardot finished.** Open the test prospect and look at its **Activities**:
- **Form success** listed, and no confirmation email in your inbox: the autoresponder step is the likely problem. Open the email template and check that **Autoresponder Emails** is ticked under "Available for Use". Then check that the completion action points to that template and not an old draft.
- **Form success** listed, and the email did arrive: the problem is in the thank-you part. Go to step 2.

**2. Test the thank-you part.** Edit the form and cut the script out of the **Thank You Code** tab (keep a copy). Save, then submit again

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
