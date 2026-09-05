# Projects

One section per project, using the fields in `template.md`. Keep "Current
status" and "Next action" up to date — those two lines answer "what am I
working on" and "what's next."

## Glovak Executive Assistant (Version 1)

- **Objective:** Build a reliable personal AI Executive Assistant to run
  Glovak's daily work and become the operating system for Glovak Intelligence.
- **Current status:** Phase 1 (Foundation) built — directory structure,
  memory, tasks, projects, ideas, and core commands are in place.
- **Desired outcome:** Glovak can reliably use `/briefing`, `/tasks`,
  `/projects`, `/ideas`, `/review`, `/decision`, `/research`, `/capture`,
  `/focus`, `/status`, `/help` every day.
- **Deadline:** None (ongoing, phased)
- **Next action:** Daily-drive Phase 1, gather feedback, then build Phase 2
  (daily briefing / weekly review / focus / decision support workflows —
  already scaffolded, needs real-world use).
- **Priority:** P2
- **Related tasks:** T001
- **Notes:** Built as plain markdown files in `glovak-executive-assistant/`
  plus Claude Code slash commands in `.claude/commands/`. No external
  integrations yet (Phase 4).
- **Decisions:** See `decisions/decisions-log.md`.
- **Risks:** Scope creep (mitigated by the anti-scope-creep rule in
  `core/instructions.md`); inconsistent daily use (mitigated by keeping
  `/briefing` fast and low-friction).

## Glovak Intelligence — Hospitality AI

- **Objective:** Develop AI solutions for hospitality businesses.
- **Current status:** Early / pre-work. Strategic direction defined; no
  active workstreams tracked here yet.
- **Desired outcome:** Proven internal workflows (built via the Executive
  Assistant) that can later become reusable, productized AI systems.
- **Deadline:** None yet.
- **Next action:** Not started — intentionally deferred until the Executive
  Assistant (this project, above) is running reliably.
- **Priority:** P3 (for now — will rise once Version 1 of the assistant is
  proven)
- **Related tasks:** —
- **Notes:** Do not build client-facing hospitality features yet — see
  `core/instructions.md` anti-scope-creep rule.
- **Decisions:** —
- **Risks:** Starting too early, before internal workflows are proven.
