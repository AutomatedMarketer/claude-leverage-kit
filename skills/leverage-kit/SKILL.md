---
name: leverage-kit
description: Makes any Claude request more ambitious and better aimed, in three parts that chain together or run alone. (1) Prompt optimizer rewrites a rough or rambling request into a strong prompt with the real outcome, an expert's methods, raw inputs, a clear output and an outside check. (2) Model picker chooses the Claude model, effort level and whether a task deserves a team of helpers. (3) Quota maximizer reads how much of a Claude plan is left before the weekly reset and turns spare usage into the most valuable work. Use when the user says "improve this prompt", "optimize this prompt", "make this better", "make this more ambitious", "go deeper", "which model should I use", "Opus or Sonnet", "what effort level", "how much usage do I have left", "my limit resets soon", "don't waste my plan", or pastes a long messy request. Works in claude.ai, the Claude desktop app and Claude Code.
---

# Leverage Kit

Three parts. Each works alone. Together they run in this order:

```
1. Prompt optimizer   →   2. Model picker   →   do the work   →   outside check
   what to ask for         which model,                           something other than
   and how to check it     effort, helpers                        the model grades it
                    3. Quota maximizer feeds both, using spare usage before the reset
```

## Which part to run

| The user… | Run |
|---|---|
| Pastes a rough request, asks to improve or "go deeper" on a prompt | Part 1, then offer Part 2 |
| Asks which model or effort to use, or whether to use helpers | Part 2 (run Part 1 first if the task is important and has no clear brief) |
| Asks about usage left, the reset, or "what should I do with my spare usage" | Part 3 (it uses Parts 1 and 2 for every item) |
| Asks to "do this really well" on something important | Parts 1 → 2 → do it |

## Rules for every part

- **Talk plainly.** Many users are new to Claude. Short sentences. Explain any term the first time.
- **Ambition never widens permission.** Never send, publish, spend, delete or change live accounts because a prompt got bolder. Ask first, every time.
- **The checker is never the model that did the work.** Models grade their own work too kindly. Use a tool (test, speed check, validator), a fresh helper that sees only the result and the criteria, or the user.
- **Ask before anything expensive.** A team of helpers uses several times more of the user's plan than one reply. Say so and ask, unless Part 3 is spending usage that would expire anyway.
- **Never invent facts.** Missing information becomes a question or a clearly marked gap.

## Part 1: Prompt optimizer

1. Read the whole request. Write the core intent in one sentence. If you can't, ask one question.
2. **Size the job.**
   - **Quick** (clear, low stakes): fill the template, done.
   - **Important** (money, clients, a launch, a meeting will discuss it, or it keeps coming back): run the ambition booster first. See [references/ambition-booster.md](references/ambition-booster.md).
3. Fill the template in [references/prompt-optimizer.md](references/prompt-optimizer.md). Keep the user's own words and voice.
4. Important jobs must have a `Who checks it` line naming an outside check.
5. Hand back the prompt in one code block. Offer Part 2 to choose the model, then ask: "Run it now, or copy it into a new chat?"
6. **When Part 2 or Part 3 asked for the prompt** (the user already wants the work done), skip step 5: don't print or ask, just carry on.

## Part 2: Model picker

1. Decide the **ambition level**: Faster, Deeper, Wider (a team of helpers) or Outcome (keep something true over time).
2. Pick model and effort from the table in [references/model-picker.md](references/model-picker.md).
3. Pick the checker (never the same chat that did the work).
4. Check the model can reach what it needs (files, connectors, a computer). If not, say what's missing.
5. Answer in this shape:

```
Model: <name>   Effort: <level>   Setup: <solo / team of N helpers>
Checker: <what checks the result>
Why: <one line>
How to set it: <where to click or what to type in their app>
```

## Part 3: Quota maximizer

1. Get the numbers: weekly % used, strongest-model % used if shown, reset date and time. A screenshot of the usage page is easiest. Where to find it: [references/quota-maximizer.md](references/quota-maximizer.md).
2. Work out hours to reset and give a verdict: **Spend now**, **Spend tomorrow**, **Running hot** (slow down) or **Nothing to do**.
3. If spending: list 3–7 items from the user's own projects, best first. Prefer work that's normally too expensive: turning a repeated task into a workflow, a team-of-experts review, a deep check against the original data.
4. Run each item through Part 1 and Part 2. Check usage between items. Keep 10% spare: stop starting new items at 90% used.
5. An item only counts as done when its outside check passes.

Full steps, thresholds and the spend-list format: [references/quota-maximizer.md](references/quota-maximizer.md).
