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
**Status:** on track — Confirmation emails ready for Pardot. Form build in progress; reCAPTCHA guidance provided.

**Done this session**
- Provided reCAPTCHA setup instructions for Pardot form

**Open items**
- Reconnect Google Workspace to verify Salesforce Tower event address
- Build Pardot form 'event-26-12-ny-world-tour-edu – Registration Form' with five hidden UTM fields and reCAPTCHA enabled
- Provide iframe link for completed Pardot form
- Test form submission twice with same address to verify status change at 30-registration threshold
- Send test emails from Pardot and preview rendering on desktop and mobile
- Publish landing page to activate event link in confirmation emails
- Preview landing page on mobile and desktop; confirm header, photo spacing, button style, text readability
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
- Copy both email HTMLs into Pardot email templates
- Build Pardot form with five hidden UTM fields and enable reCAPTCHA in Advanced tab
- Test form submission with reCAPTCHA and verify thank-you page routing
- Send test emails from Pardot and preview on desktop and mobile
- Publish landing page to activate event link in confirmation emails

**Checked live on 2026-11-02:** the web
### Last session — 2026-11-02
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | NY World Tour Event Registration Page |
| Session | `e68d87da-5721-417e-adfc-c7124417d40e` |
**In its own words (excerpt):**
Keeping "Maintain the initial value" unticked to match your other forms is the right call.

## Turning on reCAPTCHA

1. Open the form in Account Engagement and click **Edit**.
2. Go to the **Look and Feel** step of the form wizard.
3. Open the **Advanced** tab.
4. Tick the reCAPTCHA / bot protection option ("Enable explicit bot protection").
5. Click through to **Confirm & Save**.

## Things to know

- **Pardot already has some protection without it.** Pardot shows a reCAPTCHA by itself when it detects an unusual burst of submissions. Turning it on makes every visitor see it.
- **It works in the page embed.** reCAPTCHA works on Pardot-hosted forms, and the landing page loads your hosted form in an iframe, so it's covered. (Form handlers aren't covered, but we're not using one.)
- **The form gets taller.** The checkbox adds height. When you send me the iframe link, tell me reCAPTCHA is on and I'll leave room in the embed so the submit button isn't cut off.
- **Test it once.** It's worth checking that the reCAPTCHA still lets the submission through and that the right thank-you page still opens. You'd do that in the same test submission that checks the UTMs.

I haven't seen your Pardo

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
