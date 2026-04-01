# MCP Server Configuraties

MCP (Model Context Protocol) servers geven Claude Code toegang tot externe tools en diensten.

## Hoe te gebruiken

1. Kopieer `examples.json` naar `.mcp.json` in je project root
2. Verwijder de servers die je niet nodig hebt
3. Vul je API keys in
4. Herstart Claude Code

## Aanbevolen voor marketeers

| Server | Waarvoor | Gratis? |
|---|---|---|
| **GitHub** | Repos, issues, PRs | Ja (met token) |
| **Filesystem** | Bestanden buiten project | Ja |
| **Memory** | Persistent geheugen | Ja |
| **Playwright** | Websites bekijken/testen | Ja |
| **Context7** | Live documentatie | Ja |
| **Exa** | Web research | Freemium |

## API keys verkrijgen

### GitHub Personal Access Token
1. Ga naar github.com → Settings → Developer settings → Personal access tokens
2. Maak een "Fine-grained token" aan
3. Geef toegang tot de repos die je nodig hebt

### Exa API Key
1. Ga naar exa.ai en maak een account aan
2. Kopieer je API key uit het dashboard

## Tips

- Begin met 1-2 servers. Voeg pas meer toe als je ze nodig hebt
- Elke MCP server gebruikt resources — minder is meer
- Test na het toevoegen van een server of Claude er toegang toe heeft
