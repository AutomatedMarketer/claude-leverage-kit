# Model picker

Model names as of October 2026. If the user's app shows different names, use the closest match:
the biggest model for the hardest jobs, the smallest for simple, high-volume ones.

## Contents
- The models
- Ambition level → model and effort
- Choosing the checker
- When a team of helpers is worth it
- How to set the model and effort in each app

## The models

The "watch out for" notes summarise Anthropic's published prompting guides for each model (October 2026).

| Model | Best for | Watch out for |
|---|---|---|
| **Haiku 5.5** | Quick, simple, repeated jobs: sorting, pulling facts out, short answers | At low effort on long jobs it can skip a step. Use medium |
| **Sonnet 5.5** | Most everyday work: writing, editing, well-defined coding, chat | At low effort it can skip checking its work. It sometimes adds extras nobody asked for |
| **Opus 5.5** | The default for important work: long tasks, analysis, complex writing and coding | Can stop early to report on long unattended jobs. Say clearly when the job is finished |
| **Fable 5.1** | The hardest, longest jobs, or when Opus at high effort still falls short | Uses the most of your plan. May not be on every plan. Can pause to ask before doing what was asked |

Not sure? Use **Opus 5.5 at medium effort**.

## Ambition level → model and effort

| Level | What it looks like | Model and effort | Setup |
|---|---|---|---|
| **Faster** | Same task, done quicker. Clear, low stakes | Sonnet low–medium, or Haiku medium for repeated simple jobs | Solo |
| **Deeper** | Done the way a top professional would: original data, real methods, a bold target | Opus medium; high when the target is hard | Solo plus a checker |
| **Wider** | Several fields and critics on something that matters | Opus medium leading; Sonnet medium helpers; Haiku for quick scans | Team of helpers (ask first) |
| **Outcome** | "Keep this true" or a long job that runs on its own | Opus medium; Fable high if Opus falls short | Solo plus a repeatable check |

**From the prompt optimizer's size:** Quick → Faster. Important with a team → Wider. Important
with "keep this true" or a repeatable workflow → Outcome. Any other Important job → Deeper.

Effort is the "how hard to think" dial. Higher effort is slower and uses more of the plan. Start
at the level above and only raise it when the result falls short.

## Choosing the checker

The checker is never the chat that did the work. Best first:

| Kind of work | Checker |
|---|---|
| Code, websites, data | A tool Claude runs after every change: tests, a build, a speed test, a validator |
| Facts and numbers | Check each claim against its source |
| Writing, slides, creative | A fresh chat or helper that sees only the result and a checklist, then the user |
| Big decisions | A second opinion from a fresh chat, or from a different AI |

## When a team of helpers is worth it

- **Worth it:** high stakes (a launch, a big client, money on the line), several fields matter, or spare usage would expire anyway.
- **Not worth it:** quick tasks, or anything one good reply can handle.
- **Cost:** roughly several times one reply (an estimate; it depends on the job and the number of helpers).
- **Before starting one:** tell the user how many helpers and which models, and ask.
- **Where it works:** helpers (subagents) run in Claude Code and the desktop app's coding mode. In a normal chat, run the experts one after another in the same reply instead.

## How to set the model and effort in each app

| App | Model | Effort |
|---|---|---|
| claude.ai (web) and the desktop app | The model menu by the message box | The effort menu next to the model name, where shown |
| Claude Code | Type `/model` | Type `/effort` |
| Helpers in Claude Code | Ask Claude to use a specific model for each helper | Ask for an effort level per helper |
