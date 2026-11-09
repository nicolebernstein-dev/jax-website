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
### Engagement state — 2026-11-09
**Status:** on track — Draft copy created for review; live page unchanged. Awaiting approval to merge to production.

**Done this session**
- Created draft with updated hero line, 'What you will leave with' bullets in hero, and 'NYU Stern' branding
- Positioned 'Spaces are limited' under Reserve my seat button
- Confirmed draft is unpublished and preview-ready

**Open items**
- Approve or request changes to draft copy and layout (hero height, bullet placement, spacing)
- Merge approved draft content to live page and confirm styling applies
- Test live page in browser on computer and phone after merge
- Do one test registration and confirm redirect to thank-you page works
- Confirm Pardot email greeting matches 'Hi,' or report actual wording
- Remove 2 test leads from Salesforce campaign
- Post Slack announcement with updated email PDFs

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links
- Email greeting: 'Hi,' (no first name)
- Button sizing set directly on button element to prevent WordPress override

**Blockers**
- None

**Next**
- Review draft preview and approve or request changes to text and layout
- Once approved, merge draft content to live page and switch styling back to live
- Test live page in browser on computer and phone after merge

**Checked live on 2026-11-09:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-09
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | Update NY Event Registration Page |
| Session | `5d3c0f45-ef5a-4fd1-895c-99a7b5b0cfd8` |
**In its own words (excerpt):**
I've created the draft copy for you to review. It's unpublished, so only signed-in WordPress users can see it. The live page hasn't been touched.

**Preview:** sign in to WordPress, then open [the draft preview](https://www.jaxconsult.com/?page_id=3092&preview=true). In the Pages list it's titled "[DRAFT REVIEW] From Roadmap to Reality…".

**What's different from the live page:**
1. **Hero line:** "The NYU Stern team joins in person to share how they are using Orchestrate to accelerate their Salesforce work."
2. **"What you will leave with"** (heading and the 6 bullets) is now in the hero, under the date, time and Salesforce Tower, and above "Hosted by Jax Consulting…". I set it to white so it shows on the dark photo.
3. **Blue box:** same text in the same place. The only change is "NYU" → "NYU Stern" (twice).
4. **"Spaces are limited."** has moved from the hero to just under the Reserve my seat button.

Everything else is copied exactly: the form, the scripts, the video and the layout. I saved the draft and read it back to confirm the text and that it's still unpublished.

**Things to check in the preview:**
- The hero's left side is now longer than the form beside it, because the

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
