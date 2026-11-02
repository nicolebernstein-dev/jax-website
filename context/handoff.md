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
**Status:** on track — Confirmation emails built and ready to paste into Pardot. Landing page draft, form build, and address verification next.

**Done this session**
- Built D02 – Confirmation Email (Registered) as HTML ready for Pardot
- Built D03 – Confirmation Email (Waitlisted) as HTML ready for Pardot
- Verified logo images load and HTML structure is valid

**Open items**
- Reconnect Google Workspace (Connector Catalog → My Connections → Disconnect/Connect) to verify event address
- Preview landing page on mobile and desktop; confirm header, photo spacing, button style, text readability
- Decide: remove 'first-hand' from blue section or keep it
- Build Pardot form 'event-26-12-ny-world-tour-edu – Registration Form' with five hidden UTM fields
- Provide iframe link for completed Pardot form
- Test form submission twice with same address to verify status change at 30-registration threshold
- Send test emails from Pardot to verify rendering on desktop and mobile
- Publish landing page so event link in emails works live

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
- Reconnect Google Workspace to confirm Salesforce Tower address is correct
- Build Pardot form with five hidden UTM fields
- Send test emails from Pardot and preview on desktop and mobile
- Publish landing page to activate event link in confirmation emails
- Preview landing page and confirm 'first-hand' text decision

**Checked live on 2026-11-02:** Google Workspace
### Last session — 2026-11-02
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | NY World Tour Event Registration Page |
| Session | `e68d87da-5721-417e-adfc-c7124417d40e` |
**In its own words (excerpt):**
I've written both confirmation emails as complete HTML files you can paste straight into Pardot. They're attached to this session:

- **D02 – Confirmation Email (Registered)**
- **D03 – Confirmation Email (Waitlisted)**

**To copy the code:** open each file in a plain text editor (TextEdit with *Format → Make Plain Text*, Notepad or VS Code), select all and copy. In Pardot, open the email template, switch to the HTML or code view, paste and save. Double-clicking the file opens it in your browser instead, which is a good way to preview it.

**What I kept from your Jax email**
- The same layout: Jax + Revecast logo at the top, navy-bordered content box, Montserrat heading, Nunito body text, blue `#0c83df` links, the navy band, the footer logo, and the jaxconsult.com · revecast.io · Unsubscribe links, ending with the navy strip.
- The same merge tags: `{{Recipient.FirstName}}` and `{{Unsubscribe}}`.
- I took out the empty placeholder blocks and CSS rules that didn't change how the email looks, so the code is shorter.

**What each email says**

| | Registered | Waitlisted |
|---|---|---|
| Heading | You're registered! | You're on the waitlist |
| Preview text | Your seat is confirmed f

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
