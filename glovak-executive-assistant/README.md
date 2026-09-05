# Glovak Executive Assistant

A personal AI Executive Assistant, built to run inside Claude Code, that
helps organize work, manage priorities, plan days, capture ideas, run
projects, do research, draft communications, and support decisions.

**New here? Read `START-HERE.md` first — it's written for a non-programmer.**

## What this is

Version 1 of a system meant to become the operational "brain" for building
Glovak Intelligence. It's intentionally simple: everything is stored as
plain markdown files in this folder, and a set of Claude Code slash
commands (in `.claude/commands/` at the repo root) know how to read and
update them.

There is no app to install and no server to run. Open this repo in Claude
Code and use the commands below.

## Structure

```
glovak-executive-assistant/
  core/            Persona, rules, and guardrails the assistant follows
  config/          Configuration docs + credential placeholders (Phase 4)
  tasks/           Active + completed tasks
  projects/        Active projects
  ideas/           Idea Inbox
  knowledge/       Reference notes, by category
  daily/           Daily briefings (one file per day)
  weekly/          Weekly executive reviews
  decisions/       Decision-support analyses
  communications/  Drafts + templates for emails, messages, agendas
  research/        Research log
  memory/          Durable memory (profile, goals, preferences, lessons...)
  logs/            Self-improvement backlog
  docs/            Roadmap + troubleshooting (this doc's neighbors)
```

## Commands

Run these as Claude Code slash commands (typed at the start of a message):

| Command | What it does |
|---|---|
| `/briefing` | Produce today's executive briefing |
| `/tasks` | View/add/update tasks |
| `/projects` | View/add/update projects |
| `/ideas` | View or capture ideas |
| `/review` | Run the weekly executive review |
| `/decision` | Work through a decision using the decision-support framework |
| `/research` | Research a topic with labeled findings |
| `/capture` | Quickly capture an idea, note, or piece of information |
| `/focus` | "What should I be doing right now?" |
| `/status` | Snapshot of tasks, projects, and priorities |
| `/help` | List commands and how to use this system |

You don't have to use exact commands — plain requests work too (e.g. "add a
task to call the printer vendor, P3"). Commands are shortcuts, not a
required syntax.

## How memory works

See `memory/README.md`. Short version: durable facts (goals, preferences,
decisions, lessons) live in dedicated files and get updated when something
actually changes — not on every conversation.

## How to add a tool/integration later

Don't build it into `core/instructions.md` directly. Instead:
1. Add the credential's env var name to `config/config.md` and
   `config/.env.example` (placeholder only, never a real value).
2. Add a new command or extend an existing one to use the tool.
3. Update `docs/roadmap.md` to move it from "planned" to "built."

## How to modify behavior

Edit `core/instructions.md` — every command is instructed to read it first,
so a single edit changes behavior system-wide.

## Troubleshooting

See `docs/troubleshooting.md`.

## Roadmap / what's next

See `docs/roadmap.md`. Short version: Phase 1 (this) is the foundation.
Phase 2 (daily briefing / weekly review / focus / decisions) is scaffolded
but needs real-world use before being called done. Later phases add
knowledge/research depth, then external tools, then advanced capabilities —
in that order, not before.
