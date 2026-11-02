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
**Status:** on track — Landing page header redesigned with wider Washington Square Park photo; awaiting mobile preview, photo upload, and form/email copy

**Done this session**
- Removed blue gradient overlay; replaced with dark tint and soft text shadow
- Changed header photo to wider Washington Square Park shot showing fountain, Arch, and Manhattan towers
- Moved 'Spaces are limited' text under form box
- Updated address to 'Salesforce Tower' only
- Added full-width blue brand band for first two paragraphs below header
- Reordered bullets: NYU story now first under 'What you will leave with'
- Added link to Revecast Orchestrate for Higher Education solution page

**Open items**
- Preview landing page on mobile device before publishing
- Upload Washington Square Arch photo to WordPress Media Library; send new link to switch from Wikimedia Commons
- Decide on photo credit display (currently shows 'Photo: Ajay Suresh, CC BY 2.0' in bottom-right corner)
- Build Pardot Form A (Registered action) with five hidden UTM fields
- Build Pardot Form B (Waitlisted action) as copy of Form A
- Create two confirmation email templates (registered and waitlist)
- Provide iframe links for Form A and Form B
- Provide five UTM Field IDs from Pardot prospect field settings

**Decisions**
- Campaign type: Seminar/Conference
- Campaign status: Planned and Active
- Event date: December 2, 2026
- Member statuses: Registered (default), Waitlisted, Attended, No Show
- Use Registered count for seat availability
- UTM capture via script on landing page (iframe limitation)
- Thank-you pages at /nyc-education-ai-2026/thank-you/ and /nyc-education-ai-2026/waitlist/
- Header photo: wider Washington Square Park shot with dark tint and soft text shadow (no blue gradient)

**Blockers**
- None

**Next**
- Preview landing page on mobile; confirm layout and readability
- Upload Washington Square Arch photo to Media Library; send link to replace Wikimedia Commons source
- Confirm photo credit approach (keep or find public-domain alternative)
- Build Pardot Form A and Form B with UTM hidden fields and campaign member actions
- Create two confirmation email templates for autoresponder use
- Send iframe links, UTM Field IDs, and email/thank-you page wording

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
I've made all seven changes to the draft landing page: [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). I read the page back after saving and the changes are there. It's still a draft and hasn't been published.

| Your request | What I did |
|---|---|
| Remove the header overlay | Removed the blue gradient. The photo now has a plain dark tint, plus a soft shadow behind the white text so it stands out. |
| New photo that clearly shows NY | Changed to a wider shot of Washington Square Park. It shows the fountain, the Arch and the Manhattan towers behind them. |
| "Spaces are limited" under the form | Moved it under the form box. "Hosted by Jax Consulting in partnership with Salesforce" is still where it was. |
| Address | The hero now says just "Salesforce Tower". |
| First two paragraphs on blue | They're now in a full-width band in your brand blue, right below the header. The rest of the page is still white. |
| NYU story first | It's now the first bullet under "What you will leave with". |
| Link to Revecast Orchestrate once | The first "Revecast Orchestrate" under "What is Orchestrate?" links to [Orchestrate for Higher Education](https://revecast.io/solutions-

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
