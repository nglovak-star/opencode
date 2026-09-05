# Configuration

Version 1 needs no configuration or credentials to run — it's plain
markdown files plus Claude Code commands.

## Future integrations (not built yet)

When Phase 4 (External Integrations) begins, tools will be added one at a
time. Each will need credentials supplied as environment variables — never
hard-coded into files in this repo. Anticipated variables are listed in
`.env.example` as placeholders only (no real values are ever committed).

| Tool | Env var(s) (placeholder) | Purpose |
|---|---|---|
| Calendar | `GLOVAK_CALENDAR_API_KEY` | Read/write calendar events |
| Email | `GLOVAK_EMAIL_API_KEY` | Draft/send email |
| Web research | `GLOVAK_SEARCH_API_KEY` | Live web search |
| CRM | `GLOVAK_CRM_API_KEY` | Client/lead tracking |
| Automation platform | `GLOVAK_AUTOMATION_API_KEY` | Trigger external workflows |

Nothing in this table is active yet — it documents what *will* be needed,
so setup is a checklist, not a surprise.

## Rule

Never commit a real API key, password, or token to this repo. If a
credential is ever needed, add its variable name here and to
`.env.example` first, then set the real value only in your local
environment or the platform's secret manager — never in a tracked file.
