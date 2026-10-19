# Quota maximizer

Paid Claude plans have usage limits that reset on a schedule: a short session window (a few
hours) and a weekly limit. Weekly usage you don't spend before the reset is gone. This part
finds that spare usage and spends it on the most valuable work, never on busywork.

## Contents
- Step 1: get the numbers
- Step 2: the verdict
- Step 3: the spend list
- Step 4: spend safely
- Step 5: the wrap-up
- What this part never does

## Step 1: get the numbers

Easiest: ask the user for a screenshot of the usage page and read it. Otherwise ask for:
- **Weekly usage % used**
- **Strongest-model % used**, if the app shows a separate limit for it
- **When the weekly limit resets** (date and time)
- **Session usage % used** (the short window)

Where to find them:

| App | Where |
|---|---|
| claude.ai and the desktop app | Settings → Usage |
| Claude Code | Type `/usage` |

Always read the reset date and time from the usage page. Don't rely on memory or assume a day.

## Step 2: the verdict

`remaining = 100 − weekly % used`. `hours left = time until the weekly reset`.

| Verdict | When | What to say |
|---|---|---|
| **Spend now** | remaining ≥ 20% and hours left ≤ 48 | Build the spend list (Step 3) |
| **Spend tomorrow** | remaining ≥ 40% and hours left 48–72 | "Tomorrow is a good day to use spare capacity. Line up your projects." |
| **Running hot** | strongest-model ≥ 70% used with 3+ days left | "Slow down on the biggest model or you may be locked out before the reset." |
| **Nothing to do** | Anything else | "You're on pace. Nothing to do." |

## Step 3: the spend list

Ask which projects are active right now (or look at the current project folder in Claude Code).
Build 3–7 items, best first. Prefer work that's normally too expensive to do:

| Kind | Example | Why spare usage suits it |
|---|---|---|
| **Make it repeatable** | Turn a weekly task into a workflow or checklist Claude can run every time | Saves time every week after this |
| **Expert team review** | Specialists plus two critics review the most important thing you're about to launch | Several times the cost of one reply, so normally skipped |
| **Deep check** | "We believe X. Check it against the full data." | Slow and data-heavy |
| **Get ahead** | Draft next week's content, research, plans | Useful, lower priority |

Format each item:

```
1. <project> — <what to do>
   Kind: <make it repeatable / expert team / deep check / get ahead>
   Size: <small ≈ 1–2% / medium ≈ 3–5% / large ≈ 6–10% of the week>
   Model: <from Part 2>   Checker: <outside check>
```

If the user has no real projects to improve, say so and stop. Unused usage beats fake work.

## Step 4: spend safely

```
For each item:
- [ ] Build the prompt with Part 1 (important size)
- [ ] Pick model, effort and checker with Part 2
- [ ] Check usage: remaining % > item size + 10%? If not, pick a smaller item
- [ ] Do the work
- [ ] Run the outside check. Failed → fix and re-check, or report it as unfinished
- [ ] Check usage again before the next item
```

- **Keep 10% spare** for emergencies before the reset: stop starting new items at 90% used. Hitting 100% can lock the user out until the reset.
- **Use lower effort for most items** so the spare usage covers more work. Save high effort for the single hardest item.
- **Ask before** anything that sends, publishes, spends money, deletes or touches live accounts.

## Step 5: the wrap-up

Finish with:
- What got done, and which checks passed
- What's left unfinished, and why
- Usage before vs. after

## What this part never does

- Invent busywork to use up the plan
- Start an item that can't finish before the limit
- Count an item as done before its outside check passes
- Take any outside action (send, post, buy, delete) without asking
