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
**Status:** on track — Email greetings updated to 'Hi,' — PDFs refreshed. Ready to post announcement and complete remaining setup tasks.

**Done this session**
- Updated Registration Confirmation Email PDF with 'Hi,' greeting
- Updated Waitlist Confirmation Email PDF with 'Hi,' greeting
- Verified both PDFs are one page with logos at top and bottom

**Open items**
- Remove 2 test leads from Salesforce campaign before posting announcement
- Post Slack announcement with updated email PDFs to team channel
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Preview both thank-you pages on computer and phone; report desired changes
- Confirm Pardot email greeting matches 'Hi,' or update PDFs if different wording used
- Monitor registrations and update Pardot form completion actions when 30 registrations reached

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links
- Email greeting: 'Hi,' (no first name)

**Blockers**
- None

**Next**
- Confirm Pardot email greeting is 'Hi,' — if different, report wording so PDFs can be updated
- Remove 2 test leads from campaign in Salesforce
- Post Slack announcement with updated email PDFs to team channel
- Set Yoast SEO settings on both thank-you pages
- Preview thank-you pages on computer and phone; report any desired changes

**Checked live on 2026-11-03:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-03
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | NY World Tour Event Registration Page |
| Session | `e68d87da-5721-417e-adfc-c7124417d40e` |
**In its own words (excerpt):**
I've updated both email PDFs. The greeting now reads "Hi," and no longer includes the first name. Both PDFs are attached to this session:

- **Registration Confirmation Email Preview**
- **Waitlist Confirmation Email Preview**

I opened both and checked them. Each is one page and has the logos at the top and bottom. Nothing else changed.

I couldn't see your Pardot version, so I assumed the greeting there is now "Hi,". If you used different wording, like "Hello," or no greeting at all, tell me and I'll update the PDFs to match.

The Slack message from before still works with these. Just attach the new PDFs.

Sources: checked live: nothing in Pardot (I can't access it) · not checked: the exact greeting in your Pardot emails
<!-- orchestrate:session-state:end -->
