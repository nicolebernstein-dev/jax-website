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
**Status:** on track — Landing page draft updated: photo credit and NYU header line refined. Ready for preview and Pardot form build.

**Done this session**
- Updated photo credit to plain text: 'Photo: BruceSchaff, CC BY-SA 4.0'
- Revised NYU header line to: 'NYU joins us in person to share their story.'

**Open items**
- Preview landing page on mobile and desktop; confirm header, photo spacing, button style, and text readability
- Decide: remove 'first-hand' from blue section ('Hear first-hand how NYU is using AI…') or keep it
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
- Photo credit: plain text in bottom-right corner (CC BY-SA 4.0)
- Button style: orange pill (#ff9a00) with bold white text, orange outline on hover
- Thank-you pages at /nyc-education-ai-2026/thank-you/ and /nyc-education-ai-2026/waitlist/
- UTM capture via script on landing page (iframe limitation)

**Blockers**
- None

**Next**
- Preview rendered landing page on desktop and mobile; verify nav-to-photo spacing, button appearance, text contrast, and photo credit placement
- Confirm: keep or remove 'first-hand' from blue section copy
- Build Pardot Form A with five hidden UTM fields and Registered member action
- Build Pardot Form B as copy of Form A with Waitlisted member action

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
I've made both changes to the draft landing page, [From Roadmap to Reality](https://www.jaxconsult.com/?page_id=3065). The saved page includes them, and it's still a draft.

- **Photo credit:** it's still there, but as plain text with no links: "Photo: BruceSchaff, CC BY-SA 4.0". Its position and style haven't changed.
- **NYU line in the header:** it now reads **"NYU joins us in person to share their story."**

The blue section below the header still uses "first-hand" once: "Hear first-hand how NYU is using AI…". You only asked about the header, so I left that one alone. Tell me if you want it removed there too.

Sources: checked live: the draft page before the edit, and the saved version WordPress sent back after the edit · not checked: how the page looks on screen
<!-- orchestrate:session-state:end -->
