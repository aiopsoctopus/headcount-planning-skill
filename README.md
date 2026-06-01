# Headcount Planning Skill for Claude / Cowork

A Claude skill that turns whatever people data you have — a roster export, a list of open roles, two ARR numbers on a sticky note — into a board-ready headcount model. Six-tab Excel. Live formulas. Every assumption flagged before it goes anywhere near a deck.

---

## What it builds

One `.xlsx` file with:

- **Assumptions** — every editable input in one place. Change a rate here, the whole model updates.
- **Current Headcount** — roster snapshot by department, level, and fully-loaded cost
- **Hiring Plan** — proposed hires by quarter, with base and prorated fully-loaded cost per role
- **Scenario Comparison** — conservative vs. aggressive side-by-side: headcount delta, total cost delta, must-have roles in both
- **Cost Summary** — fully-loaded annual cost by department, both scenarios
- **Assumption Log** — every number Claude estimated, yellow-highlighted, with the reasoning — so you can review before sharing

---

## What you need to get started

Drop these into your project folder. The skill works with whatever you have — it'll tell you what's missing.

**Roster file** (CSV or Excel) — name, department, title/level, base salary, location, status (active/open). Even a rough one works.

**Hiring priorities** (a text file is fine) — list of roles you want to add, which quarter you're targeting, must-have vs. nice-to-have. 

**Two ARR scenarios** — a conservative and an aggressive growth rate. Even two numbers in a Slack message is enough.

No comp data for a new role? Claude will estimate a midpoint based on level and market, flag it in the Assumption Log, and move on. You review and override before the deck goes to anyone.

---

## How to install

1. Download `headcount-planning.skill`
2. Open Cowork
3. Drag the `.skill` file into the Cowork window — it installs automatically
4. Done. The skill is now available in any Cowork project.

---

## How to use it

1. Create a folder for your headcount planning inputs (wherever you keep your project files)
2. Drop in your roster export, a hiring priorities text file, and your ARR scenarios
3. Open Cowork, point it at that folder, and say something like:

   > "Build me a headcount plan from the files in this folder."

   Or more specific:

   > "Model two hiring scenarios — 18% and 32% ARR growth — using the roster and open roles I uploaded."

Claude will read what's there, ask about anything critical that's missing, and build the model. It'll tell you exactly what it assumed and what needs your eyes before you share it.

---

## A few things worth knowing

Yellow cells in the Assumption Log are Claude's estimates — comp midpoints for roles without data, overhead costs if you didn't provide them, timing assumptions if a start date wasn't specified. Those need your review. The model is only as good as the inputs, and Claude will be the first one to tell you that.

Everything traces back to the Assumptions tab. Change the benefits load rate once and every department's fully-loaded cost updates. No hunting down hardcoded numbers buried three tabs deep.

The Scenario Comparison tab shows which hires appear in both scenarios — those are your must-haves regardless of which ARR number wins. That's usually the clearest thing you can put in front of a board.

---

## Built by

Christina Moore — People Ops & Finance operator, AI Ops Octopus on Substack.

If you found this useful, the full freebie template (PDF version, for when you want something to print and scribble on) lives [here](https://aiopsoctopus.substack.com).

🐙
