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
### Engagement state — 2026-11-11
**Status:** at risk — Page updates live & verified. Link migration runbook ready for WordPress admin. Karen notification still blocked.

**Done this session**
- Validated search-and-replace strategy on 3 live pages; tested 16 rewritten URLs—all load correctly
- Created WordPress admin runbook with dry-run steps, undo plan, and CLI alternative

**Open items**
- WordPress admin executes link migration (3 replacements in order, dry run first, cache clear, spot-check)
- Recheck all 20 pages and test every link after migration completes
- Test live page in browser on computer and phone; verify form position, heading sizes, spacing
- Submit test registration and confirm thank-you page redirect works
- Confirm Pardot email greeting wording matches 'Hi,' or report actual text
- Remove 2 test leads from Salesforce campaign
- Send Karen notification—requires her Slack member ID, alternative channel, or manual copy-paste

**Decisions**
- Completion action order: Assign prospect → Add to Salesforce Campaign → Send autoresponder → Notify user → Add tag
- At 30 registrations: swap campaign Status to Waitlisted and email to Waitlist Confirmation
- Campaign type: Seminar/Conference; Event date: December 2, 2026
- Single Pardot form handles both Registered and Waitlisted actions
- Heading sizes 28px; 'Spaces are limited.' 14px with line space after Reserve button
- Link migration: case-study replacement must run first to avoid old addresses

**Blockers**
- Slack token type does not allow message search or member lookup—cannot identify or contact Karen without external input
- 17 of 20 audit pages not yet tested for sandbox/localhost links; migration may surface unmapped addresses

**Next**
- WordPress admin: back up live database, install Better Search Replace, run dry run of 3 replacements in order
- WordPress admin: execute replacements, clear caches, spot-check for pantheonsite and localhost in page source
- WordPress admin: report completion; session will recheck all 20 pages and test every link
- Provide Karen's Slack member ID, alternative contact channel, or send draft message yourself

**Checked live on 2026-11-11:** nothing — the status above is as recorded, not re-checked
### Last session — 2026-11-11
| | |
|---|---|
| Type | BUILD |
| Outcome | COMPLETED |
| Branch | `main` |
| Name | Jax Site Updates |
| Session | `6f0571c3-0a1e-497d-bea1-497f5e8f0665` |
**In its own words (excerpt):**
A search-and-replace will work even though the links are unique. The replace only swaps the wrong start of each link and keeps the rest exactly as it was. For example, `live-jax-consult.pantheonsite.io/services/data-ai/` becomes `www.jaxconsult.com/services/data-ai/`.

I tested this today on Home, Industries > Nonprofit and Industries > Public Sector. I pulled 19 unique sandbox and localhost links from those pages, swapped the start, and got 16 distinct live addresses. All 16 load a working page on www.jaxconsult.com, including service pages, case studies (moved to /insights/) and images.

**Steps for your WordPress admin:**
1. **Back up the live database** in Pantheon: Live → Backups → Create New Backup.
2. **Install Better Search Replace** (Plugins → Add New), then open it from Tools → Better Search Replace.
3. **Do a dry run of three replacements, in this order,** with all tables selected:
   - `live-jax-consult.pantheonsite.io/case-study/` → `www.jaxconsult.com/insights/`
   - `live-jax-consult.pantheonsite.io` → `www.jaxconsult.com`
   - `http://localhost/jax-consulting` → `https://www.jaxconsult.com`
4. **Check the counts** from the dry run look sensible.
5. **Run all three f

_[summary truncated — see the session record for the full text]_
<!-- orchestrate:session-state:end -->
