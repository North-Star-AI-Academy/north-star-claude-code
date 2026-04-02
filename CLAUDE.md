# North Star AI Academy — Claude Code Workshop

Dit is het oefenproject voor de **Claude Code: The Full Course 2026** training.

## Bij het openen van dit project

### Scenario 1: De gebruiker heeft ZOJUIST deze repo gekloond (vanuit een ander project)

Als de gebruiker zegt iets als "clone de repo..." of "open de map..." en je merkt dat de werkdirectory NIET de workshop-repo is (geen `exercises/` map, geen `.claude/skills/` met marketing skills), dan:

1. Kloon de repo
2. Geef DIRECT deze instructies (in de taal van de gebruiker). **Toon het welkomstmenu NOG NIET.**

**🇳🇱 Nederlands:**

> ✅ **De repo is gekloond!**
>
> De 15 marketing skills en workshop-commando's moeten nu nog geactiveerd worden. Dat gebeurt automatisch zodra je Claude Code opent in de workshop-map.
>
> **Volg deze stappen:**
>
> ---
>
> **VS Code:**
> 1. Ga naar **File → Open Folder**
> 2. Kies de map `north-star-claude-code`
> 3. Open het Claude paneel opnieuw (Ctrl+Shift+P → typ "Claude" → klik op "Claude: Open")
> 4. Je ziet een leeg invoerveld. Typ `start` en druk op **Enter**
>
> **Terminal (Mac/Linux):**
> 1. Typ `exit` om Claude af te sluiten
> 2. Typ `cd north-star-claude-code`
> 3. Typ `claude` om Claude opnieuw te starten
> 4. Typ `start` en druk op **Enter**
>
> **Claude Desktop (de app):**
> 1. Sluit het huidige project
> 2. Open de map `north-star-claude-code` als nieuw project
> 3. Typ `start` in het invoerveld en druk op **Enter**
>
> ---
>
> 💡 **Waarom?** Claude Code leest de skills en commando's alleen bij het opstarten in een projectmap. Door de map te openen en opnieuw te starten worden alle 15 marketing skills en de oefeningen automatisch beschikbaar.

**🇬🇧 English:**

> ✅ **The repo has been cloned!**
>
> The 15 marketing skills and workshop commands still need to be activated. This happens automatically when you open Claude Code in the workshop folder.
>
> **Follow these steps:**
>
> ---
>
> **VS Code:**
> 1. Go to **File → Open Folder**
> 2. Select the `north-star-claude-code` folder
> 3. Reopen the Claude panel (Ctrl+Shift+P → type "Claude" → click "Claude: Open")
> 4. You'll see an empty input field. Type `start` and press **Enter**
>
> **Terminal (Mac/Linux):**
> 1. Type `exit` to close Claude
> 2. Type `cd north-star-claude-code`
> 3. Type `claude` to start Claude again
> 4. Type `start` and press **Enter**
>
> **Claude Desktop (the app):**
> 1. Close the current project
> 2. Open the `north-star-claude-code` folder as a new project
> 3. Type `start` in the input field and press **Enter**
>
> ---
>
> 💡 **Why?** Claude Code only reads skills and commands when it starts up in a project folder. By opening the folder and restarting, all 15 marketing skills and exercises become available automatically.

**STOP hier. Toon NIET het welkomstmenu. De gebruiker moet eerst de map openen en herstarten.**

---

### Scenario 2: De gebruiker opent Claude Code IN de workshop-map

Wanneer de werkdirectory wél de workshop-repo is (er bestaan mappen als `exercises/`, `.claude/skills/`, `templates/`), en de gebruiker stuurt een bericht (zoals "start", "hallo", "hi", "begin", of wat dan ook), **verwelkom ze en geef drie duidelijke keuzes**.

**Detect the user's language** from their first message and respond in that language. If the message is just "start" or unclear, show both language options below.

---

**🇳🇱 Nederlands:**

> **Welkom bij de North Star Claude Code Workshop!** ⭐
>
> ✅ De 15 marketing skills zijn geladen en klaar voor gebruik.
>
> Wat wil je doen?
>
> **1. 📚 Oefeningen starten** — Werk door 8 levels heen en leer Claude Code stap voor stap
> → Zeg: *"Start oefening 1"*
>
> **2. 🎯 Direct met marketing skills werken** — Gebruik de 15 ingebouwde skills meteen
> → Vraag bijvoorbeeld: *"Schrijf een LinkedIn post over AI voor marketeers"* of *"Maak een cold email sequence voor mijn SaaS product"*
> → De skills zijn al actief — gewoon een relevante vraag stellen
>
> **3. 📝 Skills & templates kopiëren naar je eigen project** — Neem de skills en een CLAUDE.md template mee
> → Zeg: *"Kopieer alle marketing skills en het growth-marketer template naar mijn project op [pad]"*
> → ⚠️ **Let op:** na het kopiëren moet je Claude Code opnieuw openen in je eigen projectmap (zelfde stappen als bij de installatie) zodat de skills daar ook worden ingeladen

---

**🇬🇧 English:**

> **Welcome to the North Star Claude Code Workshop!** ⭐
>
> ✅ The 15 marketing skills are loaded and ready to use.
>
> What would you like to do?
>
> **1. 📚 Start the exercises** — Work through 8 levels and learn Claude Code step by step
> → Say: *"Start exercise 1"*
>
> **2. 🎯 Use marketing skills right away** — The 15 built-in skills are ready to go
> → Try asking: *"Write a LinkedIn post about AI for marketers"* or *"Create a cold email sequence for my SaaS product"*
> → Skills are already active — just ask a relevant question
>
> **3. 📝 Copy skills & templates to your own project** — Take the skills and a CLAUDE.md template with you
> → Say: *"Copy all marketing skills and the growth-marketer template to my project at [path]"*
> → ⚠️ **Note:** after copying, you need to reopen Claude Code in your own project folder (same steps as the installation) so the skills get loaded there too

---

## Oefeningen starten / Starting exercises

Wanneer de gebruiker zegt "Start oefening X" of "Start exercise X" of `/start-exercise X`:

1. Determine the student's preferred language:
   - Check the recent conversation history for language clues (Dutch or English)
   - If the student previously interacted in English, use English
   - If the student previously interacted in Dutch, use Dutch
   - If unsure, ask: "In welke taal wil je de oefening doen? / Which language do you prefer? (NL/EN)"

2. Find the exercise folder matching the level number: `exercises/0X-*/`

3. Read the appropriate README based on language:
   - Dutch: read `README.md`
   - English: read `README.en.md` (if it exists, otherwise fall back to `README.md`)

4. Show a brief summary of what the student will learn

5. Read the assignment(s) in the exercise folder

6. Guide the student step by step through the exercise

7. Give hints if the student gets stuck, but don't give the answer right away

Keep your tone friendly, hands-on, and encouraging. The student is likely a marketer, not a developer. Avoid jargon where possible and explain technical terms.

If no level number was provided, show an overview of all 8 levels with a short description per level.

## Repo structuur / Structure

```
.claude/commands/    → Slash commands for exercises
.claude/skills/      → 15 marketing skills (active immediately after opening this folder)
exercises/           → 8 levels (NL: README.md / EN: README.en.md)
templates/nl/        → CLAUDE.md templates (Nederlands)
templates/en/        → CLAUDE.md templates (English)
mcp-configs/         → MCP server configuration examples
cheatsheet/          → Claude Code quick reference
```

## Skills

De `.claude/skills/` map bevat 15 marketing-specifieke skills die **automatisch actief** zijn zodra Claude Code geopend wordt in deze projectmap. Ze activeren wanneer je een relevante vraag stelt:

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
3. **Geef ALTIJD de herstart-instructies per platform (zie Scenario 1 hierboven)** — de gebruiker moet Claude Code opnieuw openen in de projectmap waar de skills naartoe zijn gekopieerd

## Conventies

- Oefeningen: `README.md` (NL) en `README.en.md` (EN) naast elkaar
- Elk exercise level correspondeert met een module uit de training
- Templates in `templates/nl/` en `templates/en/`
- MCP configs in `mcp-configs/` zijn voorbeelden om naar `.mcp.json` te kopiëren
