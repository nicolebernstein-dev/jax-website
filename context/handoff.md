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
**Status:** on track — Featured image file ready to upload; video stays on YouTube; preview & 0:59 frame capture still needed

**Done this session**
- Created featured image file (1200×630) from Washington Square Arch photo
- Confirmed video hosting strategy: keep YouTube (Revecast channel)

**Open items**
- Preview landing page on computer and phone; confirm title wrapping, form fit, button visibility, spacing, video load behavior
- Capture 0:59 frame screenshot from video; upload to Media Library or provide for swap
- Upload featured image file (nyc-event-featured-image-1200x630.jpg) to WordPress Media Library and set on page
- Reconnect Google Workspace to verify Salesforce Tower event address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed
- Test form submission with ?utm_source=test&utm_campaign=test; verify UTMs, prospect record, confirmation email, thank-you page routing
- Create /thank-you/ and /waitlist/ pages with wording (draft or provide copy)
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
- Upload featured image file to WordPress Media Library and set on page (1 min)
- Preview draft landing page on computer and phone; report title wrapping, form fit, button visibility, spacing, video load behavior
- Capture 0:59 frame screenshot and upload to Media Library or provide link
- Reconnect Google Workspace to confirm Salesforce Tower address
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed

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
I couldn't set the featured image myself, so I made a version sized for it that you can upload. My WordPress tools here can't upload to the Media Library or set a page's featured image. I checked the page: it still has no featured image. The header photo isn't in your Media Library either. The page loads it straight from Wikimedia Commons, so there's nothing in WordPress to pick yet.

## Featured image

**nyc-event-featured-image-1200x630.jpg** is attached to this session. It's the same Washington Square Arch photo as the header, cropped to 1200×630, the standard size for link previews on LinkedIn, Slack and email.

To set it (about a minute):
1. Open the page in WordPress and find **Featured image** in the right sidebar (Page tab).
2. Click **Set featured image**, then **Upload files**, and choose the attached image.
3. Fill in the image details:
   - **Alt text:** Washington Square Arch, New York City
   - **Caption:** Photo: BruceSchaff, CC BY-SA 4.0 (the photo's license requires credit)
4. Click **Set featured image**, then **Save draft**.

Once it's set, Yoast will use it for link previews instead of the YouTube thumbnail it uses now. Tell me when it's done and I'll check the 

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
