---
name: weekly-hotspots
description: "Weekly review for the Productivity Project vault. Invoke with '/weekly-hotspots', 'weekly review', 'review my hotspots', or 'where am I out of balance'. Scores life hotspots and work areas, estimates the week's hours per work area, sets next week's three. Run on maintenance day."
---

# Weekly Hotspots Review

Run from the vault root. About 30 minutes.

## Preflight

- Read `CLAUDE.md` (work areas table), `Now.md`, and the most recent `Reviews/YYYY-Www.md`.
- Read this week's `Daily/` notes. Group the Top 3 items by hotspot wikilink and compute the top-3 completion rate from `top3_done`. Daily notes do not carry hours.
- Read this week's lines in `Accomplishments.md`.

## Steps

1. **Empty the head.** Ask for everything on the owner's mind going into the week. Capture verbatim.
2. **Last week.** Read back the wins. Go through last week's 3: did each happen? Ask what got in the way.
3. **Life hotspots.** Score each 1-5 (1 neglected, 3 maintained, 5 thriving) with one question each: Mind (reading, learning, quiet thinking?), Body (movement, food, sleep?), Emotions (dominant tone, anything unprocessed?), Career (what moved, what stalled?), Finances (anything ignored?), Relationships (real time with the people who matter?), Fun (anything with no agenda?).
4. **Hours retro.** Hours are estimated once a week, not logged daily. Build the estimate from two sources, then let the owner correct it:
   - The week's Top 3 items in the daily notes, grouped by their hotspot wikilink (count of items per work area, and how many were done).
   - Their calendar for the week: ask for screenshots of their calendar's week view, or read it through a calendar connector if one is connected.
Propose hours per work area to the nearest hour, say what each number is based on, and ask "what's off?". Write the corrected numbers to the review's `hours_*` keys. If neither source exists for a day, ask rather than guess.
5. **Active work areas.** For each, show the agreed hours, then ask for a 1-5 score on how they feel about the area and one line on why. Name any mismatch: many hours with a low score, or a low score with almost no hours.
6. **Autopilot work areas.** Show hours against the cap and ask two yes/no questions: does someone need an answer from you, and is anything broken or costing money? Over cap or any yes earns a slot in next week's 3. Otherwise move on.
7. **Next week.** Ask for the week's 3 (each with a hotspot wikilink), when each gets prime time, and the one specific thing the owner is saying no to so those three get real time. Push past a soft answer on the no.
8. **Write.** Create `Reviews/YYYY-Www.md` (ISO week) from `Templates/Weekly Review.md` with the flat frontmatter keys (`life_*`, `score_*`, `hours_*`) filled. Then update `Now.md` (review date, week's 3, the no, work area tables) and the scores in `Hotspots/Hotspots Dashboard.md`. If a concern changed, append a dated line to that hotspot's page.
9. **Patterns.** With 4+ reviews on file, call out any hotspot at 2 or below for two weeks running, and any active work area with near-zero hours two weeks running. End with one observation.

## Rules

- No all-3s. Force differentiation.
- Always get one specific no.
- Hours are a weekly estimate the owner confirms. Say what each number is based on.
- End with an observation, not a to-do list.
