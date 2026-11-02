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
**Status:** on track — Thank-you pages drafted & featured image set; preview & Pardot config next

**Done this session**
- Created /nyc-education-ai-2026-registered/ thank-you page (draft)
- Created /nyc-education-ai-2026-waitlist/ thank-you page (draft)
- Featured image now set on landing page

**Open items**
- Preview both thank-you pages on computer and phone; report any changes needed
- Set Yoast 'Allow search engines' to No on both thank-you pages
- Publish both thank-you pages before test submission
- Add Thank You Code to Pardot form (registered page URL initially, switch to waitlist at 30 registrations)
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed
- Test form submission with ?utm_source=test&utm_campaign=test; verify UTMs, prospect record, confirmation email, thank-you page routing
- Reload page editor, set featured image, save draft to persist it

**Decisions**
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Thank-you page URLs: /nyc-education-ai-2026-registered/ and /nyc-education-ai-2026-waitlist/ (not /thank-you/ to avoid conflict)
- Cutover at 30 registrations: single Step 6 edit session in Pardot to change Thank You Code URL
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links, merge tags {{Recipient.FirstName}} and {{Unsubscribe}}

**Blockers**
- Google Workspace connection expired — cannot verify event address in Google Doc

**Next**
- Preview both thank-you pages on computer and phone; report desired changes
- Set Yoast 'Allow search engines to show this page' to No on both pages
- Publish both thank-you pages
- Add Thank You Code to Pardot form with registered page URL
- Enable reCAPTCHA and test form submission end-to-end

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
I've created both thank-you pages as drafts in WordPress. Both saved and neither is published.

- **Registered:** [You're Registered: From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3083)
- **Waitlist:** [You're on the Waitlist: From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3084)

**The address is different from what we planned.** The site already has a live page at `/thank-you/` (the general "Thank you for contacting us" page). So I gave these their own addresses so that page isn't affected:
- `jaxconsult.com/nyc-education-ai-2026-registered/`
- `jaxconsult.com/nyc-education-ai-2026-waitlist/`

**What they look like:** both use the same white top menu and Washington Square Arch photo as the landing page. The text sits in a dark navy box in the middle, with the photo credit in the corner.

**Registered page**
- Small heading: You're registered
- Main heading: **Your seat is reserved. See you on December 2.**
- It says their confirmation email is on its way, then lists the date, time and Salesforce Tower.
- It tells them to check spam if the email doesn't arrive, and gives sales@jaxconsult.com.
- Buttons: an orange **Add to Google Calendar** button (1:30–

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
