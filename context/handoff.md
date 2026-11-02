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
**Status:** on track — Landing page draft finalized; Pardot form guide updated to single-form process. Ready for form build and email templates.

**Done this session**
- Updated Pardot Registration Forms Guide to single-form process (Form B removed)
- Added Step 6 switch table for 30-registration cutover edits
- Added Step 5 test to verify Pardot status change on duplicate submission

**Open items**
- Preview landing page on mobile and desktop; confirm header, photo spacing, button style, text readability
- Decide: remove 'first-hand' from blue section or keep it
- Build Pardot form 'event-26-12-ny-world-tour-edu – Registration Form' with five hidden UTM fields
- Create confirmation email template for Registered members
- Create confirmation email template for Waitlisted members
- Provide iframe link for completed Pardot form
- Test form submission twice with same address to verify status change at 30-registration threshold

**Decisions**
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Hidden UTM fields use existing Jax form field names and labels
- Page script routes to correct thank-you page (/thank-you/ or /waitlist/) based on registration count
- Cutover at 30 registrations: single Step 6 edit session in Pardot (campaign status, email, tag, thank-you code/message, button text)

**Blockers**
- None

**Next**
- Build Pardot form with five hidden UTM fields using existing Jax field names
- Create both confirmation email templates (Registered and Waitlisted)
- Send iframe link for completed form
- Preview landing page on desktop and mobile to verify spacing and readability
- Confirm decision on 'first-hand' text in blue section

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
I've updated the guide to the one-form process. The new version, **D01 – Pardot Registration Forms Guide**, is attached to this session and replaces the earlier one.

**What changed**
- **One form:** Form B and its copy step are gone. I named the form `event-26-12-ny-world-tour-edu – Registration Form`, without "Registered" in the name, because the same form will handle the waitlist too.
- **Step 1 is shorter:** you don't need to check or create the UTM fields. The hidden fields use the field names and labels from your existing Jax forms, and the guide mentions you can copy one of those forms to save time.
- **New Step 6, the switch at 30:** a table of every edit to make in Pardot in one sitting (campaign status, email, tag, thank-you code, thank-you message, button text), then a test entry to check it worked.
- **New test in Step 5:** before the event fills up, submit twice with the same test address to see whether Pardot changes an existing Registered member to Waitlisted.
- **Page script:** it opens the right thank-you page for both stages from the start, so nothing on the page has to change for the form to keep working after the switch.
- **Below Form text:** removed, since the

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
