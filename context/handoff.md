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
**Status:** on track — Pardot forms guide complete; awaiting iframe links, UTM Field IDs, and email copy to proceed

**Done this session**
- Created D01 – Pardot Registration Forms Guide covering both forms, UTM capture, confirmation emails, thank-you pages, and go-live checklist
- Verified UTM Lead fields exist and 381 leads have UTM data
- Identified UTM script requirement for iframe form and thank-you page redirect

**Open items**
- Build Pardot Form A (Registered action) with five hidden UTM fields
- Build Pardot Form B (Waitlisted action) as copy of Form A
- Create two confirmation email templates (registered and waitlist)
- Provide iframe links for Form A and Form B
- Provide five UTM Field IDs from Pardot prospect field settings
- Provide confirmation email text and thank-you page wording
- Add UTM script and forms to WordPress page and create thank-you page drafts
- Consider adding five UTM fields to Contact object (optional)

**Decisions**
- Campaign type: Seminar/Conference
- Campaign status: Planned and Active
- Event date: December 2, 2026
- Member statuses: Registered (default), Waitlisted, Attended, No Show
- Use Registered count for seat availability, not Responded total
- UTM capture via script on landing page (iframe limitation)
- Thank-you pages at /nyc-education-ai-2026/thank-you/ and /nyc-education-ai-2026/waitlist/

**Blockers**
- None

**Next**
- Build Pardot Form A and Form B with UTM hidden fields and campaign member actions
- Create two confirmation email templates for autoresponder use
- Send iframe links, UTM Field IDs, and email/thank-you wording
- Add UTM script and forms to WordPress page; create thank-you page drafts
- Test forms and UTM capture before publishing

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
I've attached a step-by-step guide to this session: **D01 – Pardot Registration Forms Guide**. It covers building both forms, with UTM capture, the confirmation emails and the thank-you pages. In short:

1. **UTM fields:** check (or create) five hidden prospect fields and map them to your Salesforce Lead fields `UTM_Source__c` through `UTM_Term__c`. Those Lead fields already exist, and 381 leads have UTM data in them.
2. **Confirmation emails:** create two email templates marked as available for autoresponders, one saying "You're registered" and one saying "You're on the waitlist". There are prompts for where your content goes.
3. **Form A:** First name, Last name, Email, Company and Title, plus the five hidden UTM fields. On submit it adds the person to the campaign as **Registered** and sends the registration email.
4. **Form B:** a copy of Form A that sets **Waitlisted** and sends the waitlist email.
5. **Thank-you pages:** `/nyc-education-ai-2026/thank-you/` and `/nyc-education-ai-2026/waitlist/`.
6. **Before you go live:** a test checklist, how to switch to Form B at 30 seats (including changing Form A to waitlist so nobody can still register through it) and how to move people

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
