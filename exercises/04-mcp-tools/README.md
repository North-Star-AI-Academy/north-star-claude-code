# Level 4: MCP Tools — Geef Claude toegang tot externe tools

## Doel
Begrijpen wat MCP (Model Context Protocol) is en hoe je Claude Code verbindt met externe tools voor research, data, en automatisering.

## Theorie

MCP servers zijn bruggen tussen Claude en externe diensten. Ze draaien lokaal en geven Claude toegang tot:
- **Web research** (Exa, Brave Search)
- **GitHub** (repos, issues, PRs)
- **Bestanden & databases**
- **Browser automatisering** (Playwright)
- **En veel meer...**

Configuratie gaat via `.mcp.json` in je project root.

## Opdrachten

### 4.1 — MCP configuratie bekijken
```
Lees het bestand mcp-configs/examples.json en leg uit wat elke MCP
server doet en wanneer je die zou gebruiken als marketeer.
```

### 4.2 — GitHub MCP instellen
Als je een GitHub Personal Access Token hebt, maak een `.mcp.json`:

```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "<jouw-token>"
      }
    }
  }
}
```

Test het:
```
Welke open issues staan er op de repo NorthStarAIAcademy/claude-code-workshop?
```

### 4.3 — Filesystem MCP
Voor toegang tot bestanden buiten je project:

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/pad/naar/je/marketing-assets"]
    }
  }
}
```

### 4.4 — Research workflow
Met Exa MCP kun je web research doen:
```
Zoek de laatste trends in AI-gestuurde marketing automation
en maak een samenvatting van de top 5 ontwikkelingen.
```

### 4.5 — MCP servers ontdekken
```
Welke MCP servers bestaan er die nuttig zijn voor marketeers?
Denk aan CRM, email marketing, analytics, social media, en SEO tools.
```

## Beschikbare MCP configs

Bekijk `mcp-configs/` voor kant-en-klare voorbeelden:
- Web research setup
- GitHub integration
- Bestandssysteem toegang

## Checklist
- [ ] Je begrijpt wat MCP servers zijn
- [ ] Je hebt een `.mcp.json` bekeken of aangemaakt
- [ ] Je begrijpt welke MCP servers nuttig zijn voor jouw werk

## Klaar?
Ga door naar Level 5: `/start-exercise 5`
