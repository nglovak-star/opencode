# Troubleshooting

**A command doesn't seem to do anything different from just asking normally.**
That's expected — commands in `.claude/commands/` are just pre-written
instructions. You can always get the same result by describing what you
want in plain language; the command is a shortcut.

**The assistant gave an answer that looks wrong.**
Ask it to re-check. It's instructed to label facts vs. inferences vs.
assumptions (`core/instructions.md`) — if a label looks off, point it out.

**A file's format looks broken (table not lining up, etc.).**
Markdown tables are picky about `|` characters. Ask the assistant to fix
the file — don't hand-edit tables unless you're comfortable with markdown.

**I want to change how the assistant behaves.**
Edit `glovak-executive-assistant/core/instructions.md`. Every command reads
from that file, so a change there applies everywhere.

**I want to add a new command.**
Add a new file to `.claude/commands/` following the pattern of the existing
ones (see any file in that folder for the format).

**I think something got lost or overwritten.**
This is a git repository — every change is a commit. Nothing is silently
lost; ask to see the file's git history if something looks off.
