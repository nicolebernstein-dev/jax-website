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
**Status:** on track — Registration live, Salesforce sync confirmed. Remove 2 test leads from campaign, then post announcement.

**Done this session**
- Drafted Slack announcement with landing page, campaign, and thank-you page links
- Generated Registration Confirmation and Waitlist Confirmation email PDFs
- Verified landing page is published and Salesforce campaign exists with 2 test leads
- Documented 30-registration threshold workflow and UTM tracking instructions

**Open items**
- Remove 2 test leads from Salesforce campaign before posting announcement
- Post Slack announcement with attached email PDFs to team channel
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-registered/
- Set Yoast 'Allow search engines' to No on /nyc-education-ai-2026-waitlist/
- Preview both thank-you pages on computer and phone; report desired changes
- Monitor registrations and update Pardot form completion actions when 30 registrations reached

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Form name: 'event-26-12-ny-world-tour-edu – Registration Form'
- Confirmation emails use Jax layout, Montserrat/Nunito fonts, blue #0c83df links

**Blockers**
- None

**Next**
- Remove 2 test leads from campaign in Salesforce
- Post Slack announcement with email PDFs to team channel
- Set Yoast SEO settings on both thank-you pages
- Preview thank-you pages and report any desired changes

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
I've drafted the Slack message below. The two confirmation emails are attached to this session as PDFs. Pardot email links only open for people with Pardot access, so post the PDFs with the message.

---

:tada: **The NYC World Tour education event registration is live**

*From Roadmap to Reality: Governed AI That Elevates the Student Experience*
Wednesday, December 2, 2026 · 1:30–4:30 PM ET · Salesforce Tower

**Links**
• *Landing page:* https://www.jaxconsult.com/nyc-education-ai-2026/
• *Salesforce campaign:* <https://jaxconsultingllc.lightning.force.com/lightning/r/Campaign/701UJ00001boDNdYAM/view|event-26-12-ny-world-tour-edu>
• *Registration thank-you page:* https://www.jaxconsult.com/nyc-education-ai-2026-registered/
• *Registration confirmation email:* attached (Registration Confirmation Email Preview PDF)

**How it works**
Registrants fill out the Pardot form on the landing page. Pardot then creates the lead in Salesforce, adds them to the campaign as *Registered*, sends the confirmation email and takes them to the thank-you page.

:warning: **After 30 registrations, we switch to the waitlist**
When we reach 30, we'll update the form in Pardot. From then on, new registrant

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
