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
**Status:** at risk — Page updates live & verified. Karen notification blocked by Slack access limits — needs manual send or member ID.

**Done this session**
- Attempted to notify Karen via Slack; drafted message ready to send
- Confirmed page changes are live and saved in WordPress

**Open items**
- Test live page in browser on computer and phone to verify form position, heading sizes, and spacing
- Submit one test registration and confirm redirect to thank-you page works
- Confirm Pardot email greeting matches 'Hi,' or report actual wording
- Remove 2 test leads from Salesforce campaign
- Post Slack announcement with updated email PDFs
- Send Karen notification — requires her Slack member ID, alternative channel, or manual copy-paste
- Provide corrected Salesforce campaign link if it should be included in Karen message

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes set to 28px; 'Spaces are limited.' set to 14px with line space after Reserve button

**Blockers**
- Slack token type does not allow message search or member lookup — cannot identify or contact Karen without external input

**Next**
- Provide Karen's Slack member ID, a channel name, or send the draft message yourself
- Test live page in browser on computer and phone; report any further form position adjustments needed
- Submit test registration and confirm thank-you page redirect works
- Confirm Pardot email greeting wording

**Checked live on 2026-11-09:** Slack
### Last session — 2026-11-09
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | Update NY Event Registration Page |
| Session | `5d3c0f45-ef5a-4fd1-895c-99a7b5b0cfd8` |
**In its own words (excerpt):**
I couldn't find Karen on Slack, so nothing has been sent yet. Here's the message, ready to go.

**What went wrong:**
- Slack search came back with `not_allowed_token_type`, so this connection can't search messages.
- I looked up 8 members of #oct-all-delivery-meeting by their IDs. Every lookup came back `user_not_found`, so I can't match a name to a person.
- I'm not a member of #jax_revecast-marketing, so I couldn't read who posts there.
- I've stopped trying, rather than guess who Karen is.

**Draft message to Karen:**

> Hi Karen, the NYC event page is updated and ready for outreach: https://www.jaxconsult.com/nyc-education-ai-2026/
>
> What changed, based on our call:
> • **New hero line:** "The NYU Stern team joins in person to share how they are using Revecast Orchestrate to accelerate their Salesforce work." The generic "putting AI to work" wording is gone.
> • **"What you will leave with" is now at the top**, in the hero under the date, time and location, so people see the takeaways without scrolling. The bullets now focus on practical results: how NYU Stern uses Orchestrate from data migration to delivery, a focused session on Agentforce for IT Services, a live AI-assisted

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
