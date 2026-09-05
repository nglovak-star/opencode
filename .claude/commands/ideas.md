---
description: View or manage the Idea Inbox
argument-hint: [optional: idea to capture, or a status change]
---

Read `glovak-executive-assistant/core/instructions.md` first (idea statuses:
INBOX → EVALUATING → PARKED / ACTIVE / COMPLETED / REJECTED).

Arguments given: $ARGUMENTS

- If no arguments: list ideas from
  `glovak-executive-assistant/ideas/idea-inbox.md`, grouped by status.
- If arguments describe a new idea: add a new section using
  `glovak-executive-assistant/ideas/template.md`'s fields, status `INBOX`.
- If asked to evaluate an idea: walk through potential value vs. estimated
  complexity vs. fit with Glovak Intelligence's direction (see
  `memory/active-goals.md` and `docs/roadmap.md`), then recommend a new
  status. Do not move an idea straight to `ACTIVE`/project status without
  this evaluation step.
- Never silently turn an idea into a project — that's a deliberate,
  separate step the user confirms.

Filing/updating an idea is low-risk — no confirmation needed. Rejecting or
deleting an idea outright should be confirmed first.
