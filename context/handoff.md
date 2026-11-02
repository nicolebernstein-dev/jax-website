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
**Status:** on track — Form repositioned with title in own row; NYU line finalized. Preview needed on computer & phone; reCAPTCHA, testing, thank-you pages remain.

**Done this session**
- Removed 'Reserve my seat' heading above form
- Repositioned form: eyebrow and title in full-width row; details left, form right on desktop; stacked on mobile
- Form top now aligns with NYU line, title sits above

**Open items**
- Preview landing page on computer and phone; confirm title wrapping, form fit, button visibility, spacing
- Reconnect Google Workspace to verify Salesforce Tower event address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height (~90px additional)
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
I've made both changes to the draft landing page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). The saved page includes them, and it's still a draft.

- **"Reserve my seat" heading:** removed from above the form. The orange "Reserve my seat" button at the bottom of the page is still there and still jumps up to the form.
- **Form position:** the eyebrow ("In Person · New York City") and the event title now sit in their own full-width row at the top of the header. Below that, the NYU line, date, time, location and "Hosted by" note are on the left, and the form is on the right. The top of the form now lines up with the NYU line, so the title is above it. On phones the order is title, details, then form.

**Please check the preview on a computer.** The title now spans most of the width, so it may wrap onto two lines instead of three or four. If it looks too wide, I can narrow it, or move the form a bit further down.

Sources: checked live: the draft page (read before saving, and the saved version WordPress returned) · not checked: how the page looks in a browser
<!-- orchestrate:session-state:end -->
