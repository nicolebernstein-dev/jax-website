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
**Status:** on track — Form embedded with responsive sizing; NYU line finalized; reCAPTCHA and testing remain

**Done this session**
- Updated NYU header line to final wording: 'The NYU team joins in person to share how they are putting AI to work.'
- Adjusted form box height to 500px desktop / 650px mobile for responsive fit
- Reduced gap under form from 12px to 4px

**Open items**
- Reconnect Google Workspace to verify Salesforce Tower event address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height when enabled (~90px additional)
- Test form submission with ?utm_source=test&utm_campaign=test; verify UTMs, prospect record, confirmation email, thank-you page routing
- Create /thank-you/ and /waitlist/ pages with wording (draft or provide copy)
- Preview landing page on computer and phone; confirm form fit, button visibility, header, photo spacing, text readability
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
- Preview draft landing page on computer and phone; report any form fit or button visibility issues
- Reconnect Google Workspace to confirm Salesforce Tower address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed
- Test form submission with UTM params; verify prospect record, campaign status, confirmation email, thank-you page routing
- Provide wording for /thank-you/ and /waitlist/ pages or request draft

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
I updated the NYU line and tightened the gap under the form on the draft page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). The saved version has both changes and is still a draft.

- **NYU line:** it now reads exactly as you wrote it: **"The NYU team joins in person to share how they are putting AI to work."**
- **Gap under the form:** the gap was empty space inside the form box. I'd made the box 620px tall, but the form only fills about 470px on a computer. I've set the box to 500px on computers. On phones it's 650px, because the fields stack there and the form gets taller. I also cut the space between the box and "*Spaces are limited." from 12px to 4px.

**Please check the preview on a computer and a phone.** I couldn't load the page in a browser here, so the 500px is based on the form's own styling, not a measurement. If the submit button gets cut off, or there's still a gap, tell me which device and I'll adjust it.

**When you turn on reCAPTCHA,** let me know. The checkbox adds roughly 90px, so I'll need to make the form box taller on both computers and phones, or the submit button will be cut off.

Sources: checked live: the draft page (read before sav

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
