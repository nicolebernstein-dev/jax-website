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
**Status:** on track — Landing page header, photo, button, and spacing fixed; awaiting preview and Pardot form build

**Done this session**
- Removed gap between nav bar and photo by relocating hidden note and eliminating extra paragraphs
- Updated 'Reserve my seat' button to match site style (orange pill, white text, outline hover)
- Made 'Revecast Orchestrate' link bold
- Updated NYU line to: 'NYU joins us in person to share their story firsthand.'

**Open items**
- Preview landing page on mobile and desktop; confirm header, photo spacing, button style, and text readability
- Build Pardot Form A (Registered action) with five hidden UTM fields
- Build Pardot Form B (Waitlisted action) as copy of Form A
- Create two confirmation email templates (registered and waitlist)
- Provide iframe links for Form A and Form B
- Provide five UTM Field IDs from Pardot prospect field settings

**Decisions**
- Campaign type: Seminar/Conference
- Event date: December 2, 2026
- Header: solid white bar with dark logo/menu; photo below with no gap
- Header photo: Washington Square Arch with One Fifth Avenue, clear blue sky, gradient tint (dark left, light right)
- Photo credit: displayed in bottom-right corner (CC BY-SA 4.0)
- Button style: orange pill (#ff9a00) with bold white text, orange outline on hover
- Thank-you pages at /nyc-education-ai-2026/thank-you/ and /nyc-education-ai-2026/waitlist/
- UTM capture via script on landing page (iframe limitation)

**Blockers**
- None

**Next**
- Preview rendered landing page on desktop and mobile; verify nav-to-photo spacing, button appearance, and text contrast
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
I've made all four changes to the draft landing page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). After saving, I checked the page WordPress now outputs: the changes are in it, and the page is still a draft.

| Your feedback | What I changed |
|---|---|
| Gap between the nav bar and the photo | The gap came from a hidden note at the top of the page. WordPress was wrapping it in an empty paragraph, and that pushed the photo down. I moved the note inside the header section and stopped WordPress from adding those extra paragraphs. As a backup, I also set the page content to start right under the nav bar with no spacing. |
| Button should match the site | The "Reserve my seat" button now uses the same button style as the rest of the site, like the "Learn More" button in your screenshot. It's an orange (#ff9a00) pill shape with bold white text, and it turns to an orange outline when you hover over it. |
| Bold "Revecast Orchestrate" link | Done. The link is now bold. |
| NYU line under the title | It now reads: **"NYU joins us in person to share their story firsthand."** |

**Please check the preview:** I can't see the rendered page from here, so look at it on a

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
