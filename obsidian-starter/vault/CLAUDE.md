# Productivity vault

This vault is a daily and weekly operating system built on Chris Bailey's *The Productivity Project*. It is also the context store: read it before advising the owner on priorities.

## Read at the start of every session here

1. `Now.md` for current state: prime time, maintenance day, this week's 3, work areas, open decisions, last review dates.
2. The most recent 3 files in `Daily/` (named `YYYY-MM-DD.md`).
3. The most recent file in `Reviews/` (named `YYYY-Www.md`).

If the last daily note is more than 2 days old or the last review more than 8 days old, say so in one line before anything else. Do not lecture.

## Work areas

Edit this table once. Each `key` appears as `hours_<key>` (plus `score_<key>` for active areas) in `Templates/Weekly Review.md`. Frontmatter is kept flat because Obsidian's Properties panel cannot edit nested values.

| key | Page in `Hotspots/Work/` | Type |
|-----|--------------------------|------|
| area_one | Work Area One | active |
| area_two | Work Area Two | active |
| side_one | Side Commitment One | autopilot |

- **active**: gets a weekly hours estimate and an optional 1-5 feeling score. Life hot spots are never scored; the book asks only for a list that is scanned weekly.
- **autopilot**: gets hours against a weekly cap and two yes/no questions (does someone need an answer from me; is anything broken or costing money). No score.

## What gets logged, and where

| What | Where | When |
|------|-------|------|
| Today's 3, brain dump, tasks | `Daily/YYYY-MM-DD.md` body | Morning |
| Energy 1-10, top-3 done count | `Daily/YYYY-MM-DD.md` frontmatter | End of day |
| Hours per work area, estimated in a weekly retro from the week's tagged Top 3 items and the owner's calendar | `Reviews/YYYY-Www.md` frontmatter | Maintenance day |
| One win per day | `Accomplishments.md` (newest first) | End of day |
| The hot spots scan (what was neglected, what goes on the radar), work area hours and optional feeling scores, the week's 3, the intentional no | `Reviews/YYYY-Www.md` | Maintenance day |
| The hot spots list: the few things that belong under each area of life, plus optional weekly timeboxes | `Hotspots/Hotspots Dashboard.md` | Built once, scanned and adjusted at each weekly review |
| Current concern, the number the owner watches, open decisions, dated log | `Hotspots/Work/*.md` and `Hotspots/*.md` | When it changes |
| Current state snapshot | `Now.md` | Rewritten at wrap-up and weekly review |

## Rules

- Every item in Today's 3 and every weekly item ends with a wikilink to its hotspot, e.g. `[[Work Area One]]` or `[[Body]]`. Backlinks build the graph. Add the link if it is missing.
- Daily frontmatter keys are fixed: `energy` and `top3_done` (how many of the day's three got done, 0-3). Hours are not logged daily. The weekly review's `hours_<key>` and `score_<key>` must match the work areas table.
- Capture the owner's words verbatim in dumps and reflections. Do not polish.
- History lives in dated files in the vault. `Now.md` and the dashboard show only the current state.
