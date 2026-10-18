# 01 · Install

You need **one** of these. Pick the app you use most. It takes about two minutes.

## Option A: claude.ai (web) and the Claude desktop app

The web app and the desktop app share your account, so one upload covers both.

1. **Turn on code execution (skills need it).** In Claude, open **Settings → Capabilities** and switch on **Code execution and file creation**.
2. **Download the kit.** Open [`dist/leverage-kit.zip`](../dist/leverage-kit.zip) on GitHub and click the download button (the arrow on the right).
3. **Open Skills.** Click **Customize**, then **Skills**.
4. **Upload.** Click **+**, then **Create skill**, then **Upload a skill**, and pick `leverage-kit.zip`.
5. **Check it's on.** You should see **leverage-kit** in your list with its switch turned on.
6. **Test it.** Start a new chat and type: `Which model should I use to write a proposal for a big client?`

Can't see Skills? Claude moves menus around sometimes. Search "Skills" in settings. On a Team
or Enterprise plan, your admin may need to allow skills first.

## Option B: Claude Code (the plugin way, easiest to update)

Inside Claude Code, type:

```
/plugin marketplace add AutomatedMarketer/claude-leverage-kit
/plugin install leverage-kit@leverage-kit
```

When it asks where to install, choose **Install for you**. Restart Claude Code if it asks.

To update later: type `/plugin`, open **Installed**, pick **leverage-kit**, then **Update now**.
Or, in your normal terminal (not inside Claude):

```
claude plugin update leverage-kit@leverage-kit
```

## Option C: Claude Code (copy the folder)

1. Download this repo (green **Code** button → **Download ZIP**) and unzip it.
2. Copy the folder `skills/leverage-kit` into your personal skills folder:
   - Mac / Linux: `~/.claude/skills/leverage-kit`
   - Windows: `C:\Users\<you>\.claude\skills\leverage-kit`
3. Start a new Claude Code session.

## Test that it works

Try each of these in a new chat:

| Type this | You should get |
|---|---|
| `Improve this prompt: write me a blog post about saving money` | A structured prompt with an outcome, a format and a checker |
| `Opus or Sonnet for summarising 50 customer reviews?` | A model, an effort level and one line of why |
| `How much of my plan is left?` | A request for a screenshot of your usage page, then a verdict |

If Claude answers normally without any of that, start your message with "Use leverage-kit to…".
On claude.ai, also check that code execution is still switched on (step 1).

## Uninstall

- **claude.ai / desktop:** Customize → Skills → turn it off or delete it.
- **Claude Code plugin:** `/plugin uninstall leverage-kit@leverage-kit`
- **Claude Code folder:** delete `~/.claude/skills/leverage-kit`.
