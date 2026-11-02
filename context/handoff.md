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
**Status:** on track — Form repositioned & hero shortened; preview on computer & phone needed before reCAPTCHA, testing, thank-you pages

**Done this session**
- Moved 'Spaces are limited' note under 'Hosted by' line with blank line separator
- Reduced hero height: 40px below (was 100px), 80px above (was 100px) on desktop
- Overrode theme padding on mobile/tablet: 56px above, 36px below hero
- Verified changes saved in WordPress draft

**Open items**
- Preview landing page on computer and phone; confirm title wrapping, form fit, button visibility, spacing
- Reconnect Google Workspace to verify Salesforce Tower event address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed
- Test form submission with ?utm_source=test&utm_campaign=test; verify UTMs, prospect record, confirmation email, thank-you page routing
- Create /thank-you/ and /waitlist/ pages with wording (draft or provide copy)
- Send test emails from Pardot; preview rendering on desktop and mobile
- Publish landing page to activate event link in confirmation emails
- Decide: remove 'first-hand' from blue section or keep it

**Decisions**
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Hidden UTM fields use existing Jax form field names and labels
- Page script routes to correct thank-you page based on registration count
- Cutover at 30 registrations: single Step 6 edit session in Pardot
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links, merge tags {{Recipient.FirstName}} and {{Unsubscribe}}

**Blockers**
- Google Workspace connection expired — cannot verify event address in Google Doc

**Next**
- Preview draft landing page on computer and phone; report title wrapping, form fit, button visibility, spacing issues
- Reconnect Google Workspace to confirm Salesforce Tower address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed
- Test form submission with UTM params; verify prospect record, campaign status, confirmation email, thank-you page routing

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
I've moved the note and shortened the hero on the draft landing page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). I checked the version WordPress saved: both changes are in it, and the page is still a draft.

- **"*Spaces are limited.":** it now sits under "Hosted by Jax Consulting in partnership with Salesforce.", with a blank line between them. It's no longer under the form.
- **Hero height:** on computers, the space below the hero content is now 40px instead of 100px, and the space above it is 80px instead of 100px. On tablets and phones, the site's theme was forcing 83px above and below and ignoring the page's own setting. I overrode that on this page only, so it's now 56px above and 36px below. The photo credit still sits in the bottom-right corner.

**Please check the preview on a computer and a phone.** I can't see the page as it displays from here. On computers, the form is now the tallest thing in the hero, so most of what's left at the bottom is the form box itself. If there's still too much space, tell me and I'll trim the form box too. I'd do that in small steps so the submit button doesn't get cut off.

Sources: checked live: the draft page (re

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
