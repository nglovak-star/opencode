# Decisions Log

Full analysis for significant decisions, using the template in `template.md`.
Labels used throughout: **FACT**, **SOURCE**, **INFERENCE**, **ASSUMPTION**,
**UNKNOWN**. Never present an assumption or inference as a fact.

## Build the Executive Assistant as markdown files, not a coded app — 2026-09-05

- **Objective:** Stand up a working Version 1 personal Executive Assistant
  inside this repo, usable immediately, without requiring Glovak to run or
  maintain custom software.
- **Options considered:**
  1. Plain markdown files + Claude Code slash commands (chosen)
  2. A small custom web/CLI app with a database
  3. A no-code tool (Notion, Airtable, etc.) wired to Claude via API
- **Advantages / disadvantages:**
  - Option 1: No install, no hosting, no dependencies to break (FACT: this
    repo is already git-based and Claude Code already runs here). Downside:
    less structured than a real database; relies on an agent to enforce
    format consistency.
  - Option 2: More powerful later, but adds build/maintenance burden now —
    against the "don't over-engineer V1" instruction.
  - Option 3: Adds an external dependency and account/credential management
    before Version 1 even proves useful.
- **Costs:** Option 1 is effectively free (git storage only). Options 2-3
  would cost setup time and, for option 3, a subscription.
- **Risks:** Markdown files can drift out of format if edited inconsistently
  (mitigated by templates and by the assistant maintaining the format).
- **Opportunity cost:** Minimal — this doesn't block moving to a richer
  system later if needed.
- **Assumptions (ASSUMPTION):** Glovak will primarily interact with this
  system through a Claude Code session in this repo.
- **Unknowns (UNKNOWN):** How often Glovak will actually use this day to
  day; that will surface in the first weekly review.
- **Likely outcome (INFERENCE):** This is the lowest-friction path to a
  working Version 1, matching the stated design philosophy (reliability,
  simplicity, security first).
- **Recommendation:** Proceed with markdown files + slash commands for
  Version 1; revisit only if real usage proves it's not enough.
- **Decision made:** Adopted.
