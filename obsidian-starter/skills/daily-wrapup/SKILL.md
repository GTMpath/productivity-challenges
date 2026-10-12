---
name: daily-wrapup
description: "End-of-day wrap-up for the Productivity Project vault. Invoke with '/daily-wrapup', 'wrap up the day', 'end of day check-in', or 'close out today'. Fills End of Day, logs energy, records one win, rolls carryovers into tomorrow."
---

# Daily Wrap-Up

Run from the vault root. Read `CLAUDE.md` (for the work areas table) and today's `Daily/YYYY-MM-DD.md`. If today's note does not exist, offer to create it and skip to step 4.

## Steps

1. **What got done?** Anchor against Today's 3. Push past "stuff" to specifics.
2. **What's carrying over, and why?** For each: blocked, out of time, deprioritized, or forgot.
3. **One win.** Even a small one.
4. **Energy.** Ask for energy out of 10. Write `energy` and `top3_done` (0-3) into the note's frontmatter. Do not ask for hours; those are estimated once a week. Make sure each of today's Top 3 ends with a hotspot wikilink, because the weekly hours retro groups by them.
5. **Write it down.** Answers go verbatim into End of Day. Prepend the win to `Accomplishments.md` as `- YYYY-MM-DD: <win> [[Hotspot]]`.
6. **Roll carryovers.** Add each to tomorrow's note under Do Today (create the note from the template if needed) with the reason in italics. Anything deprioritized goes to Captured for Later instead; ask if unclear.
7. **Update `Now.md`.** Set "Last daily note" to today.
8. **Close.** If it is Friday through Sunday and the last review in `Reviews/` is more than 6 days old, mention the weekly review. End with a two-line summary.

## Rules

- Capture verbatim. Ask, do not prescribe.
- If the same item has carried 3 days running, ask whether to drop it or block time for it.
- End with the day closed, not with a new to-do list.
