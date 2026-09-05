---
description: View, add, or update projects
argument-hint: [optional: project name and what to change]
---

Read `glovak-executive-assistant/core/instructions.md` first.

Arguments given: $ARGUMENTS

- If no arguments: summarize `glovak-executive-assistant/projects/projects.md`
  — for each project, show status and next action. Flag any project with a
  stale-looking "Current status" (no progress implied) or no clear next
  action as potentially stalled.
- If arguments name a new project: add a new `## <Project Name>` section
  using the fields in `glovak-executive-assistant/projects/template.md`.
  Ask only for fields you genuinely can't infer; make reasonable defaults
  for the rest and say what you chose.
- If arguments describe an update to an existing project: edit that
  project's section directly (status, next action, notes, risks, etc.).
- Be ready to answer, using this file: "What am I currently working on?",
  "What is the next action [on project X]?", "What projects are stalled?"

Adding/updating a project is low-risk — no confirmation needed. Removing a
project outright requires confirmation.
