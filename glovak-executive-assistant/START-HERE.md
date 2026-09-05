# START HERE

This is your personal Executive Assistant. You don't need to understand any
code to use it — everything below is plain language.

## What you actually do

1. Open this repository in Claude Code (or a Claude Code web/desktop
   session pointed at this repo).
2. Type a command, like:

   ```
   /briefing
   ```

3. The assistant reads your files, does the work, and either shows you the
   result or updates the relevant file (and tells you what it changed).

That's the whole loop. No installation, no setup, no server.

## The commands you'll use most

- **`/briefing`** — Start your day. Shows your top priorities, schedule,
  important tasks, and one recommended next action.
- **`/tasks`** — Add a task ("add a task: call the accountant, P2, due
  Friday") or see your task list.
- **`/status`** — Quick snapshot: what am I working on, what's overdue,
  what's next.
- **`/focus`** — "What should I be doing right now?" Use this when you feel
  scattered.
- **`/capture`** — Got an idea mid-task? Say "I have an idea..." or run
  `/capture` and it gets filed in the Idea Inbox instead of derailing you.
- **`/review`** — Run this once a week (Friday afternoon or Monday morning,
  your call) to see wins, misses, and next week's priorities.
- **`/decision`** — When you're stuck on a real decision, this walks through
  options, risks, and a recommendation — clearly separating facts from
  guesses.
- **`/help`** — Full list of commands, any time you forget.

## What this system will NOT do without asking you first

- Send an email, text, or message on your behalf.
- Delete anything important.
- Spend money or change settings that matter.
- Publish anything.

It drafts first. You approve. Then it sends. Always.

## If you want to change something

- Want the assistant to behave differently? Tell it in plain language, or
  say so and it will point you to the one file that controls behavior
  (`core/instructions.md`).
- Want to add a new kind of command? Just ask — you don't need to write it
  yourself.

## If something goes wrong

See `docs/troubleshooting.md`, or just tell the assistant what looks wrong —
it can usually fix it directly.

## What NOT to ask for yet

This is Version 1: a personal assistant for you. It is not yet a
client-facing product, and it doesn't have calendar/email/CRM access yet.
If you ask for something outside that scope, the assistant will say so,
file it as an idea for later, and bring you back to what matters today.
