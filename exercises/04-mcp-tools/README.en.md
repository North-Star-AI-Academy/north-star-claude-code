# Level 4: MCP Tools — Give Claude Access to External Tools

## Goal
Understand what MCP (Model Context Protocol) is and how to connect Claude Code with external tools for research, data, and automation.

## Theory

MCP servers are bridges between Claude and external services. They run locally and give Claude access to:
- **Web research** (Exa, Brave Search)
- **GitHub** (repos, issues, PRs)
- **Files & databases**
- **Browser automation** (Playwright)
- **And much more...**

Configuration is done via `.mcp.json` in your project root.

## Exercises

### 4.1 — Explore the MCP configuration
```
Read the file mcp-configs/examples.json and explain what each MCP
server does and when you'd use it as a marketer.
```

### 4.2 — Set up GitHub MCP
If you have a GitHub Personal Access Token, create a `.mcp.json`:

```json
{
  "mcpServers": {
    "github": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-github"],
      "env": {
        "GITHUB_PERSONAL_ACCESS_TOKEN": "<your-token>"
      }
    }
  }
}
```

Test it:
```
What open issues are there on the repo NorthStarAIAcademy/claude-code-workshop?
```

### 4.3 — Filesystem MCP
For accessing files outside your project:

```json
{
  "mcpServers": {
    "filesystem": {
      "command": "npx",
      "args": ["-y", "@modelcontextprotocol/server-filesystem", "/path/to/your/marketing-assets"]
    }
  }
}
```

### 4.4 — Research workflow
With Exa MCP you can do web research:
```
Find the latest trends in AI-driven marketing automation
and create a summary of the top 5 developments.
```

### 4.5 — Discover MCP servers
```
What MCP servers exist that are useful for marketers?
Think about CRM, email marketing, analytics, social media, and SEO tools.
```

## Available MCP configs

Check `mcp-configs/` for ready-to-use examples:
- Web research setup
- GitHub integration
- File system access

## Checklist
- [ ] You understand what MCP servers are
- [ ] You've viewed or created a `.mcp.json`
- [ ] You understand which MCP servers are useful for your work

## Done?
Move on to Level 5: `/start-exercise 5`
