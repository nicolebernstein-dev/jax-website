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
**Status:** on track — Video thumbnail live & working; featured image needs save; preview & reCAPTCHA next

**Done this session**
- Video thumbnail uploaded and linked; play button positioned below text, loads correctly at 944×526

**Open items**
- Reload page editor, set featured image, save draft to persist it (WordPress showing none currently)
- Preview landing page on computer and phone; confirm title wrapping, form fit, button visibility, spacing, video play behavior
- Upload featured image (nyc-event-featured-image-1200x630.jpg) to Media Library if not already done
- Enable reCAPTCHA in Pardot form Advanced tab; adjust form box height if needed
- Test form submission with ?utm_source=test&utm_campaign=test; verify UTMs, prospect record, confirmation email, thank-you page routing
- Create /thank-you/ and /waitlist/ pages with wording (draft or provide copy)
- Reconnect Google Workspace to verify Salesforce Tower event address
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
- Reload page editor, set featured image again, click Save draft, confirm save completed
- Preview draft page on computer and phone; test video play; report title wrapping, form fit, button visibility, spacing
- Enable reCAPTCHA in Pardot form Advanced tab and adjust form box height if needed

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
The video now uses your 0:59 thumbnail, but the featured image isn't showing as set yet. The draft page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065), saved and is still a draft.

**Video thumbnail:** done.
- The video box now uses your Video-thumbnail.png. I checked the link and the image loads.
- The orange play button sits about three-quarters of the way down, below the "Build a production deployed Agentforce agent" box, so it doesn't cover the text. On phones it's a bit smaller.
- WordPress was adding line breaks inside the video box, which could have pushed the image down and left a black strip at the top. I put that code on one line and hid any stray line breaks.
- Your image is 944×526, which is slightly wider than the player's 16:9 shape. About 4px gets trimmed off each side, which you won't notice.

**Featured image:** WordPress still shows no featured image saved on this page. Because of that, Yoast is now using the video thumbnail as the link preview image on LinkedIn, Slack and email, not the Washington Square Arch photo. Usually this means the image was chosen in the editor but the page wasn't saved afterwards.

**Before you save in the editor, r

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
