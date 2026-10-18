# Claude Leverage Kit

**AI is leverage. Learn to use it.**

A free starter kit for people who are new to Claude and want to get far more out of it,
starting today. One install gives Claude three new habits:

| Part | What it does for you |
|---|---|
| **1. Prompt builder** | Turns your rough, rambling request into a strong prompt: the real goal, how an expert would do it, and how you'll know it's right |
| **2. Model picker** | Tells you which Claude model and effort level to use, and when a job deserves a team of helpers |
| **3. Plan maximizer** | Checks how much of your Claude plan is left before it resets, and spends the spare on your most valuable work |

They work alone, or chained together: **build the prompt → pick the model → do the work → check it.**

---

## Why this exists

It's easy to use AI as a faster typewriter: ask for a task, get a decent answer, stop there.

The people getting extraordinary results do four things differently:

1. **They ask for the result, not just the task.** Not "fill in my slides", but "help me win this client".
2. **They ask for the professional's way.** Real methods, the original data and a bold target.
3. **They bring in other fields.** A team of specialists, including critics whose job is finding problems.
4. **They never let AI grade its own homework.** Something else always checks the result.

And they use the plan they already pay for, all of it, every week.

This kit builds those habits into Claude, so you get them without having to remember them.

---

## Install (about 2 minutes)

Pick the app you use. You only need one.

### claude.ai (web) and the Claude desktop app

1. In Claude, open **Settings → Capabilities** and switch on **Code execution and file creation** (skills need it).
2. Download **[leverage-kit.zip](dist/leverage-kit.zip)** (click it, then the download button).
3. Open **Customize → Skills**, click **+** → **Create skill** → **Upload a skill**, and choose the zip.
4. Done. It works in the desktop app too, because it's the same account.

Can't find Skills? Menu names move sometimes. Search "Skills" in Claude's settings.

### Claude Code

Type these two lines inside Claude Code:

```
/plugin marketplace add AutomatedMarketer/claude-leverage-kit
/plugin install leverage-kit@leverage-kit
```

Or copy the `skills/leverage-kit` folder into `~/.claude/skills/`.

Full steps with pictures-in-words: [docs/01-install.md](docs/01-install.md).

---

## How to use it

You don't need special commands. Just talk to Claude normally. These phrases wake it up:

| You want to… | Say something like |
|---|---|
| Improve a prompt | "Improve this prompt: …" or paste a long messy request and say "make this better" |
| Push a task further | "Make this more ambitious" · "Go deeper on this" · "Bring in experts" |
| Pick a model | "Which model should I use for this?" · "Opus or Sonnet?" · "What effort level?" |
| Use your spare plan | "How much of my plan is left?" (attach a screenshot of your usage page) · "My limit resets soon, what should I do?" |
| Do something really well | "This is important. Build the prompt, pick the model, then do it." |

You can also name it directly: "Use leverage-kit to…".

### A 60-second example

**You type:**
> need an email for people who downloaded my free guide but never booked a call, make it sound like me, short, mention the free 15 min call

**Claude (with the kit) hands back** a ready-to-paste prompt with:
- the **outcome** (more people book the call),
- the **method** an email expert would use,
- the **format** (3 subject lines, a short body, one link),
- **who checks it** (a fresh chat with a checklist, then you),
- the **model** to run it on (Opus, medium effort).

Then it asks: "Run it now, or copy it into a new chat?"

More examples for business owners: [docs/06-examples.md](docs/06-examples.md).

---

## How to get the most out of it

- **Use it on what matters, skip it on what doesn't.** Quick questions don't need it. Proposals, launches, client work and anything you repeat every week do.
- **Name the result behind the request.** If you want the email to get bookings, say so. Claude can only aim at what it can see.
- **Give it the original material.** The full spreadsheet, the whole transcript, the real numbers. Not your summary of them.
- **Try the bold target.** When it suggests one next to the safe goal, give it a go. Worst case, you land on the safe version.
- **Always run the check.** The kit names one for every important job. Use it.
- **Look at your plan on the day before it resets.** Ask "how much of my plan is left?" Spare usage is the cheapest time to do your most ambitious work.
- **Turn repeats into workflows.** If you ask for the same thing every week, ask Claude to make it repeatable once.

---

## How this makes you the 1%

Most people ask AI for **tasks**. The top 1% ask for **results**, done the **professional's way**,
with **more than one point of view**, and **checked by something other than the AI**.

| Most people | The 1% |
|---|---|
| "Write a product description" | "Help a buyer decide in two minutes. Use what a conversion copywriter would use. Have two critics tear it apart first." |
| Use whatever model is selected | Match the model and effort to the job |
| Trust the first answer | Name an outside check before starting |
| Let unused usage expire | Spend the spare on their highest-value work |
| Ask for the same thing every week | Make it repeatable once |

None of this needs coding. It needs the habit. This kit is the habit.

The full playbook: [docs/05-the-1-percent-playbook.md](docs/05-the-1-percent-playbook.md).

---

## How-to guides

| Guide | What you'll learn |
|---|---|
| [01 · Install](docs/01-install.md) | Set it up on claude.ai, the desktop app or Claude Code |
| [02 · Better prompts](docs/02-better-prompts.md) | Turn any rough request into a strong one |
| [03 · The right model](docs/03-right-model.md) | Which model, which effort, and when to use helpers |
| [04 · Use your whole plan](docs/04-use-your-whole-plan.md) | Find spare usage and spend it before the reset |
| [05 · The 1% playbook](docs/05-the-1-percent-playbook.md) | The habits that make AI results stand out |
| [06 · Examples](docs/06-examples.md) | Before-and-after prompts for real business jobs |

---

## Questions

**Does it cost anything?** No. The kit is free. It runs inside the Claude plan you already have.

**Does it work on the free plan?** The prompt builder and model picker work on any plan that supports skills. The plan maximizer is most useful on paid plans, which have weekly limits.

**Will it change my settings or do things on its own?** No. It suggests models and effort levels; you choose them. It never sends, posts, buys or deletes anything without asking you first.

**Does it use more of my plan?** Normally no. The only expensive option is a team of helpers, and it always asks before using one.

**Model names in the kit are out of date.** Models change fast. The kit tells Claude to use the closest match: the biggest model for the hardest jobs, the smallest for simple ones.

**Does this work with ChatGPT or other AI tools?** The skill file is built for Claude. The ideas (outcome, expert's way, other fields, outside check) work with any AI.

---

## About

Made by **Nuno Tavares**, AI Consultant · AI Automations, Agents & Skills Expert · GoHighLevel Expert.

More free training on YouTube: [@AutomatedMarketer](https://www.youtube.com/@AutomatedMarketer).

Released under the [MIT License](LICENSE): use it, share it, change it.
