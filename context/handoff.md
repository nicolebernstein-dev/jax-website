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
**Status:** on track — Landing page header rebuilt with solid nav bar and calmer photo; awaiting mobile preview and form/email build

**Done this session**
- Moved site header from floating overlay to solid white bar; photo now starts below
- Replaced busy Washington Square Park photo with calmer Washington Square Arch shot under clear sky
- Applied gradient tint (darkest left, lighter right) to improve text readability
- Fixed side padding on white copy section; aligned with blue band margins
- Made date, time, location bold
- Updated photo credit to 'Photo: BruceSchaff, CC BY-SA 4.0'

**Open items**
- Preview landing page on mobile and desktop; confirm header, photo, and text readability
- Build Pardot Form A (Registered action) with five hidden UTM fields
- Build Pardot Form B (Waitlisted action) as copy of Form A
- Create two confirmation email templates (registered and waitlist)
- Provide iframe links for Form A and Form B
- Provide five UTM Field IDs from Pardot prospect field settings
- Confirm photo credit approach (current: CC BY-SA 4.0 attribution in bottom-right)

**Decisions**
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Header: solid white bar with dark logo/menu; photo below
- Header photo: Washington Square Arch with One Fifth Avenue, clear blue sky, gradient tint (dark left, light right)
- Photo credit: displayed in bottom-right corner
- Thank-you pages at /nyc-education-ai-2026/thank-you/ and /nyc-education-ai-2026/waitlist/
- UTM capture via script on landing page (iframe limitation)

**Blockers**
- None

**Next**
- Preview rendered landing page on desktop and mobile; check header bar, photo, and text contrast
- Build Pardot Form A with five hidden UTM fields and Registered member action
- Build Pardot Form B as copy of Form A with Waitlisted member action
- Create two confirmation email templates for autoresponder
- Send iframe links, UTM Field IDs, and email/thank-you page copy

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
I've made all four changes to the draft landing page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). I read the page back after saving: the changes are there and it's still a draft.

| Your feedback | What I changed |
|---|---|
| Nav shouldn't sit on the image | The site header is normally see-through and floats over the first section. On this page only, it's now a solid white bar with the dark logo and dark menu links, and the photo starts below it. The rest of the site is unchanged. |
| Image too busy, X still showing, hard to read | **The X pattern is gone.** I also replaced the photo with a calmer one: the Washington Square Arch with One Fifth Avenue behind it under a clear blue sky, in autumn. The tint is darkest on the left behind the text and lighter on the right. |
| Side padding on the copy | Fixed. The white section had lost its side margins, so I put it in the site's standard page container, the same one the blue band uses. Both sections now line up with the same side spacing. |
| Bold date, time and location | "Wednesday, December 2, 2026 / 1:30–4:30 PM ET / Salesforce Tower" is now bold. |

**Photo credit:** this photo is CC BY-SA 4.0, so it needs

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
