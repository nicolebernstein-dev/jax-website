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
**Status:** on track — Live page updated with hero restructure and 22px heading. Awaiting browser test and registration confirmation.

**Done this session**
- Merged draft content to live page: hero line, date/time/location, 'What you will leave with' section with 22px heading
- Updated 'NYU' to 'NYU Stern' in blue box
- Moved 'Spaces are limited' text below Reserve button
- Preserved all other page elements and scripts

**Open items**
- Test live page in browser on computer and phone to verify hero layout and responsiveness
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
- 'What you will leave with' heading set to 22px on live page

**Blockers**
- None

**Next**
- Open live page on computer and phone; verify hero layout and 22px heading appearance
- Submit test registration; confirm thank-you page redirect works
- Report any layout or styling issues or confirm page is ready for outreach

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
The live page is updated: [jaxconsult.com/nyc-education-ai-2026](https://www.jaxconsult.com/nyc-education-ai-2026/). WordPress returned the saved page, still published, with the new content in it. It's saved as a new revision, and the earlier version is still in the page history if you want to go back to it.

**What changed on the live page:**
1. **Hero line:** "The NYU Stern team joins in person to share how they are using Orchestrate to accelerate their Salesforce work."
2. **Date, time and location** stay left-aligned, as they were before.
3. **"What you will leave with"** (the heading and 6 bullets, in white) now sits in the hero, under the date, time and location.
4. **Blue box:** same text in the same place, with "NYU" changed to "NYU Stern" twice.
5. **"Spaces are limited."** has moved down to just under the Reserve my seat button.

**One thing I added:** the "What you will leave with" heading uses the smaller 22px size you approved on the draft. I set it on that heading only and didn't touch the page's shared styling. Tell me if you'd rather have it back at the full heading size.

**Not changed:** the title, the page styling, the Pardot form, the UTM and redirect scripts, t

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
