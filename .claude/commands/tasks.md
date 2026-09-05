---
description: View, add, or update tasks
argument-hint: [optional: what to add/change, e.g. "add: call vendor, P3"]
---

Read `glovak-executive-assistant/core/instructions.md` first for persona and
rules (priority system: P1 Critical, P2 Important, P3 Normal, P4 Optional).

Arguments given: $ARGUMENTS

- If no arguments: show the current contents of
  `glovak-executive-assistant/tasks/tasks.md`, grouped by priority, and call
  out anything overdue (compare `Due` dates to today) or missing a priority.
- If arguments describe a new task: add a row to
  `glovak-executive-assistant/tasks/tasks.md` using the format in
  `glovak-executive-assistant/tasks/template.md`. Assign the next `T###` ID.
  If priority/category/due date weren't given, ask only if truly ambiguous —
  otherwise make a reasonable default and say what you chose.
- If arguments describe a status change (e.g. "mark T003 done"): update the
  row. If marking a task `Done`, move the row to
  `glovak-executive-assistant/tasks/completed.md` and remove it from
  `tasks.md`.
- If a task looks large/vague, offer to break it into smaller actions before
  adding it.

Adding/updating/completing tasks is low-risk — no confirmation needed.
Deleting a task outright (not completing it) requires confirmation per the
guardrails in `core/instructions.md`.
