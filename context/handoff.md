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
**Status:** on track — Video added with default thumbnail; preview & 0:59 frame capture needed before reCAPTCHA & testing

**Done this session**
- Removed asterisk from 'Spaces are limited.'
- Added video in light-grey section at bottom with lazy-load YouTube player

**Open items**
- Preview landing page on computer and phone; confirm title wrapping, form fit, button visibility, spacing, video load behavior
- Capture 0:59 frame screenshot from video; upload to Media Library or provide for swap
- Set featured image (0:59 frame or alternative) to control social share preview
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
- Preview draft landing page on computer and phone; report title wrapping, form fit, button visibility, spacing, video load behavior
- Capture 0:59 frame screenshot and upload to Media Library or provide link
- Set featured image to control social share preview
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
I removed the asterisk and added the video, but the thumbnail isn't the 0:59 frame yet. The draft page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065), saved with both changes and is still a draft.

- **"Spaces are limited.":** the asterisk is gone.
- **Video:** it's in a new light-grey section at the very bottom, below the "Reserve my seat" button. It's the full width of the text above it, with an orange play button in the middle. The YouTube player only loads when someone clicks, and the video then starts from the beginning.

**Why the thumbnail isn't the 0:59 frame:** YouTube doesn't let you pick a thumbnail by timestamp. To use that frame, I'd have to download the video and take the still from it, and YouTube blocked the download from here ("Sign in to confirm you're not a bot"). So for now the page uses the video's default YouTube thumbnail.

**To get the 0:59 frame:**
1. Pause the video at 0:59 and take a screenshot, cropped to just the video.
2. Upload it to the WordPress Media Library and send me its link. Or attach it here, and you can upload it once I've cropped and sized it.
3. I'll swap it in. That's a one-line change.

**Something else to know:** t

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
