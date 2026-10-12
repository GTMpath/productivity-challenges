---
name: daily-checkin
description: "Morning check-in for the Productivity Project vault. Invoke with '/daily-checkin', 'daily check-in', 'morning check-in', or 'start my day'. Creates today's daily note, takes a brain dump, and sets the day's three."
---

# Daily Check-In

Run from the vault root. Read `CLAUDE.md` and `Now.md` first.

## Steps

1. **Create today's note.** `Daily/YYYY-MM-DD.md` (local date) from `Templates/Daily Note.md`, replacing `{{date}}`. If it exists, continue in it.
2. **Status in three lines.** This week's 3 from `Now.md`, carryovers already in today's note, and how many days since the last daily note if more than 2.
3. **Brain dump.** Ask "What's on your mind?" and write the answer verbatim under Brain Dump. Sort anything actionable into Do Today, Waiting On, Quick Wins, or Captured for Later.
4. **Today's 3.** Ask: "Picture the end of today. What three things do you want done?" Suggest candidates from the dump and the week's 3, but the owner chooses. End each with a hotspot wikilink.
5. **Prime time.** Ask which of the three gets the prime-time block and when, and where the 30-minute offline block goes. Write both in.
6. **Close.** Read the three back in one line each and stop.

## Rules

- Three items, not four. If the owner lists more, ask which three.
- Do not polish the brain dump.
- No lecture about missed days.
