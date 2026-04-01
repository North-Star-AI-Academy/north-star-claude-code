# North Star AI Academy — Claude Code Workshop

Dit is het oefenproject voor de **Claude Code: The Full Course 2026** training.
Studenten klonen deze repo en werken door de exercises heen tijdens de live sessie.

**Bilingual support:** All exercises are available in Dutch (NL) and English (EN). Each exercise folder contains a `README.md` (Dutch) and `README.en.md` (English). Templates are organized in `templates/nl/` and `templates/en/`. Slash commands (`/start-exercise`, `/check-progress`) automatically detect the student's language preference from conversation context.

## Repo structuur

```
.claude/commands/    → Slash commands voor oefeningen
.claude/skills/      → Marketing skills (direct bruikbaar)
exercises/           → 8 levels, elk met instructies en opdrachten (NL + EN)
templates/nl/        → Kant-en-klare CLAUDE.md bestanden per marketing rol (Nederlands)
templates/en/        → Ready-made CLAUDE.md files per marketing role (English)
mcp-configs/         → Voorbeeld MCP server configuraties
cheatsheet/          → Claude Code quick reference
```

## Hoe te gebruiken

1. Kloon de repo: `git clone https://github.com/NorthStarAIAcademy/claude-code-workshop.git`
2. Open in je terminal: `cd claude-code-workshop`
3. Start Claude Code: `claude`
4. Begin met Level 1: `/start-exercise 1`

## Skills

De `.claude/skills/` map bevat marketing-specifieke skills die Claude Code automatisch beschikbaar maakt. Gebruik `/skills` om ze te bekijken of activeer ze door een relevante vraag te stellen.

## Conventies

- Alle oefeningen zijn beschikbaar in Nederlands (`README.md`) en Engels (`README.en.md`)
- Elk exercise level correspondeert met een module uit de training
- Templates zijn beschikbaar in `templates/nl/` (Nederlands) en `templates/en/` (English) — kopieer naar je eigen projecten
- MCP configs in `mcp-configs/` kun je kopiëren naar je eigen `.mcp.json`
