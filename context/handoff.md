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
**Status:** on track — Form redirect logic built and saved to draft landing page. Ready to publish thank-you pages and test end-to-end.

**Done this session**
- Added missing signal listener to draft landing page to catch Pardot 'registered'/'waitlist' signal and redirect to thank-you pages
- Verified page saved with featured image still set

**Open items**
- Publish both thank-you pages (/nyc-education-ai-2026-registered/ and /nyc-education-ai-2026-waitlist/)
- Test form submission on draft landing page preview with ?utm_source=test&utm_campaign=test; verify registered thank-you page opens in full window
- Preview both thank-you pages on computer and phone; report any changes needed
- Set Yoast 'Allow search engines' to No on both thank-you pages
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
- Publish both thank-you pages
- Test form submission on draft landing page preview with ?utm_source=test&utm_campaign=test; confirm registered thank-you page opens in full window
- Preview both thank-you pages on computer and phone; report desired changes
- Set Yoast 'Allow search engines' to No on both published pages

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
Leave the Pardot code as it is. You don't need to change anything there.

That code only sends a "form submitted" signal to the landing page. The page didn't have anything to catch that signal yet, so after submitting, people would have stayed on the form's thank-you message. I've now added the missing piece to the draft landing page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). The page saved, it's still a draft, and the featured image is still set.

**What happens now when someone submits the form:**
- Pardot sends the signal `registered`, and the whole browser window opens `/nyc-education-ai-2026-registered/`.
- At 30 registrations, change the word `registered` to `waitlist` in the Pardot Thank You Code. People will then go to `/nyc-education-ai-2026-waitlist/` instead.
- The page only accepts this signal from your Pardot site (go.jaxconsult.com), so other sites can't trigger the redirect.

**Before you test:**
1. **Publish both thank-you pages.** Right now they're drafts, so visitors would see "page not found".
2. **Test on the preview link.** Open the draft landing page preview with `?utm_source=test&utm_campaign=test` added to the end, then submit the 

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
