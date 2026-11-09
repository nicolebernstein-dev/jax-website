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
**Status:** on track — Live page updated: form repositioned again, heading & button spacing refined. Browser verification & test registration still pending.

**Done this session**
- Doubled space above form on desktop (moved down ~1 line)
- Set 'Spaces are limited.' to 14px
- Added line space between Reserve button and note

**Open items**
- Test live page in browser on computer and phone to verify form position, heading sizes, and spacing
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
- 'What you will leave with', 'What is Orchestrate?', and 'Who should attend' headings set to 28px
- 'Spaces are limited.' set to 14px; line space added between Reserve button and note

**Blockers**
- None

**Next**
- Open live page on computer and phone; verify form alignment, 28px headings, and new spacing look correct
- Report any further form position adjustments needed (e.g., 'a bit higher')
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
I've updated the live page: [jaxconsult.com/nyc-education-ai-2026](https://www.jaxconsult.com/nyc-education-ai-2026/). The save result shows it's still published, saved at 11:21 as a new revision, with all three changes in it. The earlier version is still in the page history.

**What changed:**
1. **The form sits lower on computer screens.** I doubled the space above it, so it moves down about one more line. On phones it stays below the text, as before.
2. **"Spaces are limited." is smaller.** It's now 14px.
3. **There's a line of space between the Reserve my seat button and the note.**

**Your WordPress edits are still there:** the hero line says "Revecast Orchestrate", and your new first bullet ("...for everything from data migration to delivery") is unchanged. I checked that the page hadn't been edited again since I last read it before saving.

Nothing else changed. The text, form, scripts, video and other styling are all as they were.

I haven't seen the page in a browser. If the form still needs to go up or down, just tell me roughly how much. The test registration and letting Karen know the page is ready are still open.

Sources: checked live: WordPress page 3065, read before

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
