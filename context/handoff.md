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
**Status:** at risk — Form redirect fixed with postMessage + fallback; awaiting test results. Salesforce sync still broken (0 members).

**Done this session**
- Identified browser blocking as cause of thank-you redirect failure
- Provided corrected Thank You Code with postMessage signal + window.top.location fallback
- Confirmed Salesforce campaign still has 0 members — lead sync not working

**Open items**
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Test form submission with nicole.bernstein+nyctest2@jaxconsult.com; report: error shown, thank-you page opened full window, email arrived
- Add 'Assign prospect to user/queue' completion action before 'Add to Salesforce Campaign' in Pardot form
- At 30 registrations, change both 'registered' to 'waitlist' in Pardot Thank You Code
- Preview both thank-you pages on computer and phone; report desired changes
- After test passes, verify prospect syncs to Salesforce campaign

**Decisions**
- Thank You Code uses postMessage signal + try/catch window.top.location redirect to handle browser blocking
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links

**Blockers**
- Salesforce lead sync broken — campaign has 0 members despite form submissions; needs 'Assign prospect to user/queue' completion action in Pardot

**Next**
- Test form with nicole.bernstein+nyctest2@jaxconsult.com using new Thank You Code
- Report: error shown, thank-you page opened full window, confirmation email arrived
- Add 'Assign prospect to user/queue' completion action to Pardot form before 'Add to Salesforce Campaign'
- Retest form submission; verify prospect syncs to Salesforce campaign and thank-you page opens

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
Testing again is fine. Two things to know first:

**1. Some browsers may block that code.** A form shown inside another page is often not allowed to send the whole browser window to a new page. Chrome and Safari can block this, and then the thank-you page either opens inside the form box or doesn't open at all. The landing page still has the listener I added earlier, so the safest option is to send the signal and also try the redirect. Paste this into the Thank You Code:

```
<script>window.parent.postMessage({ jaxEventForm: 'registered' }, 'https://www.jaxconsult.com'); try { window.top.location.href = "https://www.jaxconsult.com/nyc-education-ai-2026-registered/"; } catch (e) {}</script>
```

Whichever part works first, the person lands on the same page. At 30 registrations, change **both** `registered` words to `waitlist`.

**2. The registration still hasn't reached Salesforce.** I just checked: the campaign has 0 members, and no lead was created today. The notification you got was most likely Pardot's own "form submitted" email, not a sign that the record synced. Until the form assigns the prospect to a user or queue (put that completion action before "Add to Salesforce Campaig

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
