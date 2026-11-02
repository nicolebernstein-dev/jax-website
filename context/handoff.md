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
**Status:** on track — Confirmation emails completed and ready to paste into Pardot. Landing page, form build, and address verification next.

**Done this session**
- Finalized D02 – Confirmation Email (Registered) HTML with &ndash; dash fix
- Finalized D03 – Confirmation Email (Waitlisted) HTML with &ndash; dash fix
- Provided copy-ready HTML blocks for both emails

**Open items**
- Reconnect Google Workspace to verify Salesforce Tower event address
- Build Pardot form 'event-26-12-ny-world-tour-edu – Registration Form' with five hidden UTM fields
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
- Reconnect Google Workspace to confirm Salesforce Tower address is correct
- Copy both email HTMLs into Pardot email templates
- Build Pardot form with five hidden UTM fields
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
Here's the HTML for both emails. Each code block has a **Copy** button in its top-right corner. Click it, then in Pardot open the email template, switch to the HTML or code view, delete what's there, paste and save.

I made one small change from the files I attached earlier: the dash in "1:30–4:30" is now written as `&ndash;`, so it displays correctly in every email program.

## Email 1: Registered

```html
<!DOCTYPE html>
<html xmlns:v="urn:schemas-microsoft-com:vml" xmlns:o="urn:schemas-microsoft-com:office:office" lang="en-US">

<head>
	<title>You're registered: From Roadmap to Reality</title>
	<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0"><!--[if mso]>
<xml><w:WordDocument xmlns:w="urn:schemas-microsoft-com:office:word"><w:DontUseAdvancedTypographyReadingMail/></w:WordDocument>
<o:OfficeDocumentSettings><o:PixelsPerInch>96</o:PixelsPerInch><o:AllowPNG/></o:OfficeDocumentSettings></xml>
<![endif]--><!--[if !mso]><!-->
	<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900" rel="stylesheet" type="text/css">
	<link href="https://fonts.goog

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
