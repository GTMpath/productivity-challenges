# Obsidian Starter Vault

A small Obsidian vault for running *The Productivity Project* as a daily and weekly routine. It takes 10 to 15 minutes a day and 30 minutes once a week, and you can do all of it by hand. If you use Claude Code, three optional skills run the check-ins as a conversation and do the writing for you.

## What you get

| File | What it is for |
|------|----------------|
| `Templates/Daily Note.md` | Brain dump, the day's three, tasks, end-of-day reflection, and two properties at the top for energy and how many of the three got done |
| `Templates/Weekly Review.md` | Hotspot scores, hours per work area, next week's three |
| `Now.md` | One page showing where things stand this week |
| `Hotspots/` | Your hot spots list on one page, a page per hot spot that collects its history, and three example work area pages |
| `Accomplishments.md` | One win a day |
| `Daily Practice.md` | The routine, written out |
| `CLAUDE.md` | Tells Claude Code what to read and where to log things. Delete it if you do not use Claude Code. |

## What it looks like

```
vault/
├── Now.md                      where things stand this week
├── Daily Practice.md           the routine, written out
├── Accomplishments.md          one win a day
├── Daily/
│   └── Example day (delete me).md
├── Reviews/                    one dated note per week
├── Hotspots/
│   ├── Hotspots Dashboard.md   your hot spots list, on one page
│   ├── Mind.md, Body.md, Emotions.md, Career.md,
│   │   Finances.md, Relationships.md, Fun.md
│   └── Work/
│       ├── Work Area One.md
│       ├── Work Area Two.md
│       └── Side Commitment One.md
└── Templates/
    ├── Daily Note.md
    └── Weekly Review.md
```

`Daily/Example day (delete me).md` is a filled-in day, so you can see a finished note before you write your own. Each daily note has two properties at the top:

```
energy: 7
top3_done: 2
```

Hours per work area are estimated once a week in the review, from the links on the week's daily threes and your calendar.

Every one of the day's three ends with a link such as `[[Work Area One]]` or `[[Body]]`. Open Obsidian's graph view after a week and each hotspot page shows the days that fed it.

## Install

1. On the repo's GitHub page, click **Code**, then **Download ZIP**, and unzip it.
2. Choose one:
   - **New vault:** open Obsidian's vault manager (click the vault name at the bottom left, then **Manage vaults**), choose **Open folder as vault**, and select `obsidian-starter/vault`.
   - **Existing vault:** copy everything inside `obsidian-starter/vault` into your vault's folder. If your vault already has any of these folders or files, copy them across one at a time so nothing gets overwritten. Steps 4 and 5 below will also change your current Templates and Daily notes settings. Do not copy the hidden `.obsidian` folder, which would replace your own settings.

A new vault opened this way is already configured, so skip to "Make it yours". For an existing vault, do these three steps:

3. In Obsidian, open **Settings**, then **Core plugins**, and turn on **Templates** and **Daily notes**.
4. Under **Templates**, set **Template folder location** to `Templates`.
5. Under **Daily notes**, set **Date format** to `YYYY-MM-DD`, **New file location** to `Daily`, and **Template file location** to `Templates/Daily Note`.

## Make it yours (10 minutes)

1. Open `Now.md` and fill in your prime time (the hours when your energy is highest) and your maintenance day (the day you do the weekly review and batch your chores).
2. Decide your work areas. Split your job into the two to four areas you are responsible for, and add any side commitment you want kept on autopilot. `Daily Practice.md` explains the difference.
3. Rename the three example pages in `Hotspots/Work/` to match. Obsidian updates the links in your other notes when you rename a page from inside the app.
4. Pick a short key for each area, such as `sales` or `hiring`. Replace `area_one`, `area_two` and `side_one` with your keys in the properties at the top of `Templates/Weekly Review.md` and in the work areas table in `CLAUDE.md`. Change the page names in that table too, because Obsidian does not update them for you.
5. Open `Hotspots/Hotspots Dashboard.md` and write a few items under each hot spot: the things in that part of your life that need your time. This takes about ten minutes, and the list should stay short enough to scan in a minute.
6. If you have more or fewer than three areas, add or remove the matching properties in the Weekly Review template, the row in the `CLAUDE.md` table, the row in the tables in `Templates/Weekly Review.md` and `Now.md`, and the line under Career in `Hotspots/Hotspots Dashboard.md`.

The seven life hotspots come from the book. To add one, create a page for it in `Hotspots/`, then add a section and a score row to the dashboard, a row to the Weekly Review table, and a `life_` property at the top of the Weekly Review template.

## Use it

**Each morning.** Click the calendar icon in the left sidebar (**Open today's daily note**). Dump what is in your head, write your three, and pick which one gets your prime time.

**Each evening.** Fill in End of Day and add one line to `Accomplishments.md`. Then type your energy out of 10 and how many of your three got done into the two properties at the top of the note.

**Once a week.** Right-click the `Reviews` folder, choose **New note**, and name it for the week, such as `2026-W42`. Open the command palette (Cmd or Ctrl + P), run **Templates: Insert template**, and pick Weekly Review. Scan your hot spots list, estimate the week's hours per work area from your daily threes and your calendar, score each hot spot, and write next week's three. Then update `Now.md`.

## Optional: Claude Code skills

1. Copy the three folders inside `obsidian-starter/skills` into `~/.claude/skills/`.
2. Open a terminal in your vault folder and run `claude`.
3. Type `/daily-checkin` in the morning, `/daily-wrapup` at the end of the day, and `/weekly-hotspots` on maintenance day.

Claude asks the questions, writes your answers into the right notes in your own words, estimates the week's hours with you (it can read screenshots of your calendar), and keeps `Now.md` current. Because `CLAUDE.md` is in the vault, Claude Code is told at the start of every session there to read `Now.md` and your last few notes first.
