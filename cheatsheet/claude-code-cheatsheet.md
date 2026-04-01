# Claude Code Cheatsheet

## Essentiële commando's

| Commando | Wat het doet |
|---|---|
| `claude` | Start Claude Code |
| `claude "vraag"` | Start met een directe vraag |
| `claude -c` | Hervat vorige sessie |
| `Ctrl+C` | Stop huidige actie |
| `Ctrl+D` | Sluit Claude Code af |

## Slash commands

| Commando | Wat het doet |
|---|---|
| `/help` | Toon alle commando's |
| `/compact` | Comprimeer context (bespaar tokens) |
| `/clear` | Reset sessie (schone context) |
| `/status` | Toon sessie status |
| `/cost` | Toon kosten van deze sessie |
| `/model` | Wissel van model |
| `/bug` | Rapporteer een bug |

## Bestanden die Claude automatisch leest

| Bestand | Scope | Doel |
|---|---|---|
| `CLAUDE.md` | Project | Projectregels en context |
| `~/.claude/CLAUDE.md` | Globaal | Persoonlijke regels |
| `.claude/settings.json` | Project | Technische instellingen |
| `.claude/skills/*.md` | Project | Skills (automatisch geactiveerd) |
| `.claude/commands/*.md` | Project | Custom slash commands |
| `.mcp.json` | Project | MCP server configuraties |

## Context management regels

1. **Begin schoon** — Nieuwe taak? Nieuwe sessie (`/clear`)
2. **Comprimeer** — Context vol? `/compact`
3. **Wees specifiek** — "Fix bug in header.tsx:42" > "er is een bug"

## Permission modes

| Mode | Beschrijving |
|---|---|
| **Default** | Vraagt toestemming voor schrijven en bash |
| **Allowlist** | Je bepaalt welke acties automatisch mogen |
| **YOLO** | Alles is toegestaan (niet aanbevolen voor beginners) |

## Handige patronen

### Bestanden laten lezen
```
Lees src/index.html en geef feedback op de SEO
```

### Multi-file bewerking
```
Verander de kleur van alle buttons van blauw naar groen
in alle bestanden in de src/components/ map
```

### Research met sub-agents
```
Onderzoek tegelijk: (1) de beste email subject lines voor SaaS,
(2) optimale verzendtijden voor B2B email, (3) benchmark open rates
```

### Git via Claude
```
Commit alle wijzigingen met een descriptief bericht
```

### Custom skill activeren
```
Schrijf een cold email sequence voor [product] gericht op [doelgroep]
```

## De minimum stack

```
je-project/
├── CLAUDE.md                → Project context
├── .claude/
│   ├── skills/              → Marketing skills
│   │   ├── copywriting.md
│   │   ├── cold-email.md
│   │   └── ...
│   ├── commands/            → Custom workflows
│   │   └── weekly-content.md
│   └── product-context.md   → Brand & audience info
└── .mcp.json                → Tool integraties
```

## Tips voor marketeers

- **Skills kopiëren**: `cp -r workshop/.claude/skills/ mijn-project/.claude/skills/`
- **Template gebruiken**: Kopieer een template uit `templates/` als je CLAUDE.md
- **Eerst product-context**: Maak altijd eerst je product-context.md aan
- **Dagelijks 15 min**: Consistentie > intensiteit bij het leren van Claude Code

---

North Star AI Academy — northstar-academy.ai
