# Claude Code Cheatsheet

## Essential commands

| Command | What it does |
|---|---|
| `claude` | Start Claude Code |
| `claude "question"` | Start with a direct question |
| `claude -c` | Resume previous session |
| `Ctrl+C` | Stop current action |
| `Ctrl+D` | Quit Claude Code |

## Slash commands

| Command | What it does |
|---|---|
| `/help` | Show all commands |
| `/compact` | Compress context (save tokens) |
| `/clear` | Reset session (clean context) |
| `/status` | Show session status |
| `/cost` | Show costs for this session |
| `/model` | Switch model |
| `/bug` | Report a bug |

## Files Claude automatically reads

| File | Scope | Purpose |
|---|---|---|
| `CLAUDE.md` | Project | Project rules and context |
| `~/.claude/CLAUDE.md` | Global | Personal rules |
| `.claude/settings.json` | Project | Technical settings |
| `.claude/skills/*.md` | Project | Skills (auto-activated) |
| `.claude/commands/*.md` | Project | Custom slash commands |
| `.mcp.json` | Project | MCP server configurations |

## Context management rules

1. **Start clean** — New task? New session (`/clear`)
2. **Compress** — Context full? `/compact`
3. **Be specific** — "Fix bug in header.tsx:42" > "there's a bug"

## Permission modes

| Mode | Description |
|---|---|
| **Default** | Asks permission for writes and bash |
| **Allowlist** | You decide which actions are auto-approved |
| **YOLO** | Everything is allowed (not recommended for beginners) |

## Useful patterns

### Have files read
```
Read src/index.html and give feedback on the SEO
```

### Multi-file editing
```
Change the color of all buttons from blue to green
in all files in the src/components/ folder
```

### Research with sub-agents
```
Research simultaneously: (1) the best email subject lines for SaaS,
(2) optimal send times for B2B email, (3) benchmark open rates
```

### Git via Claude
```
Commit all changes with a descriptive message
```

### Activate a custom skill
```
Write a cold email sequence for [product] targeting [audience]
```

## The minimum stack

```
your-project/
├── CLAUDE.md                → Project context
├── .claude/
│   ├── skills/              → Marketing skills
│   │   ├── copywriting.md
│   │   ├── cold-email.md
│   │   └── ...
│   ├── commands/            → Custom workflows
│   │   └── weekly-content.md
│   └── product-context.md   → Brand & audience info
└── .mcp.json                → Tool integrations
```

## Tips for marketers

- **Copy skills**: `cp -r workshop/.claude/skills/ my-project/.claude/skills/`
- **Use a template**: Copy a template from `templates/en/` as your CLAUDE.md
- **Product context first**: Always create your product-context.md first
- **15 minutes daily**: Consistency > intensity when learning Claude Code

---

North Star AI Academy — northstar-academy.ai
