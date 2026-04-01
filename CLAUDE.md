# North Star AI Academy — Claude Code Workshop

Dit is het oefenproject voor de **Claude Code: The Full Course 2026** training.

## Bij het openen van dit project

Wanneer een gebruiker dit project opent of kloont, **verwelkom ze en geef drie duidelijke keuzes**:

---

### 🇳🇱 Nederlands

> **Welkom bij de North Star Claude Code Workshop!** ⭐
>
> Wat wil je doen?
>
> **1. 📚 Oefeningen starten** — Werk door 8 levels heen en leer Claude Code stap voor stap
> → Typ `/start-exercise 1` om te beginnen
>
> **2. 🎯 Direct met marketing skills werken** — Gebruik de 15 ingebouwde skills meteen
> → Vraag bijvoorbeeld: *"Schrijf een LinkedIn post over AI voor marketeers"* of *"Maak een cold email sequence voor mijn SaaS product"*
> → De skills zijn al actief — gewoon een relevante vraag stellen
>
> **3. 📝 Skills & templates kopiëren naar je eigen project** — Neem de skills en een CLAUDE.md template mee
> → Zeg: *"Kopieer alle marketing skills en het growth-marketer template naar mijn project op [pad]"*
> → ⚠️ **Belangrijk: na het kopiëren moet je Claude Code herstarten** in je eigen project zodat de skills worden ingeladen. Sluit Claude af en start opnieuw in je projectmap.

---

### 🇬🇧 English

> **Welcome to the North Star Claude Code Workshop!** ⭐
>
> What would you like to do?
>
> **1. 📚 Start the exercises** — Work through 8 levels and learn Claude Code step by step
> → Type `/start-exercise 1` to begin
>
> **2. 🎯 Use marketing skills right away** — The 15 built-in skills are ready to go
> → Try asking: *"Write a LinkedIn post about AI for marketers"* or *"Create a cold email sequence for my SaaS product"*
> → Skills are already active — just ask a relevant question
>
> **3. 📝 Copy skills & templates to your own project** — Take the skills and a CLAUDE.md template with you
> → Say: *"Copy all marketing skills and the growth-marketer template to my project at [path]"*
> → ⚠️ **Important: after copying, you need to restart Claude Code** in your own project so the skills get loaded. Close Claude and start it again in your project folder.

---

**Detect the user's language** from their first message and respond in that language. If unclear, show both options above.

## Repo structuur / Structure

```
.claude/commands/    → Slash commands for exercises
.claude/skills/      → 15 marketing skills (active immediately)
exercises/           → 8 levels (NL: README.md / EN: README.en.md)
templates/nl/        → CLAUDE.md templates (Nederlands)
templates/en/        → CLAUDE.md templates (English)
mcp-configs/         → MCP server configuration examples
cheatsheet/          → Claude Code quick reference
```

## Skills

De `.claude/skills/` map bevat 15 marketing-specifieke skills die **automatisch actief** zijn in dit project. Ze activeren wanneer je een relevante vraag stelt:

| Skill | Trigger voorbeeld |
|---|---|
| `copywriting` | "schrijf copy voor..." / "write copy for..." |
| `cold-email` | "cold email sequence..." |
| `social-content` | "LinkedIn post..." |
| `email-sequence` | "drip campaign..." / "nurture flow..." |
| `seo-audit` | "SEO check..." |
| `ad-creative` | "Google Ads copy..." |
| `content-strategy` | "content plan..." |
| `page-cro` | "conversie verbeteren..." / "improve conversions..." |
| `landing-page` | "landing page maken..." / "build a landing page..." |
| `competitor-analysis` | "concurrent analyseren..." / "analyze competitor..." |
| `schema-markup` | "structured data..." / "JSON-LD..." |
| `marketing-ideas` | "marketing ideeën..." / "marketing ideas..." |
| `copy-editing` | "verbeter deze copy..." / "improve this copy..." |
| `ab-testing` | "A/B test opzetten..." / "set up A/B test..." |
| `product-context` | "brand context..." / "product context..." |

## ⚠️ Skills kopiëren naar een ander project

Wanneer een gebruiker skills wil kopiëren naar een eigen project:

1. Kopieer de `.claude/skills/` map naar het doelproject
2. Optioneel: kopieer een template uit `templates/nl/` of `templates/en/` als `CLAUDE.md`
3. **Geef ALTIJD deze waarschuwing:**

> ⚠️ **Herstart vereist!** De skills zijn gekopieerd, maar Claude Code leest skills alleen bij het opstarten. Sluit Claude Code af en start het opnieuw in je projectmap:
> - **Terminal**: typ `exit` of druk op `Ctrl+D`, dan `claude` in je projectmap
> - **VS Code**: sluit het Claude paneel en open het opnieuw
> - **Claude Desktop**: sluit het project en open het opnieuw
>
> Na de herstart zijn alle marketing skills direct beschikbaar.

## Conventies

- Oefeningen: `README.md` (NL) en `README.en.md` (EN) naast elkaar
- Elk exercise level correspondeert met een module uit de training
- Templates in `templates/nl/` en `templates/en/`
- MCP configs in `mcp-configs/` zijn voorbeelden om naar `.mcp.json` te kopiëren
