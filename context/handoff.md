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
**Status:** on track — Form embedded with UTM tracking live; reCAPTCHA ready to enable; thank-you pages and test submission pending

**Done this session**
- Added Pardot form to draft landing page in 'Reserve my seat' slot
- Rewrote NYU header line for clarity and impact
- Verified UTM tracking script copies query params to hidden form fields
- Confirmed form has all 5 hidden UTM fields plus required fields and spam trap

**Open items**
- Reconnect Google Workspace to verify Salesforce Tower event address
- Enable reCAPTCHA in Pardot form Advanced tab (form height already set to 620)
- Test form submission with ?utm_source=test&utm_campaign=test; verify UTMs, status, email, thank-you page
- Create /thank-you/ and /waitlist/ pages with wording (draft or provide copy)
- Preview landing page on mobile and desktop; confirm header, photo spacing, button style, text readability
- Send test emails from Pardot and preview rendering on desktop and mobile
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
- Reconnect Google Workspace to confirm Salesforce Tower address
- Enable reCAPTCHA in Pardot form Advanced tab
- Test form submission with UTM params; verify prospect record, campaign status, confirmation email, thank-you page routing
- Provide wording for /thank-you/ and /waitlist/ pages or request draft
- Preview landing page on mobile and desktop
- Send test emails from Pardot and preview on desktop and mobile
- Publish landing page to activate event link in confirmation emails

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
I've added your form to the draft landing page and rewritten the NYU line: [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). The saved page includes both changes and is still a draft.

**New NYU line in the header:**
> **Meet the NYU team in person and hear how they are putting AI to work.**

"Meet… in person" makes it clear they'll be there, and "putting AI to work" says what attendees will get from it. If you'd like something punchier, two other options are:
- "NYU will be in the room, sharing what it took to put AI to work."
- "Hear from NYU, live and in person, on what's working with AI."

**The form**
- **On the page:** it's in the "Reserve my seat" slot where the placeholder box used to be. I set the height to 620 instead of 500 so the submit button doesn't get cut off. That also leaves room for the reCAPTCHA checkbox, which isn't showing on the form yet. If you turn it on and the button still gets cut off, tell me and I'll make it taller.
- **UTM tracking works:** a small script copies any `utm_source`, `utm_medium`, `utm_campaign`, `utm_term` and `utm_content` values from the page link into the form. I tested the form itself: when I added `?utm_source=…` 

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
