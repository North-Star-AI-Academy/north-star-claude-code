# North Star AI Academy — Claude Code Workshop

Dit is het oefenproject voor de **Claude Code: The Full Course 2026** training.
Studenten klonen deze repo en werken door de exercises heen tijdens de live sessie.

## Repo structuur

```
.claude/commands/    → Slash commands voor oefeningen
.claude/skills/      → Marketing skills (direct bruikbaar)
exercises/           → 8 levels, elk met instructies en opdrachten
templates/           → Kant-en-klare CLAUDE.md bestanden per marketing rol
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

- Alle oefeningen zijn in het Nederlands en Engels
- Elk exercise level correspondeert met een module uit de training
- Bestanden in `templates/` zijn bedoeld om te kopiëren naar je eigen projecten
- MCP configs in `mcp-configs/` kun je kopiëren naar je eigen `.mcp.json`
