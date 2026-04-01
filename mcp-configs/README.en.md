# MCP Server Configurations

MCP (Model Context Protocol) servers give Claude Code access to external tools and services.

## How to use

1. Copy `examples.json` to `.mcp.json` in your project root
2. Remove the servers you don't need
3. Fill in your API keys
4. Restart Claude Code

## Recommended for marketers

| Server | What for | Free? |
|---|---|---|
| **GitHub** | Repos, issues, PRs | Yes (with token) |
| **Filesystem** | Files outside project | Yes |
| **Memory** | Persistent memory | Yes |
| **Playwright** | View/test websites | Yes |
| **Context7** | Live documentation | Yes |
| **Exa** | Web research | Freemium |

## Getting API keys

### GitHub Personal Access Token
1. Go to github.com → Settings → Developer settings → Personal access tokens
2. Create a "Fine-grained token"
3. Grant access to the repos you need

### Exa API Key
1. Go to exa.ai and create an account
2. Copy your API key from the dashboard

## Tips

- Start with 1-2 servers. Only add more when you actually need them
- Each MCP server uses resources — less is more
- After adding a server, test whether Claude has access to it
