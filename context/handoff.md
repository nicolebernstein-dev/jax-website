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
### Engagement state — 2026-11-03
**Status:** on track — Button fixed, page styles & scripts restored. Ready for browser testing and Pardot confirmation.

**Done this session**
- Fixed 'Reserve my seat' button sizing on live page
- Restored page styles to one line — nav bar, hero spacing, form height, video layout now load
- Restored both scripts to one line — form redirect and video click should work
- Removed stray WordPress tags from HTML

**Open items**
- Confirm Pardot email greeting is 'Hi,' — if different wording, report so PDFs can be updated
- Remove 2 test leads from Salesforce campaign before posting announcement
- Post Slack announcement with updated email PDFs to team channel
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Test page in browser on computer and phone; do one test registration to confirm thank-you redirect
- Report any desired changes to page design or video play-button icon

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
- Test live page in browser on computer and phone — measure button, test form redirect, click video
- Do one test registration and confirm redirect to thank-you page works
- Confirm Pardot email greeting matches 'Hi,' or report actual wording
- Remove 2 test leads from Salesforce campaign
- Post Slack announcement with updated email PDFs

**Checked live on 2026-11-03:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-03
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | Event Landing Page Updates |
| Session | `b4cbb9e8-f3b5-4243-ad77-15da62c2f183` |
**In its own words (excerpt):**
I've updated the live page at [jaxconsult.com/nyc-education-ai-2026](https://www.jaxconsult.com/nyc-education-ai-2026/). The "Reserve my seat" button now uses the site's standard orange button sizing and should no longer stretch across the column.

**What changed:**
- **Button:** I set the sizing directly on the button itself, so WordPress can't break it again.
- **Page styles:** I put the style code on one line. The design it was built with now loads: the white nav bar, the hero spacing, the form height and the video thumbnail layout.
- **Scripts:** I put both scripts on one line too. Registrants should now be sent to the registered or waitlist thank-you page after they submit, and clicking the video should play it.
- **Clean-up:** I removed a few stray tags WordPress had added after the HTML comments. The page's text is unchanged.

**What I checked:** The live page's style and script code no longer has any of those stray line breaks, and both scripts are now valid code that will run. I couldn't open the page in a browser this run, so I haven't measured the button or watched the redirect and video click work. Please look at it on your computer and phone, and do one test registrati

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
