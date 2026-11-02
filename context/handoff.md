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
**Status:** on track — Thank-you pages published and live. Landing page draft ready for form testing after search engine blocking.

**Done this session**
- Published /nyc-education-ai-2026-registered/ thank-you page
- Published /nyc-education-ai-2026-waitlist/ thank-you page
- Verified both pages load for visitors

**Open items**
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Test form submission on draft landing page preview with ?utm_source=test&utm_campaign=test; verify registered thank-you page opens in full window
- Preview both thank-you pages on computer and phone; report any changes needed
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
- Google Workspace connection expired — cannot verify event address in Google Doc

**Next**
- Set Yoast 'Allow search engines' to No on both published thank-you pages
- Test form submission on draft landing page preview with ?utm_source=test&utm_campaign=test; confirm registered thank-you page opens in full window
- Preview both thank-you pages on computer and phone; report desired changes

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
I published both thank-you pages, and both load for visitors.

- [You're Registered: From Roadmap to Reality](https://www.jaxconsult.com/nyc-education-ai-2026-registered/)
- [You're on the Waitlist: From Roadmap to Reality](https://www.jaxconsult.com/nyc-education-ai-2026-waitlist/)

The landing page itself is still a draft.

**Do this next: hide them from Google.** Search engines are still allowed to show both pages. On each page, open the Yoast panel, go to **Advanced**, and set "Allow search engines to show this page in search results?" to **No**. Then click **Update**. I can't change that setting from here.

**Then test the form:**
1. Open the draft landing page preview and add `?utm_source=test&utm_campaign=test` to the end of the address.
2. Submit the form.
3. The registered thank-you page should open in the full browser window, not inside the form box. If it doesn't, tell me what you see.

Sources: checked live: both pages as WordPress saved them (status "publish"), and both web addresses (each loaded normally) · not checked: a real form submission in a browser
<!-- orchestrate:session-state:end -->
