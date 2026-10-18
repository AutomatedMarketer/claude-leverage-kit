# 03 · The right model

Claude comes in several sizes. Bigger models think better but use more of your plan. The
model picker matches the model, and how hard it thinks, to the job.

## How to use it

Ask:
- "Which model should I use for this?"
- "Opus or Sonnet for …?"
- "What effort level for …?"
- "Is this worth a team of helpers?"

You get an answer like:

```
Model: Opus 5.5   Effort: medium   Setup: solo
Checker: a fresh chat with the checklist, then you
Why: important client work that needs careful reasoning, but not a team
How to set it: model menu by the message box → Opus 5.5; effort menu → Medium
```

## The models (October 2026)

| Model | Think of it as | Use it for |
|---|---|---|
| **Haiku 5.5** | The fast assistant | Sorting, pulling facts out, short answers, lots of small jobs |
| **Sonnet 5.5** | The all-rounder | Everyday writing, editing, chat, clear coding tasks |
| **Opus 5.5** | The senior expert | Important work, analysis, long tasks. **The default when unsure** |
| **Fable 5.1** | The specialist for the hardest problems | Very hard, very long jobs, when Opus isn't enough. Uses the most of your plan |

Names change as new models come out. The rule doesn't: the biggest for the hardest jobs, the
smallest for simple, repeated ones.

## Effort: how hard it thinks

Effort is a dial: low, medium, high (sometimes more). Higher is slower and uses more of your plan.

- **Start at medium** for most important work.
- **Use low** for quick, simple jobs.
- **Raise it** only when the answer falls short.

Where to set it:

| App | Model | Effort |
|---|---|---|
| claude.ai and desktop app | Model menu by the message box | Effort menu next to the model name, where shown |
| Claude Code | `/model` | `/effort` |

## Match the model to the ambition

| You want | Model | Setup |
|---|---|---|
| **The same thing, faster** | Sonnet (or Haiku for repeated simple jobs) | Solo |
| **The expert's way** | Opus, medium | Solo plus a checker |
| **Many points of view** | Opus leading, Sonnet helpers | A team of helpers (ask first) |
| **Something kept true over time** | Opus; Fable if Opus falls short | Solo plus a check that runs every time |

## Teams of helpers

A team means several AI helpers work on parts of the job at once, with some acting as critics.

- **Great for:** launches, big clients, important decisions.
- **Not worth it for:** quick tasks.
- **Cost:** roughly several times one reply. The kit always asks first.
- **Where:** helpers run in Claude Code. In a normal chat, the kit runs the experts one after another instead.

## The one rule that matters most

**The checker is never the model that did the work.** AI is agreeable and grades itself too
kindly. Use a tool (tests, a speed check), a fresh chat that only sees the result and the
criteria, or yourself.
