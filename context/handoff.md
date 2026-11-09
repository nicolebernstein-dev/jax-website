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
**Status:** on track — Live page updated: form repositioned, 3 headings set to 28px. Awaiting browser verification and test registration.

**Done this session**
- Repositioned form to align with left text on desktop screens
- Set 'What you will leave with', 'What is Orchestrate?', and 'Who should attend' headings to 28px

**Open items**
- Test live page in browser on computer and phone to verify form position and heading sizes
- Submit one test registration and confirm redirect to thank-you page works
- Confirm Pardot email greeting matches 'Hi,' or report actual wording
- Remove 2 test leads from Salesforce campaign
- Post Slack announcement with updated email PDFs
- Notify Karen that page is ready for outreach

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- 'What you will leave with', 'What is Orchestrate?', and 'Who should attend' headings set to 28px on live page

**Blockers**
- None

**Next**
- Open live page on computer and phone; verify form alignment and 28px heading appearance
- Report any form position or heading size adjustments needed (e.g., 'form a bit lower')
- Submit test registration; confirm thank-you page redirect works
- Notify Karen page is ready for outreach

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
I've updated the live page: [jaxconsult.com/nyc-education-ai-2026](https://www.jaxconsult.com/nyc-education-ai-2026/). WordPress shows it's still published with both changes in it. It was saved as a new revision, and the earlier version is still in the page history.

**What changed:**
1. **The form sits lower.** It now starts at the same height as the text on the left, instead of one line above it. This only applies on computer-width screens. On phones the form stays below the text, as before.
2. **The three headings are 28px:** "What you will leave with", "What is Orchestrate?" and "Who should attend". Before, the first was 22px and the other two used the theme's larger default size.

Nothing else changed. The text, the form, the scripts, the video and the rest of the styling are all as they were.

I haven't viewed the public page in a browser, so please look at it on your computer. If the form needs to go lower or higher, give me a rough amount, like "a bit more" or "half a line less", and I'll adjust it. On your earlier list, the test registration and letting Karen know the page is ready are still open.

Sources: checked live: WordPress page 3065, read before saving and checked 

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
