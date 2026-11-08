# NUS AIDF AI Academy · Module 2: Vibe Coding

Welcome! This is your starter project for **Saturday 14 November 2026**.
You will build web apps by describing them to an AI coding agent (GitHub Copilot), then testing and improving them.

## 1. Open your own copy

1. Click **Use this template → Open in a codespace** (top right of this page).
2. Wait about a minute. VS Code opens in your browser.
3. Open **Copilot Chat** (Copilot icon at the top of the window) and set the mode to **Agent**.

## 2. Run your app

In the terminal (menu **Terminal → New Terminal**), type:

```
python3 -m http.server 8000
```

Click **Open in Browser** when the pop-up appears (or open the **Ports** tab and click port 8000).
Refresh that browser tab after every change. Leave the server running; press `Ctrl+C` to stop it.

## 3. Save your work (commit)

Every time something works: **Source Control** icon (left bar) → type a short message → **Commit** → **Sync Changes**.

---

## Prompts for today

Copy these into Copilot Chat (Agent mode). Change the parts in [brackets].

### Hello, World (Topic 3)

```
Create index.html: a page that says "Hello from [your name]" in dark blue and orange,
with a button that shows a random fun fact about Singapore.
```

Check: are the fun facts true?

### Savings Goal Calculator (Topic 4)

```
Build a Savings Goal Calculator as one index.html file with HTML, CSS and JavaScript.
It is for a secondary school student saving up for something.
Inputs: goal, savings so far, saving per week (S$). On Calculate, show weeks needed
(round up), the date the goal is reached, and a progress bar.
Clean and phone-friendly, dark blue #004282 with orange #ed7f0d.
No external libraries. If an input is empty, negative or not a number, show a friendly message.
```

Work it out first: goal 600, saved 120, 30 per week → **16 weeks**.

Follow-up ideas (one at a time, then test, then commit):

- `Make the Calculate button bigger and centred.`
- `Show the date like "Sat, 27 Feb 2027".`
- `Add a line chart of savings week by week.`

### Test data (Topic 4)

| Type | Goal · saved · per week (S$) | Expected result |
| --- | --- | --- |
| Normal | 600 · 120 · 30 | 16 weeks |
| Boundary | 600 · 590 · 30 | 1 week (rounded up) |
| Boundary | 600 · 600 · 30 | 0 weeks: "You're already there!" |
| Abnormal | 600 · 120 · 0 | A friendly message, not "Infinity" |
| Abnormal | abc · −50 · (empty) | A friendly message, no crash |

### Asking for a fix (Topic 5)

```
I entered [what you typed].
I expected [what should happen].
It shows [what actually happened].
Error in the Console: [paste it, or "none"].
Explain why this happens in simple words, then fix only this problem.
```

### Bug Hunt (Topic 5)

Open `bug.html` in your browser (`http://…/bug.html`). It should show S$1157.63 for S$1,000 at 5% for 3 years. Find the bugs before asking Copilot!

### Your group project (Topic 6)

Fill in `SPEC_CARD.md` with your team first. Then paste it into Copilot as the start of your first build prompt.
Record the prompts you used in `PROMPT_LOG.md`: you will need them for your presentation.

---

## Rules for today

- **No secrets:** never put passwords or API keys in your code. This repository can be seen by others.
- **Made-up data only:** no real names, NRIC, phone numbers or bank details.
- **Check the maths:** work out one answer by hand and test it.
- **Be honest:** say that AI helped you, and be ready to explain how your code works.
- **Not financial advice:** money apps here are for learning. Add a line such as "For learning only. Not financial advice."

Using Copilot Free instead of Copilot Student? You can stop GitHub using your chats for AI training at
[github.com/settings/copilot/features](https://github.com/settings/copilot/features) → Privacy.
