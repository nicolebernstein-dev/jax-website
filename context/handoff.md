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
**Status:** on track — Draft refined: date/time centered, heading sized to 22px. Awaiting approval to merge to live.

**Done this session**
- Centered date, time, location in hero left column
- Resized 'What you will leave with' heading to 22px

**Open items**
- Approve or request changes to draft copy and layout (heading size, date centering scope)
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
- Review draft preview and approve or request changes to heading size or date centering scope
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
I made both changes on the draft only. The live page hasn't been touched.

**Preview:** [the draft preview](https://www.jaxconsult.com/?page_id=3092&preview=true) (sign in to WordPress first, then refresh).

1. **Date, time and location are centered.** "Wednesday, December 2, 2026 / 1:30–4:30 PM ET / Salesforce Tower" now sits in the middle of the left column of the hero, not across the full page width. Everything else in that column is still left-aligned.
2. **"What you will leave with" is smaller.** I set it to 22px, close to the size of the body text, so it reads as a sub-heading. It's still white and uses the same font. The two headings further down ("What is Orchestrate?" and "Who should attend") are unchanged.

The response from the save shows both changes in the content and the page is still a draft. Nothing else changed: the text, the form, the scripts, the video and the layout are all as before.

If you'd like the heading a little bigger or smaller, tell me a size (for example 20px or 26px). If the date block should be centered across the whole hero rather than just its column, I can do that too. Once you're happy with it, I'll copy the content to the live page, and you'll

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
