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
**Status:** on track — Featured & video thumbnails ready to upload; preview & reCAPTCHA setup next

**Done this session**
- Created video thumbnail (1280×720) from 0:59 screenshot with 16:9 fit

**Open items**
- Upload featured image (nyc-event-featured-image-1200x630.jpg) to WordPress Media Library and set on page
- Upload video thumbnail (nyc-event-video-thumbnail-1280x720.jpg) to Media Library; send File URL and confirm play button position (centered or lower)
- Preview landing page on computer and phone; confirm title wrapping, form fit, button visibility, spacing, video load behavior
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
- Upload featured image to WordPress Media Library and set on page (1 min)
- Upload video thumbnail to Media Library; send File URL and specify play button position
- Preview draft landing page on computer and phone; report title wrapping, form fit, button visibility, spacing, video load behavior
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
I've attached two images to this session, both ready to upload to the WordPress Media Library:

- **nyc-event-featured-image-1200x630.jpg** is the featured image. It's the Washington Square Arch photo from the header, sized for link previews on LinkedIn, Slack and email.
  - Alt text: Washington Square Arch, New York City
  - Caption: Photo: BruceSchaff, CC BY-SA 4.0 (the photo's license requires this credit)
- **nyc-event-video-thumbnail-1280x720.jpg** is the video thumbnail, made from your 0:59 screenshot. I trimmed 4px off each side so it fits the 16:9 player exactly and enlarged it to 1280×720.
  - Alt text: Jax Consulting video: Build a production deployed Agentforce agent

**What to do next**
1. In the page editor, set the first image as the **Featured image** (right sidebar, Page tab).
2. Upload the thumbnail to the Media Library and send me its **File URL**. You'll find it in the image's details panel. I'll put it on the video.

I can't upload to the Media Library from here, so this has to be done on your end.

**About the play button:** the orange play button sits in the middle of the video, and on this frame that's right over the "Build a production deployed Agentforce ag

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
