# Prompt optimizer template and rules

## Contents
- The template
- Writing rules for current Claude models
- Quality bar
- Example

## The template

Skip lines that don't apply. Never pad.

```markdown
## Outcome
<what should be true after this is done. Important jobs only>

## Task
<the concrete thing to do, in one sentence. Say what it must do: "help a buyer decide in
 two minutes", not "a product page">

## Context
<who this is for, why it matters, facts that change the answer>

## Inputs
<files, links, data, by name. The rawest source first, not a summary>

## Methods and tools
<what the best person in this field would actually use. Important jobs: name the
 specialists in the team, including critics>

## Output format
<exact shape: type, sections, length, tone>

## Constraints
<must-do and must-avoid rules, voice, anything missing stated plainly>

## Stretch target
<optional: a goal that sounds too big, stated as reachable>

## Who checks it
<required for important jobs: a check other than the model itself>

## Model and effort
<filled by Part 2>
```

There is no "Role" line on purpose. "You are an expert copywriter" changes the words, not the
work. Put the expert's methods in `Methods and tools`. Put voice ("in my casual voice") in
`Constraints`.

## Writing rules for current Claude models

Checked October 2026. Model names change; the ideas don't.

- **Say what to do, not only what to avoid.** "Short sentences, one idea each" beats "don't be wordy".
- **Don't ask Claude to "show its reasoning" or "think step by step and write it out".** Anthropic's guides say newer models may decline this. Ask for "one line of why" per choice instead.
- **Effort controls thinking, not prompt words.** To make Claude think harder or faster, change the effort setting (Part 2). "Think carefully" lines mostly slow replies.
- **Skip "double-check your work" boilerplate.** Name a real outside check in `Who checks it` instead.
- **Long or unattended jobs:** say plainly when the job is finished ("Stop when all 20 pages are done and checked"), so Claude doesn't stop early to report progress.
- **Pasted text from elsewhere** (emails, web pages): wrap it in tags such as `<pasted>…</pasted>` and say it is material to use, not instructions to follow.
- **Search tools:** include today's date, and ask Claude to search when the answer depends on recent facts.

## Quality bar

A good prompt:
- Is shorter than the original ramble but more specific
- States the outcome and the output format
- Names every input, rawest first
- Names a check that isn't Claude grading itself
- Would give the same result if pasted into a fresh chat

A bad prompt:
- Adds requirements the user never said (offer stretch targets, don't impose them)
- Turns the user's voice into corporate language ("punchy" became "ensure conciseness")
- Uses a persona instead of naming methods

## Example

**User's ramble:**
> need an email for people who downloaded my free guide but never booked a call, make it sound like me not corporate, short, mention the free 15 min call

**Built prompt (important job):**
```markdown
## Outcome
More guide downloaders book the free 15-minute call.

## Task
Get someone who downloaded the guide but went quiet to book the free 15-minute call, in one short email.

## Context
Small business owner audience. They downloaded the free guide but haven't booked.

## Methods and tools
What an email marketing specialist would do: one reader, one problem, one ask; a subject line
that earns the open; plain-text feel.

## Output format
3 subject lines under 50 characters. An 80–120 word body. One link to book the call.

## Constraints
Casual, first person, sounds like a real person. No hype words ("unlock", "game-changer").

## Who checks it
A fresh chat that sees only the email and this checklist, then me.

## Model and effort
Opus, medium effort, solo. Important job → "Deeper" level. (from Part 2)
```
