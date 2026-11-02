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
**Status:** on track — Landing page header photo added; awaiting forms, UTM IDs, and email copy to proceed

**Done this session**
- Added Washington Square Arch photo to landing page header with brand gradient overlay
- Verified photo license (CC0) and link functionality

**Open items**
- Build Pardot Form A (Registered action) with five hidden UTM fields
- Build Pardot Form B (Waitlisted action) as copy of Form A
- Create two confirmation email templates (registered and waitlist)
- Provide iframe links for Form A and Form B
- Provide five UTM Field IDs from Pardot prospect field settings
- Provide confirmation email text and thank-you page wording
- Upload Washington Square Arch photo to WordPress Media Library and send new link
- Add UTM script and forms to WordPress page; create thank-you page drafts

**Decisions**
- Campaign type: Seminar/Conference
- Campaign status: Planned and Active
- Event date: December 2, 2026
- Member statuses: Registered (default), Waitlisted, Attended, No Show
- Use Registered count for seat availability
- UTM capture via script on landing page (iframe limitation)
- Thank-you pages at /nyc-education-ai-2026/thank-you/ and /nyc-education-ai-2026/waitlist/
- Header photo sourced from Wikimedia Commons (CC0)

**Blockers**
- None

**Next**
- Upload Washington Square Arch photo to Media Library; send new link to switch header
- Test landing page header on mobile before publishing
- Build Pardot Form A and Form B with UTM hidden fields and campaign member actions
- Create two confirmation email templates for autoresponder use
- Send iframe links, UTM Field IDs, and email/thank-you wording
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
The draft landing page header now uses Marco Almbauer's photo of the Washington Square Arch. You can preview it at [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). The page is still a draft and hasn't been published.

**What changed**
- **Header background:** the arch photo now sits behind the hero. Your blue brand gradient is laid over it, partly see-through, so the white title, event details and form box stay easy to read. The photo is sized to fill the header on any screen.
- **Nothing else:** all the text, the form slot and the decorative pattern are the same as before.
- **Checked:** I read the page back after saving. It's still a draft and the new header is in place. I also opened the photo link to make sure it works.

**Credit and license:** the photo is CC0 (public domain), so no credit line is needed on the page. I left a hidden note in the page code that records the photographer and source.

**Before you publish:** the photo loads from Wikimedia Commons, because I can't add files to your WordPress Media Library from here. That works fine, but your site will be more reliable if the photo lives in your own Media Library:
1. Upload "Washington Square Arch

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
